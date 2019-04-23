---
title: Удаление Трустфрамеворкполици
description: Эта операция удаляет существующий объект Трустфрамеворкполици из клиента Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2583cbf5fd8feee12b18482c515490d2de8ce8be
ms.sourcegitcommit: d264fa064215879fa88a4680402cd57a470d73db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2019
ms.locfileid: "31989403"
---
# <a name="delete-trustframeworkpolicy"></a>Удаление Трустфрамеворкполици

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Удаление существующего [трустфрамеворкполици](../resources/trustframeworkpolicy.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Policy. ReadWrite. Трустфрамеворк|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Для приложений|Не поддерживается.|

Рабочая или учебная учетная запись должна быть глобальным администратором клиента.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---------------|:----------|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

В следующем примере удаляется объект **трустфрамеворкполици**.

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```

##### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
