# <a name="educationstudent-resource-type"></a>Тип ресурса educationStudent

Добавляются дополнительные сведения в файл [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|birthDate|Date| Дата рождения учащегося.|
|externalId|String (строка)| Идентификатор учащегося в исходной системе.|
|gender|educationGender| Возможные значения: `female`, `male`, `other`, `unknownFutureValue`.|
|grade|String (строка)|Текущий уровень оценок учащегося.|
|graduationYear|String (строка)| Год выпуска учащегося.|
|studentNumber|String (строка)| Номер учащегося.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
