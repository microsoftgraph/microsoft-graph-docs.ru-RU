---
title: Обновление userInsightsSettings
description: Обновление свойств объекта userInsightsSettings.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 5f161d5b75e862f358d07fee2347bb3f4d18bbad
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107912"
---
# <a name="update-userinsightssettings"></a>Обновление userInsightsSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновим параметры конфиденциальности [для itemInsights и](../resources/iteminsights.md) [сведения](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) о часах собраний пользователя.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) | User.ReadWrite |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |


## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/settings/itemInsights
PATCH /users/{userId}/settings/itemInsights
```

>**Примечание:** Запросы с `userId` разрешениями User.ReadWrite.All доступны только пользователю или `userPrincipalName` пользователю. Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение|
|:-----------|:------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json. Обязательный.  |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|isEnabled|Boolean| `true` если включены **сведения о элементах itemInsights и** часах собраний; `false` если сведения о **элементах itemInsights и** время собраний отключены. Значение по умолчанию: `true`. Необязательный параметр.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и `200 OK` [объект userInsightsSettings](../resources/userinsightssettings.md) в тексте ответа.

## <a name="example"></a>Пример 

### <a name="request"></a>Запрос

Ниже приводится пример запроса на то, как пользователь обновляет "**isEnabled**" параметр конфиденциальности, чтобы отключить его сведения о элементе и сведения о часах собраний.

<!-- {
  "blockType": "request",
  "name": "update_userInsightsSettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/users/{userId}/settings/itemInsights
Content-type: application/json

{
  "isEnabled": "false"
}
```


### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userInsightsSettings",
  "name": "update_userInsightsSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabled": false,
}
```
