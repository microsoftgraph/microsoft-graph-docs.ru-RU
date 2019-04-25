---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Удаление страницы с сайта SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f855942288556fdf07e2b3af78408976c34eb052
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537135"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a>Удаление страницы из списка страниц сайта

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаляет объект [ситепаже][] из [списка][] страниц сайта на [сайте][].

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[сайта]: ../resources/site.md

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Чтобы удалить элемент, пользователь должен получить доступ к приложению на запись для элемента, который требуется удалить.

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя       | Значение | Описание
|:-----------|:------|:--------------------------------------------------------
| _if-match_ | etag  | Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a>Ответ

В случае успешного выполнения этот вызов возвращает `204 No Content` ответ, указывающий на то, что ресурс был удален и что не было возвращено.

## <a name="example"></a>Пример

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a>Запрос

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a>Отклик

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete",
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
