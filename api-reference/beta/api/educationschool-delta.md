---
title: 'educationSchool: Delta'
description: Получите новые или обновленные учебные заведения, не требующие полного прочтения всей коллекции учебных заведений.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ef31d8cfa9f7b3680c4371e87eb86a46051f75bf
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764776"
---
# <a name="educationschool-delta"></a>educationSchool: Delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите новые или обновленные учебные заведения, не требующие полного прочтения всей коллекции учебных заведений. Дополнительные сведения: [use Query Delta Query](/graph/delta-query-overview) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | EduRoster. ReadBasic, EduRoster. Read или EduRoster. ReadWrite              |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                                           |
| Для приложений                            | EduRoster. ReadBasic. ALL, EduRoster. Read. ALL или EduRoster. Вритеврите. ALL |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /education/schools/{id}/delta
POST /education/me/schools/{id}/delta
POST /education/users/{id}/schools/{id}/delta

```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
| :------------ | :------------ |
| Авторизация | Bearer {code} |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции [educationSchool](../resources/educationschool.md) в тексте отклика.

## <a name="example"></a>Пример

В приведенном ниже примере показано, как вызывать этот API.

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/schools/{id}/delta
```

##### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 313

{
  "value": [
    {
      "principalEmail": "principalEmail-value",
      "principalName": "principalName-value",
      "externalPrincipalId": "externalPrincipalId-value",
      "lowestGrade": "lowestGrade-value",
      "highestGrade": "highestGrade-value",
      "schoolNumber": "schoolNumber-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
