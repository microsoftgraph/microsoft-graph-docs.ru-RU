---
title: Перечисление agreementAcceptances
description: Извлечение списка объектов agreementAcceptance пользователя.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 12c47f7719f9a5befb31e393a309242d35f984d0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722718"
---
# <a name="list-agreementacceptances"></a>Перечисление agreementAcceptances

Пространство имен: microsoft.graph

Извлечение списка объектов [agreementAcceptance пользователя.](../resources/agreementacceptance.md)
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AgreementAcceptance.Read |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/agreementAcceptances
GET /users/{id | userPrincipalName}/agreementAcceptances
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов agreementAcceptance](../resources/agreementacceptance.md) в тексте ответа.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/agreementAcceptances

GET https://graph.microsoft.com/v1.0/users/f2f4f8e9-c99d-4c73-b990-34f81fbf7fcf/agreementAcceptances
```

### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "093b947f-8363-4979-a47d-4c52b33ee1be",
      "userId": "f2f4f8e9-c99d-4c73-b990-34f81fbf7fcf",
      "agreementFileId": "f2f4f8e9-c99d-4c73-b990-34f81fbf7fcf",
      "recordedDateTime": "2021-03-10T00:39:56.0523527Z",
      "userDisplayName": "Test_User",
      "userPrincipalName": "Test_User@TestTenant.onmicrosoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
