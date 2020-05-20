---
title: Удаление oAuth2PermissionGrant
description: Удаление объекта oAuth2PermissionGrant, представляющего делегированное предоставление разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: bc36f62d1bb0568fc24b48061e427c404f16e43c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288928"
---
# <a name="delete-a-delegated-permission-grant-oauth2permissiongrant"></a>Удаление делегированного предоставления разрешений (oAuth2PermissionGrant)

Пространство имен: microsoft.graph

Удаление [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).

При удалении делегированного разрешения предоставленный им доступ отзывается. Существующие маркеры доступа продолжат действовать в течение всего времени существования, но новые маркеры доступа не будут предоставлены делегированным разрешениям, определенным в удаленном **oAuth2PermissionGrant**.

> [!NOTE]
> Можно предоставить два делегированных разрешения на авторизацию приложения, действующего от имени пользователя при вызове API. Это может произойти, когда пользователь отправляет приложение по собственному имени (создавая **oAuth2PermissionGrant** с *участником* **консенттипе** , определяя пользователя), а затем администратор предоставляет согласие администратора на уровне клиента от имени всех пользователей (создание второго **oAuth2PermissionGrant** с **консенттипе** *аллпринЦипалс*).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
DELETE /oAuth2Permissiongrants/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2PermissionGrant"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/oauth2PermissionGrants/{id}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
