---
title: Создание accessReview
description: В Azure AD доступа к функции проверки, создайте новый объект accessReview.
localization_priority: Normal
ms.openlocfilehash: 1ee5ce696f1d71c57adf9e6c5ee30c067536c8ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851445"
---
# <a name="create-accessreview"></a>Создание accessReview

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD создайте новый объект [accessReview](../resources/accessreview.md) .

До внесения этого запроса, вызывающий должен иметь ранее [извлекается список бизнес-поток шаблонов](businessflowtemplate-list.md), иметь значение `businessFlowTemplateId` необходимо включить в запрос.

После выполнения этого запроса, вызывающего следует [Создать programControl](programcontrol-create.md), чтобы связать с программой проверки доступа.  

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.All, а также должны иметь ProgramControl.ReadWrite.All для выполнения сценария с последующих вызовов для создания programControl |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носителя \{маркеров\}. Обязательный. |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите представление JSON объекта [accessReview](../resources/accessreview.md) .

В следующей таблице показаны свойства, которые необходимы для создания accessReview.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | Имя проверки доступа.  |
| `startDateTime`           |`DateTimeOffset`                                                | Дата и время при планировании проверки быть запуск.  Это должно быть даты в будущем.   |
| `endDateTime`             |`DateTimeOffset`                                                | Дата и время после запланированного окончания проверки. Это должно быть более поздней, чем дата начала по крайней мере один день.   |
| `description`             |`String`                                                        | Описание, чтобы показать рецензентов. |
| `businessFlowTemplateId`  |`String`                                                        | Business поток идентификатор шаблона, полученный из [businessFlowTemplate](../resources/businessflowtemplate.md).  |
| `reviewerType`            |`String`                                                        | Тип отношения рецензент права доступа проверенные объекта, один из `self`, `delegate` или `entityOwners`. | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | Объект, для которого создается проверки доступа, такие как члены группы или назначения пользователей для приложения. | 


Если значение равно reviewerType, указанное `delegate`, а затем вызывающий объект должен также включать `reviewers` свойство с семейством [удостоверению пользователя](../resources/useridentity.md) рецензентов.

Кроме того вызывающего может включать параметры для создания серии повторяющихся review или для изменения поведения проверки по умолчанию. В частности, для создания повторяющихся review вызывающего необходимо включить `accessReviewRecurrenceSettings` в access Проверьте параметры,


## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `201, Created` код ответа и объект [accessReview](../resources/accessreview.md) в теле ответа.

## <a name="example"></a>Пример

Это пример создания одноразовый (не повторяющееся) доступа проверки, явно указание двух пользователей в качестве рецензентов.

##### <a name="request"></a>Запрос
В тексте запроса укажите представление объекта [accessReview](../resources/accessreview.md) с JSON.

<!-- {
  "blockType": "request",
  "name": "create_accessReview_from_accessReviews"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
    "displayName":"TestReview",
    "startDateTime":"2017-02-10T00:35:53.214Z",
    "endDateTime":"2017-03-12T00:35:53.214Z",
    "reviewedEntity": {
        "id": "99025615-a0b1-47ec-9117-35377b10998b",
    },
    "reviewerType" : "delegate",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "description":"Sample description",
    "reviewers":
    [
        {
            "id":"f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        {
            "id":"5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    ],
    "settings":
    {
        "justificationRequiredOnApproval": true,
        "activityHistoryInDays":30,
        "mailNotificationsEnabled":true,
        "remindersEnabled":true
    }
}
```

##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegate",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
