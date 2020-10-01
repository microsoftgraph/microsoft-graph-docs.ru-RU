---
title: Тип ресурса Програмконтрол
description: В функции рецензирования Access в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 9837f160015dedb0f37cce65b8209ff9a6ec5331
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330178"
---
# <a name="programcontrol-resource-type"></a>Тип ресурса Програмконтрол

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции [рецензирования Access](accessreviews-root.md) в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.


## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:------ |:----------- |:----------- |
| [Создание Програмконтрол](../api/programcontrol-create.md) |    [програмконтрол](programcontrol.md) |   Добавление Програмконтрол в программу. |
| [Удаление Програмконтрол](../api/programcontrol-delete.md) | Нет. | Удаление Програмконтрол из программы. |
| [Список Програмконтролс](../api/programcontrol-list.md) | Коллекция [програмконтрол](programcontrol.md) | Перечисление элементов управления для всех программ в клиенте. |
| [Список Програмконтролс программы](../api/program-listcontrols.md) | Коллекция [програмконтрол](programcontrol.md) |    Получение коллекции элементов управления программы. |
| [Список Програмконтролтипес](../api/programcontroltype-list.md) | Коллекция [програмконтролтипе](programcontroltype.md)| Список типов элементов управления программы. |

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:-------- |:---- |:----------- |
| id | Строка | Присвоенный компоненту идентификатор ссылки между программой и элементом управления. |
| програмид | Строка | Програмид программы, частью которой является этот элемент управления. Требуется при создании. |
| controlId | Строка | ControlId элемента управления, в частности идентификатор проверки доступа. Требуется при создании. |
| контролтипеид | Строка | Програмконтролтипе определяет тип элемента управления программы, например элемент управления, который связывается с проверками гостевого доступа. Требуется при создании. |
| displayName | Строка | Имя элемента управления. |
| status | String | Состояние жизненного цикла элемента управления. |
| createdDateTime | DateTimeOffset | Дата и время создания программного элемента управления. |
| owner | [userIdentity](useridentity.md) | Пользователь, создавший элемент управления программы. |
| resource | [програмресаурце](programresource.md) | Ресурс, группа или приложение, предназначенные для проверки доступа этого элемента управления. |

## <a name="relationships"></a>Отношения

| Связь | Тип   | Описание |
|:------------ |:---- |:----------- |
| Программа | [Программа](program.md) | Программа, частью которой является этот элемент управления. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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


