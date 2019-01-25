---
title: Создание outlookTaskFolder
description: Создайте папку задачи в группе задач по умолчанию (`My Tasks`) из почтового ящика пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 81c77d96b4d7c66cfbc7dde3481a7bfaa8cd6c5f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514448"
---
# <a name="create-outlooktaskfolder"></a>Создание outlookTaskFolder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте папку задачи в группе задач по умолчанию (`My Tasks`) из почтового ящика пользователя.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Tasks.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Tasks.ReadWrite    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders

```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите представление JSON объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) .

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `201 Created` объект [outlookTaskFolder](../resources/outlooktaskfolder.md) и кода ответа в теле ответа.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В следующем примере создается задача папку с именем кого в группе задач по умолчанию (`My Tasks`) из почтового ящика пользователя.
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskfolders 
Content-type: application/json
Content-length: 60

{
  "name": "Volunteer"
}
```
В тексте запроса укажите представление JSON объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) .
##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGig==",
  "isDefaultFolder": false,
  "name": "Volunteer",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
