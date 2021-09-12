---
title: тип ресурса hostSecurityState
description: Содержит сведения о хосте (включая устройства, компьютеры и т. п.).
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3513342aaadb2eaf80a787b26988ff2a638813ac
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59007210"
---
# <a name="hostsecuritystate-resource-type"></a>тип ресурса hostSecurityState

Пространство имен: microsoft.graph

Содержит сведения о хосте (включая устройства, компьютеры и т. п.).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|fqdn|Строка|Host FQDN (полное доменное имя) (например, `machine.company.com` ).|
|isAzureAadJoined|Логический|True, если хост является доменом, присоединимым к Azure Active Directory Службы домена.|
|isAzureAadRegistered|Логический|True, если хост зарегистрирован Azure Active Directory устройств (устройства BYOD — то есть не полностью управляемые предприятием).|
|isHybridAzureDomainJoined|Логический|True, если хост является доменом, присоединимым к локальному домену Active Directory.|
|netBiosName|Строка|Имя локального хоста без доменного имени DNS.|
|os|String|Операционная система host. (Например, Windows10, MacOS, RHEL и т.д.).|
|privateIpAddress|Строка|Частный (не маршрутируемый) адрес IPv4 или IPv6 (см. [RFC 1918)](https://tools.ietf.org/html/rfc1918)во время оповещения.|
|publicIpAddress|Строка|Общедоступный адрес IPv4 или IPv6 (см. [RFC 1918)](https://tools.ietf.org/html/rfc1918)во время оповещения.|
|riskScore|Строка|Оценка риска, сгенерированная поставщиком и рассчитанная на хост.  Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.|

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

