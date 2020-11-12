---
title: Получение Акцессревиевинстанце
description: Получение объекта Акцессревиевинстанце.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b14fe31961524b6aef67d08e683bfecd7a2324c2
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001015"
---
# <a name="get-accessreviewinstance"></a>Получение Акцессревиевинстанце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение объекта [акцессревиевинстанце](../resources/accessreviewinstance.md) с помощью идентификатора акцессревиевинстанце и его родительского [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md). Возвращает все свойства экземпляра, кроме связанного [акцессревиевинстанцедеЦисионитемс](../resources/accessreviewinstancedecisionitem.md).

Чтобы получить решения для экземпляра, используйте [List акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem-list.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL  |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений                            | Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL |

Чтобы вызвать этот API, пользователь, вошедшего в систему, должен быть включен в роль каталога, которая разрешает им читать проверку доступа, или пользователь может быть назначен в качестве проверяющего при проверке доступа.  Более подробную информацию можно узнать в статье требования к ролям и разрешениям для [рецензирования Access](../resources/accessreviewsv2-root.md).

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}
```
## <a name="request-headers"></a>Заголовки запросов
Нет.

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [акцессревиевинстанце](../resources/accessreviewinstance.md) в тексте отклика.

## <a name="examples"></a>Примеры
### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "get_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/12490cdb-6a18-4c08-ba2c-44442f0a0138
```


### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "12490cdb-6a18-4c08-ba2c-44442f0a0138",
    "startDateTime": "2020-09-21T20:03:36Z",
    "endDateTime": "2020-09-23T20:03:36Z",
    "status": "NotStarted",
    "scope": {
        "query": "/groups/b7a4444b-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
}
```

## <a name="see-also"></a>См. также

- [Получение Акцессревиевсчедуледефинитион](accessreviewscheduledefinition-get.md)
- [Список Акцессревиевинстанце](accessreviewinstance-list.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
