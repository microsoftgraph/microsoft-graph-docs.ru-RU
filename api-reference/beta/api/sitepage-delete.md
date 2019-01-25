---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Удаление страницы на сайте SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f855942288556fdf07e2b3af78408976c34eb052
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513027"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a>Удалить страницу в списке страниц сайта узла

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаляет [sitePage][] страниц сайта [списка][] на [сайте][].

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Для удаления элемента, пользователю должно быть предоставлено доступ на запись приложения для удаляемого элемента.

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

Успешно завершена, этот вызов возвращает `204 No Content` уведомление о том, что ресурс был удален и возникла ничего не возвращает.

## <a name="example"></a>Пример

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a>Запрос

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a>Ответ

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
