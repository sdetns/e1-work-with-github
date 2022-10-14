# CHEATSHEET

# Übung 1: 
## Matrix Code Snippet
```yaml
strategy:
    matrix:
        os: [ubuntu-latest, macos-latest]
  ```
## Job Abhängigkeiten Snippet 
```yaml
meet:
    # TODO job dependency
    runs-on: ubuntu-latest
    steps:
    - name: Diskutieren
      run: echo "Diskutieren"
    
    # TODO use a github action from the marketplace
      
bye:
    # TODO job dependency
    runs-on: ubuntu-latest
    steps: 
        - name: Say bye
        run: echo "Tschüss"
  ```

## API Call
``` bash
curl --request POST \
  --url https://api.github.com/repos/Matthias-Zax/e1-work-with-github/dispatches \
  --header 'Accept: */*' \
  --header 'Authorization: Bearer >>>YOUR_TOKEN<<<' \
  --data '{"event_type": "hello, I am a Postman Call"}'
  ```
