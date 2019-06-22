```lua 
	local function privateMessage(name, message)
		for _, v in pairs(player.GetAll()) do 
			if string.find(string.lower(v:Name()), string.lower(name)) then 
				v:ChatPrint(('[~] %s : %s'):format(name, message))
			end 
		end 
	end 
```