Simple HTTP server

1) Python 3 
python -m http.server 8000
2) Bash
while true;
  do echo -e "HTTP/1.1 200 OK\n\n$(iostat)" \
  | nc -l -k -p 8080 -q 1; 
done
