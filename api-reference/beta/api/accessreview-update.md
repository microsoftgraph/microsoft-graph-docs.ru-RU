---
title: Обновление accessReview
description: В Azure AD access дается обзор компонента "," Обновление существующий объект accessReview изменение одно или несколько свойств.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e4e74daa092c6f18c845c7f0c468af90385b899b
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016753"
---
# <a name="update-accessreview"></a>Обновление accessReview

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [accessReview](../resources/accessreview.md) изменение одно или несколько свойств.

Этот интерфейс API не предназначен для изменения рецензентов или решения, принимаемые проверки.  Чтобы изменить рецензентов, используйте [addReviewer](accessreview-addreviewer.md) или [removeReviewer](accessreview-removereviewer.md) API-интерфейсы.  Чтобы остановить одноразовый review уже запущенной или уже запущен экземпляр повторяющейся проверки, раньше, используйте [Остановить](accessreview-stop.md) API. Чтобы применить решения для целевой группы или приложения права доступа, используйте [Применение](accessreview-apply.md) API. 


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носителя \{маркеров\}. Обязательная часть. |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите представление JSON параметров объекта [accessReview](../resources/accessreview.md) .

В следующей таблице показаны свойства, которые могут быть предоставлены при обновлении accessReview.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | Имя проверки доступа.  |
| `startDateTime`           |`DateTimeOffset`                                                | Дата и время при планировании проверки быть запуск.  Это должно быть даты в будущем.   |
| `endDateTime`             |`DateTimeOffset`                                                | Дата и время после запланированного окончания проверки. Это должно быть более поздней, чем дата начала по крайней мере один день.   |
| `description`             |`String`                                                        | Описание, чтобы показать рецензентов. |



## <a name="response"></a>Отклик
Успешно завершена, этот метод возвращает `204, Accepted` код ответа и объект [accessReview](../resources/accessreview.md) в теле ответа.

## <a name="example"></a>Пример

Это пример обновления одноразовый (не периодические) проверки доступа.

##### <a name="request"></a>Запрос
В тексте запроса укажите представление JSON новых свойств объекта [accessReview](../resources/accessreview.md) .

<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews('006111db-0810-4494-a6df-904d368bd81b')
Content-type: application/json

{
    "displayName":"TestReview new name"
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
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview new name",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
