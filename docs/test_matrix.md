# Joint test matrix
| # | Activity | Test | Expected | Actual | Pass? | Tester |
|---|---|---|---|---|---|---|
| 1 | 1 | Initial state is safe | SAFE sequence shown | | | |
| 2 | 1 | Valid request P1 | Granted | | | |
| 3 | 1 | Unsafe request | Denied, rolled back | | | |
| 4 | 1 | Wrong token | Auth fails | | | |
| 5 | 1 | Malformed request | Rejected safely | | | |
| 6 | 1 | Client disconnects | Server keeps running | | | |
| 7 | 2 | Real ticket | Accepted | | | |
| 8 | 2 | Edited ticket | Refused | | | |
| 9 | 2 | Old QR image | Refused | | | |
| 10 | 2 | Reused order code | Refused | | | |
| 11 | 2 | Ticket at two gates | DUPLICATE ENTRY alert | | | |
