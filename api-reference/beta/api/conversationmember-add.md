---
title: Добавление Конверсатионмембер
description: Добавление Конверсатионмембер к каналу.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd1f2c6689176422fa35a500224c6f2a5f277851
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36634053"
---
# <a name="add-conversationmember"></a>Добавление Конверсатионмембер

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавление [конверсатионмембер](../resources/conversationmember.md) к каналу [](../resources/channel.md).

> [!NOTE]
>Эта операция поддерживается только для каналов с [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) `private`. Вызовы с любыми другими [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) будут возвращать ответ о неправильном запросе 400.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|---------|-------------|
|Делегированные (рабочая или учебная учетная запись)|Group.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Для приложений|Group.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

Включите в запрос указанные ниже свойства.

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|roles|string collection|Роли для этого пользователя.|
|user|[user](../resources/user.md)|Пользователь, добавляемый в канал.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [конверсатионмембер](../resources/conversationmember.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member"
} -->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/
content-type: application/json
content-length: 26

{
  "@odata.type": "microsoft.graph.aadConversationMember",
  "roles": [],
  "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 468

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
