---
title: Добавление Едукатионкатегориес
description: Добавление существующего Едукатионкатегори к этому educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0f5a536ba1dc6390d8642f82de2d4bf131602c62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007898"
---
# <a name="add-educationcategories"></a>Добавление Едукатионкатегориес

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавьте один или несколько существующих объектов [едукатионкатегори](../resources/educationcategory.md) в этот [educationAssignment](../resources/educationassignment.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  EduAssignments. Реадвритебасик, EduAssignments. ReadWrite  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Для приложений | Не поддерживается.  | 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите odata.id существующих объектов [едукатионкатегори](../resources/educationcategory.md) , которые требуется добавить к этому назначению.


## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/$ref
Content-type: application/json
Content-length: 212

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/classes/11021/assignmentCategories/ec98f158-341d-4fea-9f8c-14a250d489ac"
}

```
В тексте запроса укажите odata.id существующего объекта [едукатионкатегори](../resources/educationcategory.md) , который требуется добавить к этому назначению.
##### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add educationCategory to educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


