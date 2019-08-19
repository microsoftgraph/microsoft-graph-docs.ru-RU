---
title: Список Акцессревиевс
description: Получение объектов Акцессревиев для Бусинессфловтемплате.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46c9abdbc0a1d5dca4c4e61d423b23ed31691384
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462704"
---
# <a name="list-accessreviews"></a>Список Акцессревиевс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение объектов [акцессревиев](../resources/accessreview.md) для определенного [бусинессфловтемплате](../resources/businessflowtemplate.md). Список из нуля или более объектов **акцессревиев** возвращается для каждой одноразовой и повторяющейся проверки доступа, созданной с помощью этого шаблона бизнес-процесса.

>[!NOTE]
> Если какой-либо из проверок доступа, соответствующих фильтру, является повторяющейся проверкой доступа, возвращается один объект **акцессревиев** для представления каждого повторяющегося ряда в целом. Например, если имеется ежемесячная проверка доступа участников группы "гость", то есть Ежеквартальная проверка доступа участников группы "гость" для группы "б" и одноразовый доступ к просмотру гостевых участников группы C и вызывающим запросом на рецензию доступа с бизнес-процессом шаблон рецензирования участников группы, будут возвращены три объекта. Чтобы получить экземпляры повторяющейся проверки доступа или экземпляра проверки доступа, запланированный на определенный месяц или квартал, вызывающий может впоследствии перемещаться по связи **экземпляра** объекта повторяющегося объекта **акцессревиев** . Связь **экземпляра** связывается с объектами **акцессревиев** для текущего или прошлых экземпляров проверки поповторяющегося доступа.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership |

 Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [акцессревиев](../resources/accessreview.md) в тексте отклика.

## <a name="examples"></a>Примеры
##### <a name="request"></a>Запрос
В приведенном ниже примере показан запрос на получение всех одноразовых и повторяющихся проверок доступа для шаблона рабочего процесса "6E4F3D20-C5C3-407F-9695-8460952BCC68".

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6E4F3D20-C5C3-407F-9695-8460952BCC68'
```


---


##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
       {
         "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
         "displayName": "review",
         "startDateTime": "2017-11-14T01:14:54.89Z",
         "endDateTime": "2017-12-14T01:14:54.89Z",
         "status": "InProgress",
         "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
         "reviewerType": "self",
         "description": "",
         "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"}
       }
    ]
}
```

## <a name="see-also"></a>См. также

- [Получение Акцессревиев](accessreview-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviews",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
