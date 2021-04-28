---
title: Перечисление категорий
description: Список всех категорий, связанных с этим назначением.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d833a566f6406a6ed1132053ad5ecbe83e6058c9
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061646"
---
# <a name="list-categories"></a>Перечисление категорий

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список всех категорий, связанных с этим назначением.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Приложение* | EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite | 

*Разрешения приложения в настоящее время доступны только для частных пользователей предварительного просмотра.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов educationCategory](../resources/educationcategory.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories
```
##### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories added to an assignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->