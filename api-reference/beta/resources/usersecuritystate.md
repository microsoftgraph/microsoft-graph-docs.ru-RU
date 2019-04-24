---
title: Тип ресурса Усерсекуритистате
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62a54a996d7fe9c892da797cee352a57d0782035
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453604"
---
# <a name="usersecuritystate-resource-type"></a>Тип ресурса Усерсекуритистате

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о состоянии учетной записи пользователя.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|Аадусерид|Строка|Идентификатор объекта пользователя AAD (GUID) — представляет объект пользователя физической или многопользовательской учетной записи.|
|имя_учетной_записи|Строка|Имя учетной записи пользователя (без домена Active Directory или DNS-домена) (также называется `mailNickName`).|
|domainName|Строка|NetBIOS/Active Directory учетной записи пользователя (то есть формат домен \ пользователь).|
|emailRole|emailRole|Для оповещений, связанных с электронной почтой: "роль" — Электронная почта учетной записи пользователя. Возможные значения: `unknown`, `sender`, `recipient`.|
|Исвпн|Boolean|Указывает, вошел ли пользователь в систему через VPN.|
|Логондатетиме|DateTimeOffset|Время возникновения входа. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Логонид|Строка|Идентификатор входа пользователя.|
|logonIp|Строка|IP-адрес, с которого поступил запрос на вход.|
|Логонлокатион|Строка|Расположение (по сопоставлению IP-адресов), связанное с событием входа пользователя этим пользователем.|
|logonType|logonType|Способ входа пользователя в систему. Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|
|onPremisesSecurityIdentifier|String|Идентификатор безопасности (SID) Active Directory (локальный идентификатор) пользователя.|
|riskScore|Строка|Рассчитанный поставщиком и вычисляемый показатель риска учетной записи пользователя. Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.|
|Усераккаунттипе|userAccountSecurityType|Тип учетной записи пользователя (членство в группе), определение Windows. Возможные значения: `unknown`, `standard`, `power`, `administrator`.|
|userPrincipalName|String|Имя пользователя для входа в Интернет: (имя учетной записи пользователя) @ (DNS-имя домена учетной записи пользователя).|

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
<!--
{
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/usersecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
