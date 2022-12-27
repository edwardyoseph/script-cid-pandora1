
setBool("Guest Account", true)
addBot("AnjayMabarSlebew", "")

function cekbotonlineoroffline()
    if getBot().status ~= "online" then
        connect()
        sleep(3000)
        while getBot().status ~= "online" do
            connect()
            sleep(3000)
        end
    end
end

cekbotonlineoroffline()
