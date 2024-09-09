# disk-test
SATA Samsung 870 evo vs WD 850X vs Samsung MZVL2512G

## Samsung MZVL2512G
Command Line: C:\Users\ntjcb\Downloads\DiskSpd\amd64\diskspd.exe -c10M -d30 -r -w40 -t4 -o32 -b4k -Sh -L c:\diskspd\testfile.dat
Input parameters:

        timespan:   1
        -------------
        duration: 30s
        warm up time: 5s
        cool down time: 0s
        measuring latency
        random seed: 0
        path: 'c:\diskspd\testfile.dat'
                think time: 0ms
                burst size: 0
                software cache disabled
                hardware write cache disabled, writethrough on
                performing mix test (read/write ratio: 60/40)
                block size: 4KiB
                using random I/O (alignment: 4KiB)
                number of outstanding I/O operations per thread: 32
                threads per file: 4
                using I/O Completion Ports
                IO priority: normal

System information:

        computer name: Nate-desktop
        start time: 2024/09/09 02:02:42 UTC

        cpu count:              24
        core count:             16
        group count:            1
        node count:             1
        socket count:           1
        heterogeneous cores:    y

        active power scheme:    Balanced (381b4222-f694-41f0-9685-ff5bb260df2e)

Results for timespan 1:
*******************************************************************************

actual test time:       30.01s
thread count:           4


Total IO
thread |       bytes     |     I/Os     |    MiB/s   |  I/O per s |  AvgLat  | LatStdDev |  file
-----------------------------------------------------------------------------------------------------
     0 |     13160480768 |      3213008 |     418.20 |  107060.04 |    0.066 |     0.086 | c:\diskspd\testfile.dat (10MiB)
     1 |     13000613888 |      3173978 |     413.12 |  105759.52 |    0.065 |     0.087 | c:\diskspd\testfile.dat (10MiB)
     2 |     12702928896 |      3101301 |     403.66 |  103337.87 |    0.066 |     0.087 | c:\diskspd\testfile.dat (10MiB)
     3 |     13008027648 |      3175788 |     413.36 |  105819.83 |    0.066 |     0.086 | c:\diskspd\testfile.dat (10MiB)
-----------------------------------------------------------------------------------------------------
total:       51872051200 |     12664075 |    1648.35 |  421977.26 |    0.066 |     0.086

Read IO
thread |       bytes     |     I/Os     |    MiB/s   |  I/O per s |  AvgLat  | LatStdDev |  file
-----------------------------------------------------------------------------------------------------
     0 |      7892606976 |      1926906 |     250.80 |   64206.07 |    0.087 |     0.106 | c:\diskspd\testfile.dat (10MiB)
     1 |      7803854848 |      1905238 |     247.98 |   63484.08 |    0.086 |     0.106 | c:\diskspd\testfile.dat (10MiB)
     2 |      7620038656 |      1860361 |     242.14 |   61988.74 |    0.087 |     0.107 | c:\diskspd\testfile.dat (10MiB)
     3 |      7801057280 |      1904555 |     247.90 |   63461.32 |    0.087 |     0.106 | c:\diskspd\testfile.dat (10MiB)
-----------------------------------------------------------------------------------------------------
total:       31117557760 |      7597060 |     988.83 |  253140.21 |    0.087 |     0.106

Write IO
thread |       bytes     |     I/Os     |    MiB/s   |  I/O per s |  AvgLat  | LatStdDev |  file
-----------------------------------------------------------------------------------------------------
     0 |      5267873792 |      1286102 |     167.40 |   42853.96 |    0.035 |     0.010 | c:\diskspd\testfile.dat (10MiB)
     1 |      5196759040 |      1268740 |     165.14 |   42275.45 |    0.034 |     0.010 | c:\diskspd\testfile.dat (10MiB)
     2 |      5082890240 |      1240940 |     161.52 |   41349.13 |    0.034 |     0.010 | c:\diskspd\testfile.dat (10MiB)
     3 |      5206970368 |      1271233 |     165.46 |   42358.52 |    0.034 |     0.010 | c:\diskspd\testfile.dat (10MiB)
-----------------------------------------------------------------------------------------------------
total:       20754493440 |      5067015 |     659.52 |  168837.05 |    0.034 |     0.010

Total latency distribution:
  %-ile |  Read (ms) | Write (ms) | Total (ms)
----------------------------------------------
    min |      0.024 |      0.017 |      0.017
   25th |      0.058 |      0.028 |      0.036
   50th |      0.068 |      0.033 |      0.056
   75th |      0.092 |      0.039 |      0.074
   90th |      0.149 |      0.046 |      0.116
   95th |      0.178 |      0.050 |      0.158
   99th |      0.219 |      0.058 |      0.205
3-nines |      0.516 |      0.084 |      0.404
4-nines |      3.961 |      0.269 |      3.885
5-nines |      4.273 |      0.875 |      4.209
6-nines |      4.405 |      1.202 |      4.382
7-nines |      4.460 |      1.773 |      4.437
8-nines |      4.460 |      1.773 |      4.460
9-nines |      4.460 |      1.773 |      4.460
    max |      4.460 |      1.773 |      4.460

