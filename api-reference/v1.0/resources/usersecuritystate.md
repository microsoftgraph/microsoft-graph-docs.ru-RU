# <a name="usersecuritystate-resource-type"></a>тип ресурса userSecurityState

Содержит информацию о состоянии учетной записи пользователя.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|aadUserId|Строка|Идентификатор объекта AAD User  (GUID) — представляет физическую сущность / пользователя с несколькими учетными записями.|
|accountName|Строка|Имя учетной записи пользователя (без домена Active Directory или домена DNS) – (также называемое `mailNickName`).|
|domainName|Строка|Домен учетной записи пользователя NetBIOS/Active Directory (в формате домен\учетная запись).|
|emailRole|emailRole|Для оповещений, связанных с электронной почтой, – «роль» электронной почты пользовательской учетной записи. Возможные значения: `unknown`, `sender`, `recipient`.|
|isVpn|Логический|Указывает, вошел ли пользователь в систему через VPN.|
|logonDateTime|DateTimeOffset|Время входа в программу. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|logonId|Строка|Идентификатор входа пользователя в программу.|
|logonIp|Строка|IP-адрес, с которого поступил запрос на вход в программу.|
|logonLocation|Строка|Местоположение (определяемое по IP-адресу), связанное с событием входа в программу этим пользователем.|
|logonType|logonType|Способ входа пользователя в программу. Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|
|onPremisesSecurityIdentifier|Строка| SID пользователя – локальный идентификатор безопасности в Active Directory.|
|riskScore|Строка|Указанная поставщиком / рассчитанная оценка рисков для учетной записи пользователя. Рекомендуемый диапазон значений: от 0 до 1, что соответствует величине в процентах.|
|userAccountType|userAccountSecurityType|Тип учетной записи (членство в группе), согласно определению, принятому в Windows. Возможные значения: `unknown`, `standard`, `power`, `administrator`.|
|userPrincipalName|Строка|Учетное имя пользователя - формат для Интернета: (имя учетной записи пользователя)@(имя домена DNS учетной записи пользователя).|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
