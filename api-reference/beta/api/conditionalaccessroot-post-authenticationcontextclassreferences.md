---
title: Создание проверки подлинностиContextClassReference
description: Создание новой проверки подлинностиContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8ad536988d73e8550ec4561f0ca6ead77c40d256
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547458"
---
# <a name="create-authenticationcontextclassreference"></a>Создание проверки подлинностиContextClassReference

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание новой [проверки подлинностиContextClassReference](../resources/authenticationContextClassReference.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)                    |
|:--------------------------------------|:---------------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Policy.ReadWrite.ConditionalAccess |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение                            | Policy.ReadWrite.ConditionalAccess |

> [!NOTE]
> Этот API имеет [известные проблемы, связанные](/graph/known-issues#permissions) с разрешениями.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/authenticationContextClassReferences
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание      |
|:--------------|:-----------------|
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса поставляем представление JSON объекта [authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и новый объект `201 Created` [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
В следующем примере показано создание новой проверки подлинности, которая доступна приложениям для использования.



<!-- {
  "blockType": "request",
  "name": "create_authenticationcontextclassreference"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences
Content-type: application/json

{
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```



#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.authenticationContextClassReference"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/authenticationContextClassReference/$entity",
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
