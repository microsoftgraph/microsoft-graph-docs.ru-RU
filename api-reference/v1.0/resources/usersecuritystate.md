---
title: Тип ресурса userSecurityState
description: Содержит информацию о состояниях об учетной записи пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9f451f2bc42500eee15bd59809c124a79186916f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27992058"
---
# <a name="usersecuritystate-resource-type"></a>Тип ресурса userSecurityState

Содержит информацию о состояниях об учетной записи пользователя.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|aadUserId|String|AAD пользователя объекта идентификатор (GUID) — представляет удостоверение пользователя физических/несколькими-account.|
|Имя учетной записи|String|Имя учетной записи для учетной записи пользователя (без домена Active Directory и DNS домена) - (также называемая `mailNickName`).|
|domainName|String|NetBIOS/Active Directory в домен учетной записи пользователя (то есть, в формате домен\учетная запись).|
|emailRole|emailRole|Связанные с электронной почты оповещений,-электронной почты для учетной записи пользователя «роли». Возможные значения: `unknown`, `sender`, `recipient`.|
|isVpn|Boolean|Указывает, вошел ли пользователь через VPN.|
|logonDateTime|DateTimeOffset|Время входа в программу. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|logonId|String|Идентификатор пользователя входа.|
|logonIp|String|IP-адрес, запрос на вход исходит от.|
|logonLocation|String|Расположение (по сопоставления IP-адреса), связанных с событие вход пользователя с этим пользователем.|
|logonType|logonType|Метод входа пользователя. Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|
|onPremisesSecurityIdentifier|String|Active Directory (локально) идентификатор безопасности (SID) пользователя.|
|riskScore|String|Оценка риска поставщика создается/вычисляемые учетной записи пользователя. Рекомендуемое значение диапазона 0-1, который соответствует в процентах.|
|userAccountType|userAccountSecurityType|Тип учетной записи (членство в группе) для определения Windows. Возможные значения: `unknown`, `standard`, `power`, `administrator`.|
|userPrincipalName|String|Учетное имя пользователя - формат для Интернета: (имя учетной записи пользователя) @(имя домена DNS учетной записи пользователя).|

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
