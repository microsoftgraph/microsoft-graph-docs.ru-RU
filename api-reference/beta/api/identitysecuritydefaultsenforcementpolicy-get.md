---
title: Получение Идентитисекуритидефаултсенфорцементполици
description: Получение свойств и связей объекта идентитисекуритидефаултсенфорцементполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c2ae06cd13c4c9f7401e839d8ac570710ac9e41c
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895990"
---
# <a name="get-identitysecuritydefaultsenforcementpolicy"></a>Получение Идентитисекуритидефаултсенфорцементполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение свойств объекта [идентитисекуритидефаултсенфорцементполици](../resources/identitysecuritydefaultsenforcementpolicy.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Policy.Read.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложения                            | Policy.Read.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметр `select` запроса OData для настройки ответа. Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [идентитисекуритидефаултсенфорцементполици](../resources/identitysecuritydefaultsenforcementpolicy.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_identitysecuritydefaultsenforcementpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/policies/identitySecurityDefaultsEnforcementPolicy
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/identitySecurityDefaultsEnforcementPolicy",
  "description": "Security defaults is a set of basic identity security mechanisms recommended by Microsoft. When enabled, these recommendations will be automatically enforced in your organization. Administrators and users will be better protected from common identity related attacks.",
  "displayName": "Security Defaults",
  "id": "00000000-0000-0000-0000-000000000005",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identitySecurityDefaultsEnforcementPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
