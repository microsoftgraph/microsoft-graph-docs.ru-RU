---
title: тип ресурса hostSecurityState
description: Содержит сведения о хосте (включая устройства, компьютеры и т. п.).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 20de01e91abbc2e3cf568a8898b79680e73188e549ffd306abf4f7aed092b16b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54184895"
---
# <a name="hostsecuritystate-resource-type"></a>тип ресурса hostSecurityState

Пространство имен: microsoft.graph

Содержит сведения о хосте (включая устройства, компьютеры и т. п.).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|fqdn|String|Host FQDN (полное доменное имя) (например, `machine.company.com` ).|
|isAzureAadJoined|Логическое|True, если хост является доменом, присоединимым к Azure Active Directory Службы домена.|
|isAzureAadRegistered|Логическое|True, если хост зарегистрирован Azure Active Directory устройств (устройства BYOD — то есть не полностью управляемые предприятием).|
|isHybridAzureDomainJoined|Логическое|True, если хост является доменом, присоединимым к локальному домену Active Directory.|
|netBiosName|String|Имя локального хоста без доменного имени DNS.|
|os|String|Операционная система host. (Например, Windows10, MacOS, RHEL и т.д.).|
|privateIpAddress|String|Частный (не маршрутируемый) адрес IPv4 или IPv6 (см. [RFC 1918)](https://tools.ietf.org/html/rfc1918)во время оповещения.|
|publicIpAddress|String|Общедоступный адрес IPv4 или IPv6 (см. [RFC 1918)](https://tools.ietf.org/html/rfc1918)во время оповещения.|
|riskScore|String|Оценка риска, сгенерированная поставщиком и рассчитанная на хост.  Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.|

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

