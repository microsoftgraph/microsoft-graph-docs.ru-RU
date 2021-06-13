---
title: Назначение спискаCategories
description: Извлечение списка объектов категории.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3f7851e746cb87905768604610cd17d036cc963c
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911839"
---
# <a name="list-assignmentcategories"></a>Назначение спискаCategories

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение списка [объектов educationCategory.](../resources/educationcategory.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                                                                         |
| Приложение                            | EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                     |
| :------------ | :------------------------ |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов educationCategory](../resources/educationcategory.md) в тексте ответа.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "sampleKeys": ["4797d052-ebf5-4018-a088-e11adc6b2cbb"],
  "name": "get_class_categories"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/4797d052-ebf5-4018-a088-e11adc6b2cbb/assignmentCategories
```

##### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes('4797d052-ebf5-4018-a088-e11adc6b2cbb')/assignmentCategories",
    "value": [
      {
          "displayName": "Quizzes",
          "id": "f997a279-6bcf-429e-b1d0-d2320c4b84ab"
      },
      {
          "displayName": "Homework",
          "id": "9b8f8f88-ddfc-4aad-9fe9-280513fffc74"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
