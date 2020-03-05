---
title: Тип ресурса Програмконтрол
description: В функции рецензирования Access в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ee374108cdebca2e6ae06ee18a245f5c9eeebf74
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521448"
---
# <a name="programcontrol-resource-type"></a>Тип ресурса Програмконтрол

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции [рецензирования Access](accessreviews-root.md) в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание Програмконтрол](../api/programcontrol-create.md) |     [програмконтрол](programcontrol.md) |   Добавление Програмконтрол в программу.|
|[Удаление Програмконтрол](../api/programcontrol-delete.md) |     Нет.   |   Удаление Програмконтрол из программы.|
|[Список Програмконтролс](../api/programcontrol-list.md) | Коллекция [програмконтрол](programcontrol.md)| Перечисление элементов управления для всех программ в клиенте.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `id`                     |`String`                | Присвоенный компоненту идентификатор ссылки между программой и элементом управления                                      |
| `programId`              |`String`                | Програмид программы, частью которой является этот элемент управления. Требуется при создании.                            |
| `controlId`              |`String`                | ControlId элемента управления, в частности идентификатор проверки доступа. Требуется при создании.                                                |
| `controlTypeId`          |`String`                | Програмконтролтипе определяет тип элемента управления программы, например элемент управления, который связывается с проверками гостевого доступа. Требуется при создании. |
| `displayName`            |`String`                | Имя элемента управления.                                                             |
| `status`                 |`String`                | Состояние жизненного цикла элемента управления.                                                 |
| `createdDateTime`        |`DateTimeOffset`        | Дата и время создания программного элемента управления.                                        |
| `owner`                  |[userIdentity](useridentity.md)   | Пользователь, создавший элемент управления программы.                                               |
| `resource`               |`programResource`       | Ресурс, группа или приложение, предназначенные для проверки доступа этого элемента управления.                   |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `program`                |[Программа](program.md)               | Программа, частью которой является этот элемент управления.                                                |

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список Програмконтролс программы](../api/program-listcontrols.md) |      Коллекция [програмконтрол](programcontrol.md)| Получение коллекции элементов управления программы.|
|[Список Програмконтролтипес](../api/programcontroltype-list.md) | Коллекция [програмконтролтипе](programcontroltype.md)| Список типов элементов управления программы. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControl"
}-->

```json
{
 "id": "string (identifier)",
 "programId": "string (identifier)",
 "controlId": "string (identifier)",
 "controlTypeId": "string (identifier)",
 "displayName": "string",
 "status": "string",
 "createdDateTime": "string (timestamp)",
 "owner": {"@odata.type":"microsoft.graph.userIdentity"},
 "resource":{"@odata.type":"microsoft.graph.programResource"}
}

```

## <a name="the-programresource-complex-type"></a>Сложный тип Програмресаурце

Ресурс Program, содержащийся в объекте Program Control, представляет собой ссылку на объект, который является целевым объектом проверки доступа.

Этот тип наследуется `microsoft.graph.identity` от и обладает одним дополнительным свойством:

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `type`               |`String`  | Тип ресурса, указывающий, является ли он группой или приложением. |     

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programResource"
}-->

```json
{
 "type": "string"
}

```
<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
