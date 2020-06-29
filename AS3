#include <iostream>

using namespace std;
// function prototype
void getJudgeData(double &);
void calcScore(double, double, double, double, double);
double findLowest(double, double, double, double, double);
double findHighest(double, double, double, double, double);

//function main

int main( )
{
    double score1;
	double score2;
	double score3;
	double score4;
	double score5;

    // comment 1: ask for each judge's score.
	getJudgeData(score1);
	getJudgeData(score2);
	getJudgeData(score3);
	getJudgeData(score4);
	getJudgeData(score5);

    // comment 2: calculate the average sum without the highest and lowest one, and print out the result.
	calcScore(score1, score2, score3, score4, score5);

    return 0;
}

void getJudgeData(double &score)
{
    // comment 3: prompt the user to input the score.
    cout << "Enter a judge's score: ";
    cin >> score;

    // comment 4: if the score is invalid(smaller than 0 or bigger than 10) then input warning and asking for the score agian until it is vaid
    while (score < 0 || score >10 )
    {
        cout << "The score must be between 0.0 and 10.0\n";
        cout << "Enter a judge's score: ";
        cin >> score;
    }
};


void calcScore(double s1, double s2, double s3, double s4, double s5)
{
    double sum = 0, mean, min_s, max_s;
    double ar1[5] = {s1, s2, s3, s4, s5};

    // comment 5: call the findLowest() and findHighest() function to find the highest and lowest number, and assign them to min_s and max_s individually.
    min_s = findLowest(s1, s2, s3, s4, s5);
    max_s = findHighest(s1, s2, s3, s4, s5);

    // comment 6: we use for loop to determine whether the element is the highest or lowest one, if so, we will not add it to the 'sum' variable.
    for (int i=0;i<5;i++)
    {
        if (ar1[i] != min_s && ar1[i] != max_s)
        {
            sum += ar1[i];
        }
    }

    // comment 7: due to the loop above, we summed up the 3 scores without adding the highest and lowest score, now we divide it by 3 to get the mean score.
    mean = sum/3 ;

    // comment 8: print out the result.
    cout << "\nAfter dropping the lowest and highest scores, the average score was " << mean << ".\n";
};


double findLowest(double s1, double s2, double s3, double s4, double s5)
{
    double array[5] = {s1, s2, s3, s4, s5};
    double temp =11; // comment 9: set the default of temp as 11 in order to get the first comparison below correcctly.

    // comment 10: this for loop will compare each element among the five scores.
    for(int i=0;i<5;i++)
    {
        if(array[i]<temp) // comment 11: if the element is lower than the temp then change the temp to the current elemetn, by this, we can find the lowest in the end.
        temp=array[i];
    }
    return temp;
};


double findHighest(double s1, double s2, double s3, double s4, double s5)
{
    double array[5] = {s1, s2, s3, s4, s5};
    double temp = 0; // comment 12: set the default of temp as 0 in order to get the first comparison below correcctly.

    // comment 13: this for loop compare each element among the five scores.
    for(int i=0;i<5;i++)
    {
        if(array[i]>temp) // comment 14: if the element is higher than the temp then change the temp to the current elemetn, by this, we can find the highest in the end.
        temp=array[i];
    }
    return temp;
};
