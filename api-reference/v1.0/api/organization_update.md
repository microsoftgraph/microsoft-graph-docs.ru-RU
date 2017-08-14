# <a name="update-organization"></a>Обновление организации

Обновите свойства организации, которая прошла проверку подлинности.
## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных **областей**:
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /organization

```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedPlans|AssignedPlan|Коллекция планов обслуживания, сопоставленных с клиентом.                            **Примечание.** Значение null не допускается.            |
|city|String|            |
|companyLastDirSyncTime|DateTimeOffset|Время и дата последней синхронизации клиента с локальным каталогом.|
|country|String|            |
|countryLetterCode|String|            |
|deletionTimestamp|DateTimeOffset||
|dirSyncEnabled|Boolean|Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию).|
|displayName|String|Отображаемое имя для клиента.|
|marketingNotificationEmails|String|                                        **Примечание.** Значение null не допускается.            |
|objectType|String|Строка, которая определяет тип объекта. Для клиентов всегда задается значение Company. Наследуется от [directoryObject](../resources/directoryobject.md).|
|postalCode|String|            |
|preferredLanguage|String|            |
|provisionedPlans|ProvisionedPlan|                                        **Примечание.** Значение null не допускается.            |
|provisioningErrors|ProvisioningError|                                        **Примечание.** Значение null не допускается.            |
|securityComplianceNotificationMails|String||
|securityComplianceNotificationPhones|String||
|state|String|            |
|street|String|            |
|technicalNotificationMails|String|                                        **Примечание.** Значение null не допускается.            |
|telephoneNumber|String|            |
|verifiedDomains|VerifiedDomain|Коллекция доменов, сопоставленных с этим клиентом.                            **Примечание.** Значение null не допускается.            |

## <a name="response"></a>Отклик

В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [organization](../resources/organization.md) в теле отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/organization
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
