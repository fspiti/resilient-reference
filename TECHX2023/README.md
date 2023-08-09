# IBM MasterSkills September '22: IBM **Security** QRadar SOAR Labs

![screenshot](./logo.png)

***Bo Bleckel & Shane Curtin, App Engineers, IBM **Security** QRadar SOAR***

---

## Lab Guides
 1. [Part I: Building Custom Integrations With the App Host](Lab%20Guides/Part%20I:%20Building%20Custom%20Integrations%20With%20the%20App%20Host/README.md)
 2. [Part II: Advanced Development of Playbooks](Lab%20Guides/Part%20II:%20Advanced%20Development%20of%20Playbooks/README.md)

---

## Lab Assets

* Click [here](./Lab%20Assets/) to access files needed during the lab

---

## Custom Apps

* Click [here](./Custom%20Apps/) to access some custom app.zips that are used

## Tips
- [Lab Guides](#lab-guides)
- [Lab Assets](#lab-assets)
- [Custom Apps](#custom-apps)
- [Tips](#tips)
  - [Copy/Paste in SkyTap Terminal](#copypaste-in-skytap-terminal)
  - [Copy/Paste in SkyTap FireFox Browser](#copypaste-in-skytap-firefox-browser)
  - [Restart SOAR Service](#restart-soar-service)
  - [View SOAR Logs](#view-soar-logs)
  - [Playbook Designer](#playbook-designer)
  - [App Host Commands](#app-host-commands)
### Copy/Paste in SkyTap Terminal

* Copy:
  ```
  CTRL + SHIFT + C
  ```

* Paste:
  ```
  CTRL + SHIFT + V
  ```

### Copy/Paste in SkyTap FireFox Browser

* Copy:
  ```
  CTRL + C
  ```

* Paste:
  ```
  CTRL + V
  ```

### Restart SOAR Service
```
sudo systemctl restart resilient
```

### View SOAR Logs
```
sudo tail -f /usr/share/co3/logs/client.log
```

### Playbook Designer

* Zoom in:
  ```
  CTRL + SHIFT + +
  ```

* Zoom out:
  ```
  CTRL + -
  ```

  > **NOTE** this key mapping worked on MacOS, this may be different on your OS...
### App Host Commands

* Get Deployments:
  ```
  sudo kubectl get deployments -L app.kubernetes.io/instance -A
  ```

* Get Logs:
  ```
  sudo kubectl logs deployment/<deployment_name> -f -n <namespace>
  ```

---