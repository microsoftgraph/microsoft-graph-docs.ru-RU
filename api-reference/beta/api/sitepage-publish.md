---
author: rahmit
description: Опубликуйте последнюю версию ресурса Ситепаже, которая делает версию страницы доступной для всех пользователей. Если страница извлечена, необходимо вернуть страницу и опубликовать ее. Если страница извлечена в вызывающий объект этого API, страница автоматически возвращается и затем публикуется.
ms.date: 09/10/2018
title: Страница публикации
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 90d08b3f8fae2ed186d1809b4318eec7ef9cf5dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453172"
---
# <a name="sitepage-publish"></a>Ситепаже: публикация

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Опубликуйте последнюю версию ресурса [ситепаже][] , которая делает версию страницы доступной для всех пользователей. Если страница извлечена, необходимо вернуть страницу и опубликовать ее. Если страница извлечена в вызывающий объект этого API, страница автоматически возвращается и затем публикуется.

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All    |
|Для приложений | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a>Тело запроса

У этого сообщения нет текста запроса. Любой Отправленный текст запроса будет игнорироваться.

## <a name="response"></a>Отклик

При успешном выполнении вызова API возвращается отклик `204 No Content`.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!--
{
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish",
  "suppressions": []
}
-->
