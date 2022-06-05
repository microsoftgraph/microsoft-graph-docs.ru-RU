---
title: Тип ресурса hostSecurityState
description: Содержит сведения о узле с отслеживанием состояния (включая устройства, компьютеры и т. д.).
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ade1d89ee392eae5fe30cab8f85329c285e3590d
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898940"
---
# <a name="hostsecuritystate-resource-type"></a>Тип ресурса hostSecurityState

Пространство имен: microsoft.graph

Содержит сведения о узле с отслеживанием состояния (включая устройства, компьютеры и т. д.).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|Полное доменное имя|Строка|Полное доменное имя узла (полное доменное имя) (например, `machine.company.com`).|
|isAzureAadJoined|Boolean|Значение true, если хост присоединен к домену доменных служб Azure Active Directory.|
|isAzureAadRegistered|Boolean|Значение true, если хост зарегистрирован с помощью регистрации устройств Azure Active Directory (устройства BYOD, то есть не полностью управляемые предприятием).|
|isHybridAzureDomainJoined|Boolean|Значение true, если хост присоединен к локальному домену Active Directory.|
|netBiosName|Строка|Имя локального узла без доменного имени DNS.|
|os|Строка|Операционная система узла. (Например, Windows10, MacOS, RHEL и т. д.).|
|privateIpAddress|Строка|Частный (не маршрутизируемый) IPv4-адрес или IPv6-адрес (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) во время оповещения.|
|publicIpAddress|Строка|Общедоступный маршрутизируемый IPv4-адрес или IPv6-адрес (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) во время оповещения.|
|riskScore|Строка|Созданная поставщиком или вычисляемая оценка риска узла.  Рекомендуемый диапазон значений — 0–1, что соответствует проценту.|

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

