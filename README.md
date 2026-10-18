# large-and-small-element-


#include <iostream>
using namespace std;

int main()
{
    int a[5], i, small, large, choice;

    cout << "Enter 5 elements:\n";
    for (i = 0; i < 5; i++)
    {
        cin >> a[i];
    }

    small = large = a[0];

    cout << "1. Smallest element";
    cout << "\n2. Largest element";
    cout << "\nEnter your choice: ";
    cin >> choice;

    switch (choice)
    {
        case 1:
            for (i = 1; i < 5; i++)
            {
                if (a[i] < small)
                    small = a[i];
            }
            cout << "Smallest = " << small;
            break;

        case 2:
            for (i = 1; i < 5; i++)
            {
                if (a[i] > large)
                    large = a[i];
            }
            cout << "Largest = " << large;
            break;

        default:
            cout << "Invalid choice";
    }

    return 0;
}
