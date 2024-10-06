# bug-bounty
pursuing a career as a bug bounty? This is the basic command

subfinder -d "domain.com" -silent -all -o output.txt
echo "doamin.com" | subfinder -silent -all -o output.txt

assetfinder --subs-only domain.com > output.txt
echo "domain.com" | assetfinder --subs-only > output.txt

shosubgo -d domain.com -s https://account.shodan.io > output.txt ##berbayar
shosubgo -f urls.txt -s https://account.shodan.io > output.txt

github-subdomain -d domain.com -raw -t token github-subdomain -o output.txt ##berbayar

chaos -d domain.com -silent -key https://cloud.projectdiscovery.io -o output.txt
echo "domain.com" | chaos -silent -key https://cloud.projectdiscovery.io -o output.txt  

echo "domain.com" | gau --subs --fc 200 > output.txt

echo "domain.com" | waybackurls | httpx -silent -mc 200 > output.txt

paramspider -d domain.com

katana -u "domain.com" -o output.txt

echo "https://domain.com" | httpx | hakrawler -u

echo "domain.com" | gau --fc 200 | nuclei -t /home/blue/nuclei-templates/dast/vulnerabilities/ -dast -silent ##mempersingkat waktu scan ketimbang langsung menargetkan subdomainnya

dirsearch -u "https://domain.com" -e php,sql,txt,bak -x 404,501

