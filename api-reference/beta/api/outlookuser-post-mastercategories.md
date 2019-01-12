---
title: Создание категории Outlook
description: Создание объекта outlookCategory в основном списке категорий пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e76f6ddc0f733bd2e50b3aac62707acbed370ee3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984705"
---
# <a name="create-outlook-category"></a>Создание категории Outlook

> **Важно**: интерфейсы API в разделе версии /beta в Microsoft Graph в предварительной версии и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Создание объекта [outlookCategory](../resources/outlookcategory.md) в основном списке категорий пользователя.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | MailboxSettings.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | MailboxSettings.ReadWrite   |
|Для приложений | MailboxSettings.ReadWrite |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |


## <a name="request-body"></a>Текст запроса
Включите в текст запроса описание объекта [outlookCategory](../resources/outlookcategory.md) в формате JSON.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код ответа `201 Created` и новый объект [outlookCategory](../resources/outlookcategory.md) в тексте ответа.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
Включите в текст запроса описание объекта [outlookCategory](../resources/outlookcategory.md) в формате JSON.
##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 250

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
