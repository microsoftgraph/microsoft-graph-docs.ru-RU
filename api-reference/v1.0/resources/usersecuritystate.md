---
title: тип ресурсов userSecurityState
description: Содержит сведения о учетной записи пользователя.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 65aadebaea821fd722b51587e1a504cc008ca7cacb9945a034cb877e2b92b275
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129934"
---
# <a name="usersecuritystate-resource-type"></a>тип ресурсов userSecurityState

Пространство имен: microsoft.graph

Содержит сведения о учетной записи пользователя.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|aadUserId|String|Идентификатор объекта пользователя AAD (GUID) — представляет физическое/многосчетное пользовательское лицо.|
|имя учетной записи|String|Имя учетной записи пользователя (без домена Active Directory или домена DNS) — (также `mailNickName` называемого).|
|domainName|String|Домен учетной записи пользователя NetBIOS/Active Directory (то есть формат домена\учетной записи).|
|emailRole|emailRole|Для оповещений, связанных с электронной почтой, — "роль" учетной записи пользователя. Возможные значения: `unknown`, `sender`, `recipient`.|
|isVpn|Логическое|Указывает, вошел ли пользователь в систему через VPN.|
|logonDateTime|DateTimeOffset|Время, в которое произошел вход. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|logonId|String|ID для регистрации пользователя.|
|logonIp|String|IP-адрес запроса на вход возник из.|
|logonLocation|String|Расположение (по сопоставлению IP-адресов), связанное с событием регистрации пользователя этим пользователем.|
|logonType|logonType|Метод входной записи пользователя. Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|
|onPremisesSecurityIdentifier|String|Идентификатор безопасности Active Directory (локально) пользователя.|
|riskScore|String|Оценка риска учетной записи пользователя сгенерирована/рассчитана с учетной записью поставщика. Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.|
|userAccountType|userAccountSecurityType|Тип учетной записи пользователя (членство в группе) Windows определение. Возможные значения: `unknown`, `standard`, `power`, `administrator`.|
|userPrincipalName|String|Имя регистрации пользователя — интернет-формат: (имя учетной записи пользователя)@(имя доменного имени учетной записи пользователя DNS).|

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

