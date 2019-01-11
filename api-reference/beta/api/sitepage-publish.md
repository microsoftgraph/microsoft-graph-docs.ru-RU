---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Страница публикации
localization_priority: Normal
ms.openlocfilehash: 0b98f22dda2c4b08d04150b8b24126fdff5ca505
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836157"
---
# <a name="sitepage-publish"></a>sitePage: публикация

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Публикация последней версии ресурсов [sitePage][] , предоставляющего версии страницы для всех пользователей. Если страница извлечена, вернуть ее и опубликовать его. Если страница извлечена вызывающему этот интерфейс API, страница автоматически вернули и последующей публикацией.

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

Это сообщение не имеет текста запроса. Любой текст запроса отправляются будет игнорироваться.

## <a name="response"></a>Отклик

При успешном выполнении вызова API возвращается отклик `204 No Content`.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish"
} -->
