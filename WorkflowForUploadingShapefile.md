##Workflow for Uploading a Shapefile

On upload of a Shapefile, the proposed workflow is:

1. User selects a model from the list of Strabo Content Models (see table below) for their data.
  1. If a Strabo Content Model is not applicable then the user should be able to name their own model. This should be prefixed or suffixed with their user id, or some other way to uniquely name their custom model so it doesn't match one of Strabo model names.
  2. When spots whose "type" property does not match one of the Strabo Content Models is loaded into the app all of the fields on that spot's page will be free text input boxes.
2. After the user selects a Strabo Content Model they should be given the option to map their fields to the fields for the selected Strabo Content Model.

Using a Strabo Content Model comes with the following restrictions:

1. Required fields must be mapped. If not, user needs to create a custom model.
2. If there is a controlled vocabulary for a required field, values in that field must map to the controlled vocabulary terms. If not, user needs to create a custom model.
  1. There is an exception, detailed as follows. Some fields have an option in the vocabulary for "other". In the mobile app if "other" is selected a free text form is made available to the user where the user can define a custom term. On Shapefile upload this "other" option and free text field need to be checked before the server says the content model does not match.
3. If a field does not match a field in the Content Model, or the field matches but the term does not match a field's controlled vocabulary, this field can be included as a custom field within the selected Content Model. Content Models should allow for unlimited custom fields and they should be free text fields. These custom fields, when given to the app as json, should be an object under the element "custom" within "properties".

We currently have 9 Content Models.

| Model Name  | Map Representation  |
|---|---|
| Contact  | point or line  |
| Fault  | point or line  |
| Fold  | point or line  |
| Notes  | point, line or polygon  |
| Orientation  | point  |
| Rock Description  | polygon  |
| Sample Locality  | point  |
| Shear Zone  | point or line  |
| Spot Grouping  | point, line or polygon  |