## WD 850X
Command Line: C:\Users\ntjcb\Downloads\DiskSpd\amd64\diskspd.exe -c10M -d30 -r -w40 -t4 -o32 -b4k -Sh -L e:\diskspd\testfile.dat

Input parameters:

        timespan:   1
        -------------
        duration: 30s
        warm up time: 5s
        cool down time: 0s
        measuring latency
        random seed: 0
        path: 'e:\diskspd\testfile.dat'
                think time: 0ms
                burst size: 0
                software cache disabled
                hardware write cache disabled, writethrough on
                performing mix test (read/write ratio: 60/40)
                block size: 4KiB
                using random I/O (alignment: 4KiB)
                number of outstanding I/O operations per thread: 32
                threads per file: 4
                using I/O Completion Ports
                IO priority: normal

System information:

        computer name: Nate-desktop
        start time: 2024/09/09 02:03:32 UTC

        cpu count:              24
        core count:             16
        group count:            1
        node count:             1
        socket count:           1
        heterogeneous cores:    y

        active power scheme:    Balanced (381b4222-f694-41f0-9685-ff5bb260df2e)

Results for timespan 1:
*******************************************************************************

actual test time:       30.00s
thread count:           4


Total IO
thread |       bytes     |     I/Os     |    MiB/s   |  I/O per s |  AvgLat  | LatStdDev |  file
-----------------------------------------------------------------------------------------------------
     0 |     18190950400 |      4441150 |     578.28 |  148039.26 |    0.122 |     0.080 | e:\diskspd\testfile.dat (10MiB)
     1 |     17971286016 |      4387521 |     571.30 |  146251.62 |    0.122 |     0.080 | e:\diskspd\testfile.dat (10MiB)
     2 |     17717297152 |      4325512 |     563.22 |  144184.64 |    0.123 |     0.080 | e:\diskspd\testfile.dat (10MiB)
     3 |     17896853504 |      4369349 |     568.93 |  145645.88 |    0.123 |     0.080 | e:\diskspd\testfile.dat (10MiB)
-----------------------------------------------------------------------------------------------------
total:       71776387072 |     17523532 |    2281.72 |  584121.40 |    0.122 |     0.080

Read IO
thread |       bytes     |     I/Os     |    MiB/s   |  I/O per s |  AvgLat  | LatStdDev |  file
-----------------------------------------------------------------------------------------------------
     0 |     10908897280 |      2663305 |     346.79 |   88777.39 |    0.163 |     0.077 | e:\diskspd\testfile.dat (10MiB)
     1 |     10788433920 |      2633895 |     342.96 |   87797.05 |    0.164 |     0.077 | e:\diskspd\testfile.dat (10MiB)
     2 |     10627387392 |      2594577 |     337.84 |   86486.44 |    0.165 |     0.077 | e:\diskspd\testfile.dat (10MiB)
     3 |     10738761728 |      2621768 |     341.38 |   87392.81 |    0.164 |     0.077 | e:\diskspd\testfile.dat (10MiB)
-----------------------------------------------------------------------------------------------------
total:       43063480320 |     10513545 |    1368.96 |  350453.70 |    0.164 |     0.077

Write IO
thread |       bytes     |     I/Os     |    MiB/s   |  I/O per s |  AvgLat  | LatStdDev |  file
-----------------------------------------------------------------------------------------------------
     0 |      7282053120 |      1777845 |     231.49 |   59261.87 |    0.060 |     0.027 | e:\diskspd\testfile.dat (10MiB)
     1 |      7182852096 |      1753626 |     228.34 |   58454.57 |    0.060 |     0.027 | e:\diskspd\testfile.dat (10MiB)
     2 |      7089909760 |      1730935 |     225.38 |   57698.20 |    0.061 |     0.027 | e:\diskspd\testfile.dat (10MiB)
     3 |      7158091776 |      1747581 |     227.55 |   58253.07 |    0.061 |     0.027 | e:\diskspd\testfile.dat (10MiB)
-----------------------------------------------------------------------------------------------------
total:       28712906752 |      7009987 |     912.76 |  233667.70 |    0.060 |     0.027

Total latency distribution:
  %-ile |  Read (ms) | Write (ms) | Total (ms)
----------------------------------------------
    min |      0.038 |      0.018 |      0.018
   25th |      0.118 |      0.042 |      0.062
   50th |      0.148 |      0.054 |      0.111
   75th |      0.194 |      0.073 |      0.163
   90th |      0.244 |      0.094 |      0.218
   95th |      0.271 |      0.106 |      0.251
   99th |      0.348 |      0.128 |      0.323
3-nines |      1.077 |      0.304 |      0.869
4-nines |      1.678 |      0.558 |      1.552
5-nines |      3.161 |      0.954 |      3.027
6-nines |      3.413 |      1.196 |      3.389
7-nines |      3.482 |      1.462 |      3.482
8-nines |      3.759 |      1.462 |      3.759
9-nines |      3.759 |      1.462 |      3.759
    max |      3.759 |      1.462 |      3.759


