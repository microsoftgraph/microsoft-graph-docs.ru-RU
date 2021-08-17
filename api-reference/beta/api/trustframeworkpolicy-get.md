---
title: Get trustFrameworkPolicy
description: Эта операция извлекает существующий контент trustFrameworkPolicy из клиента Azure AD B2C.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a536f0a1da21b0e56ce1c7cb5a8b37fd97569769a22c99f02c6d5efafb3157c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139728"
---
# <a name="get-trustframeworkpolicy"></a>Get trustFrameworkPolicy

Пространство имен: microsoft.graph

>**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Извлечение содержимого существующего [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| Policy.Read.All, Policy.ReadWrite.TrustFramework|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение|Policy.Read.All, Policy.ReadWrite.TrustFramework|

Рабочая или учебная учетная запись должна быть глобальным администратором клиента.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/{id}/$value
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select` и `$expand` для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---------------|:----------|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` XML-представление [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) в тексте ответа.  

>**Примечание:** тип контента ответа будет `application/xml` .

## <a name="example"></a>Пример

В следующем примере извлекается определенное **довериеFrameworkPolicy**.

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored",
  "name": "get_trustFramework"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_Test/$value
```

##### <a name="response"></a>Отклик

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_Test" PublicPolicyUri="http://tenantName.onmicrosoft.com/B2C_1A_Test">
    .....
    ....
    <!---PolicyContent-->
    ....
    ....
</TrustFrameworkPolicy>
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get trustFramework policy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


