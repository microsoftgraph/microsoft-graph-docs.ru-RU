# <a name="networkconnection-resource-type"></a>Тип ресурса networkConnection

Содержит информацию о состоянии сетевого подключения, связанного с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|applicationName|String|Имя приложения, управляющее сетевым подключением (например, Facebook, SMTP, и т.д.).|
|destinationAddress|String|Конечный IP-адрес (сетевого подключения).|
|destinationDomain|String|Часть домена назначения URL-адреса назначения. (например, "www.contoso.com").|
|destinationPort|String|Порт назначения (сетевого подключения).|
|destinationUrl|String|Строка URL/URI сетевого подключения - исключая параметры. (например, «www.contoso.com/products/default.html»)|
|direction|connectionDirection|Направление сетевого подключения. Возможные значения: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Дата регистрации домена назначения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется часовой пояс UTC). Например, полночь 1 января 2014 года в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`|
|localDnsName|String|Локальное разрешение DNS-имени в том виде, в котором оно отображается в локальном DNS-кэше (например, в случае замены файла "hosts").|
|natDestinationAddress|String|Назначение IP-адреса преобразования сетевых адресов.|
|natDestinationPort|String|Конечный порт преобразования сетевых адресов.|
|natSourceAddress|String|Исходный IP-адрес преобразования сетевых адресов.|
|natSourcePort|String|Исходный порт преобразования сетевых адресов.|
|protocol|[securityNetworkProtocol](securitynetworkprotocol.md)|Сетевой протокол. Возможные значения: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.|
|riskScore|String|Поставщик создал/вычислил оценку риска для сетевого подключения. Рекомендуемый диапазон значений: от 0 до 1, что соответствует величине в процентах.|
|sourceAddress|String|Источник (т.е. исходный объект) IP-адреса (сетевого подключения).|
|SourcePort|String|Источник (т.е. исходный объект) IP-адреса порта (сетевого подключения).|
|status|connectionStatus|Состояние сетевого подключения. Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|String|Параметры (суффикс) URL-адреса назначения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkConnection"
}-->

```json
{
  "applicationName": "String",
  "destinationAddress": "String",
  "destinationDomain": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "@odata.type: microsoft.graph.connectionDirection",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "@odata.type: microsoft.graph.connectionStatus",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->