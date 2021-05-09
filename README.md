# TOHacks-climate-project
#include <iostream>
using namespace std;
int main()
{
	double a;
	double flag = 0;
	double b;
	double flg = 0;
	double c;
	double fl = 0;
	double d;
	double fg = 0;
	cout << "Enter a year in future: ";
	cin >> a;
	while (flag == 0)
	{
		if (a < 2021)
		{
			cout << "Invalid input. Enter a year again: " << endl;
			cin >> a;
		}
		else
		{
			cout << "You entered the year: " << a << endl;
			flag = 1;
		}
	}
	cout << "The temperature rise by the year " << a << " will be approximately: " << 0.012 * (a - 1900) << " degrees celscius as compared to pre inductrial levels." << endl;
	cout << "\nOne of the biggest damages temperature rise can bring about is increasing water levels of seas and oceans." << endl;
	cout << "The water level rise by the year " << a << " will be around: " << (a - 1900) * 0.175 << " centimetres more as compared to pre industrial levels." << endl;
	cout << "\nWe have discussed some basic about global warming. Now, lets try to analyze things which will help minimize its effects." << endl;
	cout << "Enter the number of trees(in billions) that can be planted: ";
	cin >> b;
	while (flg == 0)
	{
		if (b < 0 || b>1000)
		{
			cout << "Enter a number between 0 and 1000." << endl;
			cin >> b;
		}
		else
		{
			cout << "You entered: " << b << endl;
			flg = 1;
		}
	}
	cout << "By planting " << b << " billion trees, climate change can be controlled by: " << (b / 10) << "%" << endl;
	cout << "\nThere is another technique, which can be useful in addressing climate change, which is using renewable energy." << endl;
	cout << "Enter the percentage of energy that you prefer to use renewable energy in your home: ";
	cin >> c;
	while (fl == 0)
	{
		if (c < 0 || c>100)
		{
			cout << "Invalid input. Enter again: ";
			cin >> c;
		}
		else
		{
			cout << "You entered: " << c << endl;
			fl = 1;
		}
	}
	cout << "If " << c << "% of the energy used in your house comes from renewable energy, personal home's contribution to global warming will be reduced by: " << (c * 0.81) << "%"<< endl;
	cout << "\nLastly, another technique that can be used for reducing pollution is to use more public transport instead of private vehicles." << endl;
	cout << "Enter the percentage, what percent of all travel will a person prefer public transport over private transport: ";
	cin >> d;
	while (fg == 0)
	{
		if (fg < 0 || fg>100)
		{
			cout << "Invalid input. Enter a value within 0 and 100: ";
			cin >> d;
		}
		else
		{
			cout << "You entered: " << d << endl;
			fg = 1;
		}
	}
	cout << "If someone uses public transport for " << d << "% of all of their travel, personal travel contribution to global warming will be reduced by: " << (d / 2) << "%" << endl;
	cout << "\nGlobal warming is a very serious issue, which has to be controlled, or else its future effects are very dangerous." << endl;
	system("pause");
	return 0;
}
