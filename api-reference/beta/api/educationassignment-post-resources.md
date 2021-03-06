---
title: Создание Едукатионассигнментресаурце
description: OData. Type, указывающая тип создаваемого ресурса. Обратите внимание, что файловые ресурсы сначала необходимо отправить в **ресаурцефолдер**назначений.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1e432d4521ffe871de75be4ae8764953d99a3abc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002557"
---
# <a name="create-educationassignmentresource"></a>Создание Едукатионассигнментресаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте [ресурс назначения](../resources/educationassignmentresource.md). В самом ресурсе есть @odata. Type, указывающий тип создаваемого ресурса. Обратите внимание, что файловые ресурсы сначала необходимо отправить в **ресаурцефолдер**назначений.

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
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в формате JSON.


## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "ignored",
  "name": "create_educationassignmentresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources
Content-type: application/json
Content-length: 212

{
  "distributeForStudentWork": "false",
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "#microsoft.education.assignments.api.educationLinkResource"
  }
}

```
В тексте запроса добавьте представление объекта [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в формате JSON.
##### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 229

{
  "id": "122333",
  "distributeForStudentWork": false,
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "#microsoft.education.assignments.api.educationLinkResource"
  }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


