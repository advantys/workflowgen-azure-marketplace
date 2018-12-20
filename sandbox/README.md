# SandBox

## Image configuration

- Windows Server 2016 Datacenter
- IIS
- SQL Server Express 2016
- WorkflowGen 7.14.3
- WorkflowGen Authentication
- Node js 8.11.3

## Recommended VM Size for Sandbox

| Minimal | Recommended | Optimal |
| --- | --- |---|
| B1S | B2S | B2ms |

## Request a trial licence

Please use this link to request a trial license : https://www.workflowgen.com/en/contact/

## How to connect ?

When your virtual machine is running, WorkflowGen is accessible at `http://[IP_VM]/wfgen`

You can replace IP adress by DNS name.

## Default credentials

**Username** : `wfgen_admin`

**Password** : `Admin123!`

## Configuration to do

### Change WorkflowGen application URL

In WorkflowGen config panel, you need to change `application url` parameter. By default the value is `http://localhost/wfgen`, you need to set `http://[IP_VM]/wfgen`.

For more stability, you can set DNS Name instead of IP adress.

### Configure SMTP

By default IIS is use as SMTP server, in WorkflowGen configuration you can find localhost as SMTP server.

To more efficient you can use Azure SendGrid SMTP, you can find more details in documentation : https://advantys.gitbooks.io/workflowgen-technical-reference-guide/content/azure-integration.html#azure-sendgrid-smtp-configuration