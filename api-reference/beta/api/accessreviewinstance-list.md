---
title: Список Акцессревиевинстанце
description: Получение объектов Акцессревиевинстанце.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 844564c383b065adc80672cad727807cbb590ca7
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001011"
---
# <a name="list-accessreviewinstance"></a>Список Акцессревиевинстанце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение объектов [акцессревиевинстанце](../resources/accessreviewinstance.md) для определенного [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md). Возвращается список из нуля или более объектов **акцессревиевинстанце** , включая все вложенные свойства. Возвращенные объекты не включают связанные АкцессревиевинстанцедеЦисионитемс. Чтобы получить решения для экземпляра, используйте [List акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem-list.md).

>[!NOTE]
>Если возвращается множество **акцессревиевинстанцес** , чтобы повысить эффективность и избежать истечения времени ожидания, извлеките набор результатов на страницы, включив в него как параметр запроса $Top, который содержит не более 100, и параметр запроса $Skip = 0 в запросе. Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу с помощью свойства @odata. nextLink в ответе, который содержит URL-адрес следующей страницы результатов. При наличии этого свойства Продолжайте делать дополнительные запросы с URL-адресом @odata. nextLink в каждом ответе до тех пор, пока не будут возвращены все результаты, как описано в разделе разбиение данных Microsoft Graph в приложении.
>
>Если не указано ни одного параметра запроса и число результатов превышает 100, Microsoft Graph автоматически разбивать результаты на страницы 100 на каждой странице.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL  |
|Для приложений                            | Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL |

Вошедшего в систему пользователя также должен находиться в роли каталога, который позволяет им читать проверку доступа. Чтобы просмотреть только те экземпляры, для которых пользователь, вошедшего в систему, назначен проверяющему, ознакомьтесь со статьей [Просмотр списка ожидающих доступных экземпляров](accessreviewinstance-pendingaccessreviewinstances.md)

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances
```
## <a name="request-headers"></a>Заголовки запросов
Нет.

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и массив объектов [акцессревиевинстанце](../resources/accessreviewinstance.md) в тексте отклика.

## <a name="examples"></a>Примеры
### <a name="request"></a>Запрос
В приведенном ниже примере показан запрос на получение всех экземпляров проверки доступа для определения.

<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04f34444/instances?$top=100&$skip=0
```

### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "12490cdb-6a18-4c08-ba2c-44442f0a0138",
            "startDateTime": "2020-09-21T20:03:36Z",
            "endDateTime": "2020-09-23T20:03:36Z",
            "status": "NotStarted",
            "scope": {
                "query": "/groups/b7a04444-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        },
        {
            "id": "64444761-b89f-4d9c-afb9-fcfc8bb9cf45",
            "startDateTime": "2020-09-14T20:03:36.74Z",
            "endDateTime": "2020-09-16T20:03:36.74Z",
            "status": "Completed",
            "scope": {
                "query": "/groups/b7a04444-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```

## <a name="see-also"></a>См. также

- [Список Акцессревиевсчедуледефинитион](accessreviewscheduledefinition-list.md)
- [Получение Акцессревиевинстанце](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
