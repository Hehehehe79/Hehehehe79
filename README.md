EnablePrimaryMouseButtonEvents  (true);
function OnEvent(event,arg)
    if IsKeyLockOn("Capslock")then
        if IsMouseButtonPressed(3)then
            repeat
                if IsMouseButtonPressed(1) then
                    repeat
                        MoveMouseRelative(0,14)
                        Sleep(8)
                    until not IsMouseButtonPressed(1)
                end
            until not IsMouseButtonPressed(0)
        end
    end
end
