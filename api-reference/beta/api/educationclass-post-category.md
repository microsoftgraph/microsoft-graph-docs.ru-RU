---
title: Создание educationCategory
description: Создает новую категорию.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bf0fb3c2459fba0c309e37149e0f87013ff12449
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911776"
---
# <a name="create-educationcategory"></a>Создание educationCategory

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создает новое [educationCategory](../resources/educationcategory.md) для [класса educationClass.](../resources/educationclass.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Для приложений | Не поддерживается. | 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories

```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляют представление JSON объекта [educationCategory.](../resources/educationcategory.md)


## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект educationCategory](../resources/educationcategory.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "sampleKeys": ["9a5e4047-c1dc-4243-9628-580d3c64b80c"],
  "name": "create_educationcategory_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/9a5e4047-c1dc-4243-9628-580d3c64b80c/assignmentCategories
Content-type: application/json
Content-length: 33

{ 
  "displayName": "Quizzes"
}
```
В теле запроса поставляют представление JSON объекта [educationCategory.](../resources/educationcategory.md)

##### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 85

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('9a5e4047-c1dc-4243-9628-580d3c64b80c')/assignmentCategories/$entity",
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


