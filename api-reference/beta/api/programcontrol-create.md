---
title: Создание programControl
description: В Azure AD доступа к функции проверки, создайте новый объект programControl.  Это связывает проверки доступа к программе.
localization_priority: Normal
ms.openlocfilehash: 4dfbb76244a41867b8a57faa42f63dc728f59136
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851536"
---
# <a name="create-programcontrol"></a>Создание programControl

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD создайте новый объект [programControl](../resources/programcontrol.md) .  Это связывает проверки доступа к программе.

До внесения этого запроса, вызывающий объект должен иметь ранее

 - [созданные программы](program-create.md) или [вернуть программу](program-list.md), иметь значение `programId` необходимо включить в запрос,
 - [создан проверки доступа](accessreview-create.md) или [получить обзор доступа](accessreview-get.md), иметь значение `controlId` необходимо включить в запрос, и
 - [получить список типов элементов управления программы](programcontroltype-list.md), иметь значение `controlTypeId` необходимо включить в запрос.


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | `ProgramControl.ReadWrite.All`.  Также должен быть выполнен вход пользователя в роль каталог, который позволяет использовать для создания programControl. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носителя \{маркеров\}. Обязательный. |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите представление JSON объекта [programControl](../resources/programcontrol.md) .

Ниже приведены свойства, которые необходимы для создания элемента управления программы.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| `programId`              |`String`                | ProgramId программа этот элемент управления будет стать частью.                             |
| `controlId`              |`String`                | ControlId элемента управления, в частности идентификатор доступа просмотрите.                                                |
| `controlTypeId`          |`String`                | ProgramControlType определяет тип элемента управления, программа -, например дается обзор элемента управления, создание ссылок на доступ в качестве гостя. |

## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `201, Created` код ответа и объект [programControl](../resources/programcontrol.md) в теле ответа.


## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В тексте запроса укажите представление объекта [programControl](../resources/programcontrol.md) с JSON.

<!-- {
  "blockType": "request",
  "name": "create_programControl_from_programControls"
}-->
```http
POST https://graph.microsoft.com/beta/programControls
Content-type: application/json

{
    "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
}
```

##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "63b2302c-7e62-43b7-aefb-063ba5bdb853",
  "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
  "displayName": "test",
  "status": "Active",
  "createdDateTime": "2018-05-18T20:26:05.2976279Z"
}
```

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список programControlTypes](../api/programcontroltype-list.md) | [programControlType](../resources/programcontroltype.md) коллекции| Список типов элементов управления программы. |


<!-- {
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
