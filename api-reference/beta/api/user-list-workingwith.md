---
title: Список workingWith
description: Вычисляемое представление о списке пользователей, с которыми работает пользователь.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 587a9e34db293a738e1242b3d41406bb15990834
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987483"
---
# <a name="list-workingwith"></a>Список workingWith

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вычисляемое представление о списке пользователей, с которыми работает пользователь.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.Read.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User.Read.All |

## <a name="http-request"></a>HTTP-запрос
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
| Заголовок         | Значение                      |
|:---------------|:---------------------------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type   | application/json           |

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код ответа 200 ОК и коллекцию объектов [User](../resources/user.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "id": "id-value",
  "preferredName": "preferredName-value",
  "Email": "Email-value",
}
```
