# onjoin.sk-
skrypt minecraft / serwer / onjoin


on join:
    set join message to "&9%player% &6Dolaczyl do gry!"
	give to player 10 apple
	send "Nagroda za wejscie na serwer!"
on quit:
    set leave to message to "&9%player% &6Wyszedl z gry!"
	
on join:
    if player has permission "vip.dolacz":
	set join message to "&b[VIP] &9%player% &6Doloczyl do gry!"
	give player 1 diamond
	send "&cDziekujemy za zakup VIP'a , w nagrode otrzymales 1 diamenta"
	give 5 apple to all players 
	send "&aGracz &c%player% &adolaczyl w trybie VIP'a i otrzymales darmowe jablko!"
