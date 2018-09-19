# <a name="hostsecuritystate-resource-type"></a>тип ресурса hostSecurityState

Содержит сведения о состоянии узла (в том числе устройств, компьютеров и т.п.).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|fqdn|Строка|FQDN  (полное доменное имя) узла (например, `machine.company.com`).|
|isAzureAadJoined|Логический|Имеет значение true, если узел является доменом в составе доменных служб Active Directory Azure.|
|isAzureAadRegistered|Логический|Имеет значение true, если узел зарегистрирован в регистрации устройств Azure Active Directory (BYOD-устройства - то есть устройства, не полностью управляемые предприятием).|
|isHybridAzureDomainJoined|Логический|Имеет значение true, если узел входит в локальный домен Active Directory.|
|netBiosName|Строка|Имя локального узла без доменного имени DNS.|
|os|Строка|Операционная система узла. (Например, Windows10, MacOS, RHEL, и т.д.).|
|privateIpAddress|Строка|Частный (немаршрутизируемыц) адрес IPv4 или IPv6 (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) на момент оповещения.|
|publicIpAddress|Строка|Общедоступный маршрутизируемый адрес IPv4 или IPv6 (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) на момент оповещения.|
|riskScore|Строка|Выполняемая поставщиком / рассчитываемая оценка рисков для узла.  Рекомендуемый диапазон значений: от 0 до 1, что соответствует величине в процентах.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
