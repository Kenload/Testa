while true do
    local player = game.Players.LocalPlayer
    local character = player.Character
    local hitbox = character and character:FindFirstChild("Hitbox")
    local tackleHitbox = character and character:FindFirstChild("TackleHitbox")

    if hitbox then
        hitbox.Size = Vector3.new(4, 4 , 6)
        hitbox.Transparency = 1
    else
        warn("Normal Hitbox not found.")
    end

    if tackleHitbox then
        tackleHitbox.Size = Vector3.new(5, 5, 5)
        tackleHitbox.Transparency = 1
    else
        warn("Tackle Hitbox not found.")
    end

    wait(0)
end 
