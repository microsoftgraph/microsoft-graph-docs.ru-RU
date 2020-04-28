---
title: Создание Програмконтрол
description: В средстве проверки доступа Azure AD создайте новый объект Програмконтрол.  При этом будет связана проверка доступа к программе.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 17c25df842975c324ab827fc071283df7a5d44cd
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123097"
---
# <a name="create-programcontrol"></a>Создание Програмконтрол

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В средстве проверки [доступа](../resources/accessreviews-root.md) Azure AD создайте новый объект [програмконтрол](../resources/programcontrol.md) .  При этом будет связана проверка доступа к программе.

Перед выполнением этого запроса вызывающий абонент должен был

- [созданная программа](program-create.md) или [получена программа](program-list.md)со значением `programId` , включаемым в запрос.
- [создана проверка доступа](accessreview-create.md) или [полученная проверка доступа](accessreview-get.md), для которой значение `controlId` должно быть включено в запрос, а
- [получен список типов программного управления](programcontroltype-list.md), чтобы включить в запрос значение `controlTypeId` , которое необходимо включить в запрос.


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | ProgramControl.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            |  ProgramControl.ReadWrite.All  |

Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им создавать **програмконтрол**. 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [програмконтрол](../resources/programcontrol.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании программного элемента управления.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| `programId`              |`String`                | Програмид программы, которая будет являться частью этого элемента управления.                             |
| `controlId`              |`String`                | ControlId элемента управления, в частности идентификатор проверки доступа.                                                |
| `controlTypeId`          |`String`                | Програмконтролтипе определяет тип элемента управления программы, например элемент управления, который связывается с проверками гостевого доступа. |

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [програмконтрол](../resources/programcontrol.md) в тексте отклика.


## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В тексте запроса добавьте представление объекта [програмконтрол](../resources/programcontrol.md) в формате JSON.


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

---


##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
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
|[Список Програмконтролтипес](../api/programcontroltype-list.md) | Коллекция [програмконтролтипе](../resources/programcontroltype.md)| Список типов элементов управления программы. |


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
