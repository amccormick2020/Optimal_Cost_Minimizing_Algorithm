# Line_Fitting_Algorithm
Minimizes error by fitting multiple lines of best fit over scatterplot datasets.  

Takes a python dictionary as input with 4 key-value pairs, example instances provided

1st “key” is “n_list”, “value” is a list of m numbers. For i = 0, 1, · · · , m − 1, n_list[i] is the number of points in
the i-th instance (that are to be fitted by lines). (Note that here and in the following, the points will be indexed
by 0, 1, 2, · · · instead of by 1, 2, 3, · · · .)
2nd “key” is “ x_list, “value” is a list of m items. For i = 0, 1, · · · , m − 1, x_list[i] is a list of n_list[i] numbers.
For i = 0, 1, · · · , m − 1 and j = 0, 1, · · · , n_list[i] − 1, x[i][j] is the x-coordinate of the j-th point in the i-th
instance. Here x[i][0] < x[i][1] < x[i][2] < · · · < x[i][n_list[i] − 1].
3rd “key” is “ y_list, “value” is a list of m items. For i = 0, 1, · · · , m − 1, y_list[i] is a list of n_list[i] numbers.
For i = 0, 1, · · · , m − 1 and j = 0, 1, · · · , n_list[i] − 1, y[i][j] is the y-coordinate of the j-th point in the i-th
instance.
4th “key” is C_list, “value” is a list of m numbers. For i = 0, 1, · · · , m−1, C_list[i] is a positive real number, which
is the input parameter C specified in the definition of the “Multi-Line Fitting Problem” for the i-th instance.
(That is, for the i-th instance, C_list[i] is the extra cost for every extra line we use to fit points.)
