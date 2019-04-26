---
title: Тип ресурса Хостсекуритистате
description: Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).
localization_priority: Normal
ms.openlocfilehash: 0646547b7f3e31dcf283c1ce423a52b4ae16f013
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570787"
---
# <a name="hostsecuritystate-resource-type"></a>Тип ресурса Хостсекуритистате

Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|полным|String|ПОЛНОЕ доменное имя узла (полное доменное имя) ( `machine.company.com`например,).|
|Исазуреааджоинед|Boolean|True, если узел подключен к доменным службам Azure Active Directory.|
|Исазуреаадрегистеред|Boolean|True, если узел зарегистрирован с регистрацией устройств Azure Active Directory (BYOD Devices — то есть, не полностью управляется предприятием).|
|Ишибридазуредомаинжоинед|Boolean|True, если узел является доменом, присоединенным к локальному домену Active Directory.|
|Нетбиоснаме|String|Имя локального узла без DNS-имени домена.|
|совместим|String|Хост операционной системы. (Например, Windows10, MacOS, РХЕЛ и т. д.).|
|Приватеипаддресс|String|Частный (без маршрутизации) IPv4-или IPv6-адрес (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) на момент оповещения.|
|ПублиЦипаддресс|String|IPv4-или IPv6-адрес общеДоступной маршрутизации (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) во время оповещения.|
|riskScore|String|Полученный поставщиком и вычисляемый показатель риска для узла.  Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.|

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
