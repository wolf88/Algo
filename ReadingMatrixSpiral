#include <map>
#include <iostream>
#include <sstream>
#include<string>
#include<vector>
using namespace std;



#include <stdio.h>
#include <map>
using namespace std;
vector<vector<int >> transpose(vector<vector<int >>& A);
int main()
{
	vector<vector<int >> A = { {1,2,3} ,
	                           {4,5,6},
	                           {7,8,9} };

	int S = A.size();
	vector<int> spiro;
	spiro = A[0];

	for (int k = 0; k < S; k++)
	{
		vector<int> T;
		A.erase(A.begin() + 0);
		if (A.size()==1)
		{ 
			T = A[0];
			for (int kk = 0; kk < A[0].size(); kk++)
			{
				
				A[0][kk] = T[A.size() - kk];
			}
		}
		else
		{
			A = transpose(A);
		}
		
		T = A[0];
		T.insert(T.begin(), spiro.begin(), spiro.end());
		spiro = T;
	}

	for (int l = 0; l < spiro.size(); l++)
		cout << spiro[l] << ",";
	return 0;

}
