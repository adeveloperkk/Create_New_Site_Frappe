# Frappe 

Create a New ERPNext Site in existing
A site is required to run ERPNext.
```bash
bench new-site mpdrealteck
```
```bash
bench get-app --branch main https://github.com/frappe/crm
bench get-app --branch version-15 erpnext
```

Install ERPNext on the Site
```bash
bench --site mpdrealteck install-app crm
bench --site mpdrealteck install-app erpnext
```
```bash
bench --site mpdrealteck enable-scheduler
```
Disable Maintenance Mode:
```bash
bench --site mpdrealteck  set-maintenance-mode off
```


```bash
sudo bench setup add-domain --site mpdrealteck tools.mpdrealteck.com
```
```bash
sudo -H bench setup lets-encrypt mpdrealteck --custom-domain tools.mpdrealteck.com


```
Replace bench with this if shows error
/home/developerkk/.local/bin/bench 

skip below if possible
```bash
bench config dns_multitenant on(skip if possible)
```

```bash
sudo -H bench setup lets-encrypt mpdrealteck --custom-domain tools.mpdrealteck.com

```