## WD 870 SATA SSD
Command Line: C:\Users\ntjcb\Downloads\DiskSpd\amd64\diskspd.exe -c10M -d30 -r -w40 -t4 -o32 -b4k -Sh -L d:\diskspd\testfile.dat

Input parameters:

        timespan:   1
        -------------
        duration: 30s
        warm up time: 5s
        cool down time: 0s
        measuring latency
        random seed: 0
        path: 'd:\diskspd\testfile.dat'
                think time: 0ms
                burst size: 0
                software cache disabled
                hardware write cache disabled, writethrough on
                performing mix test (read/write ratio: 60/40)
                block size: 4KiB
                using random I/O (alignment: 4KiB)
                number of outstanding I/O operations per thread: 32
                threads per file: 4
                using I/O Completion Ports
                IO priority: normal

System information:

        computer name: Nate-desktop
        start time: 2024/09/09 02:04:32 UTC

        cpu count:              24
        core count:             16
        group count:            1
        node count:             1
        socket count:           1
        heterogeneous cores:    y

        active power scheme:    Balanced (381b4222-f694-41f0-9685-ff5bb260df2e)

Results for timespan 1:
*******************************************************************************

actual test time:       30.01s
thread count:           4


Total IO
thread |       bytes     |     I/Os     |    MiB/s   |  I/O per s |  AvgLat  | LatStdDev |  file
-----------------------------------------------------------------------------------------------------
     0 |      2688827392 |       656452 |      85.44 |   21873.37 |    1.463 |     0.133 | d:\diskspd\testfile.dat (10MiB)
     1 |      2666860544 |       651089 |      84.74 |   21694.67 |    1.473 |     0.166 | d:\diskspd\testfile.dat (10MiB)
     2 |      2687041536 |       656016 |      85.39 |   21858.84 |    1.463 |     0.138 | d:\diskspd\testfile.dat (10MiB)
     3 |      2689904640 |       656715 |      85.48 |   21882.13 |    1.462 |     0.133 | d:\diskspd\testfile.dat (10MiB)
-----------------------------------------------------------------------------------------------------
total:       10732634112 |      2620272 |     341.05 |   87309.02 |    1.465 |     0.143

Read IO
thread |       bytes     |     I/Os     |    MiB/s   |  I/O per s |  AvgLat  | LatStdDev |  file
-----------------------------------------------------------------------------------------------------
     0 |      1614753792 |       394227 |      51.31 |   13135.88 |    1.498 |     0.135 | d:\diskspd\testfile.dat (10MiB)
     1 |      1600901120 |       390845 |      50.87 |   13023.19 |    1.508 |     0.167 | d:\diskspd\testfile.dat (10MiB)
     2 |      1612816384 |       393754 |      51.25 |   13120.12 |    1.499 |     0.139 | d:\diskspd\testfile.dat (10MiB)
     3 |      1613557760 |       393935 |      51.27 |   13126.15 |    1.497 |     0.135 | d:\diskspd\testfile.dat (10MiB)
-----------------------------------------------------------------------------------------------------
total:        6442029056 |      1572761 |     204.71 |   52405.33 |    1.501 |     0.145

Write IO
thread |       bytes     |     I/Os     |    MiB/s   |  I/O per s |  AvgLat  | LatStdDev |  file
-----------------------------------------------------------------------------------------------------
     0 |      1074073600 |       262225 |      34.13 |    8737.49 |    1.409 |     0.112 | d:\diskspd\testfile.dat (10MiB)
     1 |      1065959424 |       260244 |      33.87 |    8671.49 |    1.419 |     0.150 | d:\diskspd\testfile.dat (10MiB)
     2 |      1074225152 |       262262 |      34.14 |    8738.73 |    1.410 |     0.118 | d:\diskspd\testfile.dat (10MiB)
     3 |      1076346880 |       262780 |      34.20 |    8755.99 |    1.409 |     0.111 | d:\diskspd\testfile.dat (10MiB)
-----------------------------------------------------------------------------------------------------
total:        4290605056 |      1047511 |     136.34 |   34903.69 |    1.412 |     0.124

Total latency distribution:
  %-ile |  Read (ms) | Write (ms) | Total (ms)
----------------------------------------------
    min |      0.617 |      0.562 |      0.562
   25th |      1.442 |      1.371 |      1.406
   50th |      1.470 |      1.400 |      1.447
   75th |      1.530 |      1.431 |      1.498
   90th |      1.619 |      1.502 |      1.586
   95th |      1.673 |      1.559 |      1.643
   99th |      1.806 |      1.664 |      1.775
3-nines |      4.417 |      2.606 |      3.845
4-nines |      4.886 |      4.685 |      4.843
5-nines |     10.297 |     10.399 |     10.353
6-nines |     11.049 |     10.919 |     10.975
7-nines |     11.449 |     10.975 |     11.449
8-nines |     11.449 |     10.975 |     11.449
9-nines |     11.449 |     10.975 |     11.449
    max |     11.449 |     10.975 |     11.449
