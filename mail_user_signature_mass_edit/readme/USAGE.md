1. Go to *Settings > Users & Companies > Signature Mass Edits*.
2. Create a new record.
3. Select the company whose internal users must be updated.
4. Optionally select one or more groups to restrict the update to users belonging
   to those groups. Only internal users are updated.
5. Enter the HTML signature template.
6. Click *Confirm*.

The signature template is rendered on the `res.users` model. For example:

```html
<p>
  <strong>{{ object.name }}</strong><br/>
  {{ object.company_id.name }}<br/>
  {{ object.email or '' }}
</p>
```
