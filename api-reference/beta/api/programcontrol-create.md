---
title: Создание programControl
description: В функции обзоров доступа Azure AD создайте новый объект programControl.  Это связывает обзор доступа с программой.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: cd4a00faeee1b97adc525727c1c01d69f26e4a27
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049823"
---
# <a name="create-programcontrol"></a>Создание programControl

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) создайте новый [объект programControl.](../resources/programcontrol.md)  Это связывает обзор доступа с программой.

Прежде чем сделать этот запрос, вызываемая должна иметь ранее

- [создали программу](program-create.md) или [извлекли программу,](program-list.md)чтобы иметь значение включить `programId` в запрос,
- [создать обзор доступа](accessreview-create.md) или [получить обзор доступа,](accessreview-get.md)чтобы иметь значение включить в `controlId` запрос, и
- [извлекли список типов управления программой,](programcontroltype-list.md)чтобы иметь значение включить в `controlTypeId` запрос.


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | ProgramControl.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение                            |  ProgramControl.ReadWrite.All  |

Подписанный пользователь также должен быть в роли каталога, что позволяет им создавать **программуControl**. 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [programControl.](../resources/programcontrol.md)

В следующей таблице показаны свойства, необходимые при создании управления программой.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| `programId`              |`String`                | ProgramId программы этот контроль станет частью.                             |
| `controlId`              |`String`                | ControlId управления, в частности идентификатор обзора доступа.                                                |
| `controlTypeId`          |`String`                | ПрограммаControlType определяет тип управления программой , например, контрольную ссылку на отзывы о доступе гостей. |

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и `201, Created` [объект programControl](../resources/programcontrol.md) в тексте ответа.


## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В теле запроса поставляем JSON-представление [объекта programControl.](../resources/programcontrol.md)


# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-programcontrol-from-programcontrols-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-programcontrol-from-programcontrols-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-programcontrol-from-programcontrols-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-programcontrol-from-programcontrols-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
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
|[List programControlTypes](../api/programcontroltype-list.md) | [коллекция programControlType](../resources/programcontroltype.md)| Типы управления программами списка. |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


