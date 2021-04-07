Matthew Allen

Name: ConnectBot

Eval: I looked into the inner workings of the score calculating function, because I figured whatever happened, I'd definitely be using the original score. I then drew some graphs and scenarios on paper and decided the best approach would be to encapsulate two in a row sequences into the final scores. So, I made all two in a rows worth one point each and figured that the error range that would be causes by non-open-ended two in a rows would be mostly insignificant.

The test cases in test_boards.py are meant to run through mostly the algorithms that would take forever with larger boards (like default minimax). I usually prefer to manually test everything else by playing games and having friends play games against the AI.

The eval function is definitely NOT O(1), because I was extremely confused as to how that would be possible, especially since looking through the board would require loops anyway. Also, I reused my basic minimax algorithm and adjusted it for each scenario numerous times. I also used some interior helper functions that I created so I could keep everything mostly recursive and pass parameters correctly.