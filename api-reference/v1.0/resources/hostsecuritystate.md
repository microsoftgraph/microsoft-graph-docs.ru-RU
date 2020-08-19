---
title: Тип ресурса Хостсекуритистате
description: Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e358280e1c510a763a8fa38febce060448491270
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806088"
---
# <a name="hostsecuritystate-resource-type"></a>Тип ресурса Хостсекуритистате

Пространство имен: microsoft.graph

Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|полным|String|ПОЛНОЕ доменное имя узла (полное доменное имя) (например, `machine.company.com` ).|
|исазуреааджоинед|Логический|True, если узел подключен к доменным службам Azure Active Directory.|
|исазуреаадрегистеред|Логический|True, если узел зарегистрирован с регистрацией устройств Azure Active Directory (BYOD Devices — то есть, не полностью управляется предприятием).|
|ишибридазуредомаинжоинед|Логический|True, если узел является доменом, присоединенным к локальному домену Active Directory.|
|нетбиоснаме|String|Имя локального узла без DNS-имени домена.|
|совместим|String|Хост операционной системы. (Например, Windows10, MacOS, РХЕЛ и т. д.).|
|приватеипаддресс|String|Частный (без маршрутизации) IPv4-или IPv6-адрес (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) на момент оповещения.|
|публиЦипаддресс|String|IPv4-или IPv6-адрес общедоступной маршрутизации (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) во время оповещения.|
|riskScore|String|Полученный поставщиком и вычисляемый показатель риска для узла.  Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.|

## <a name="json-representation"></a>Представление в формате JSON

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
