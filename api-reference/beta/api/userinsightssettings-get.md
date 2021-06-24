---
title: Get userInsightsSettings
description: Извлечение свойств объекта userInsightsSettings.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 11796934c9ea2edd7a5c3905604671f29604f973
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109214"
---
# <a name="get-userinsightssettings"></a>Get userInsightsSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите настраиваемые пользователем параметры конфиденциальности для [itemInsights](../resources/iteminsights.md) и сведения [о часах собраний.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) | User.Read, User.ReadWrite |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |


## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/settings/itemInsights
GET /user/{userId}/settings/itemInsights
```

>**Примечание:** Запросы с `userId` разрешениями User.ReadWrite.All доступны только пользователю или `userPrincipalName` пользователю. Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект userInsightsSettings](../resources/userinsightssettings.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приводится пример запроса на представление элементов пользователя и параметры времени собраний.

<!-- {
  "blockType": "request",
  "name": "get_userInsightsSettings"
}-->

```http
GET https://graph.microsoft.com/beta/me/settings/itemInsights
```


### <a name="response"></a>Отклик

Ниже приведен пример ответа. 
> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userInsightsSettings",
  "name": "get_userInsightsSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabled": true
}
```


