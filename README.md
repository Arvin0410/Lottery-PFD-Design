# Lottery-PFD-Design

Ethereum
1. Simple Lottery is nonrecurring, uses blockhashes for random numbers, and has only one winner. Players can buy tickets for 1 ether and a 5 minute duration is added from the start which will prohibits the users from buying when the time has expired. After that, The Deplyoing account can now draw the winner randomly and the winner can now withdraw the prize.
    
2. Recurring Lottery occurs in rounds so that a new prize pool is started every time the old one closes. The same with simple lottery, but on this one, players can buy multiple tickets instead of just one. Users may also check their remaining or current balance. The Deplyoing account can draw a winner every round as well as delete a round after it is complete to clean up old data.

3. RNG Lottery uses a commit-reveal sequence to create a verifiably random number. Every player submits a commitment hash when they buy a ticket. When the ticketing period is over, there is a reveal period during which each player must reveal the secret number used to generate their commitment hash. The secret number is hashed on-chain with the player’s address, and this hash must match the commitment submitted with the ticket. Players who don’t reveal their numbers during the reveal period are dropped from the lottery. The secret numbers are hashed together to generate the random seed for picking a winner.

4. Powerball Lottery requires the player to pick 6 numbers per ticket, they may pick the first 5 numbers from 1-69. The sixth number is a special Powerball number and players may pick from 1-26. Each round also has a time limit which depends on how long the deploying account sets it, after each round drawing is held and the winning ticket consisting of five standard numbers and a Powerball number is picked. Prizes are paid out based on the number of winning numbers matched on your ticket.
