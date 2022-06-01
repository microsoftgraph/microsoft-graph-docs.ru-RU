---
title: Тип ресурса programControl (не рекомендуется)
description: В Azure AD проверки доступа объект управления программой представляет элемент управления, связывая проверку доступа с программой.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 8f3acee6e81452f9cc5cc839ab89b5ee61cfa401
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820919"
---
# <a name="programcontrol-resource-type-deprecated"></a>Тип ресурса programControl (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

В Azure AD [проверки доступа](accessreviews-root.md) объект управления программой представляет элемент управления, связывая проверку доступа с программой.


## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:------ |:----------- |:----------- |
| [Создание объекта programControl](../api/programcontrol-create.md) |    [programControl](programcontrol.md) |   Добавьте programControl в программу. |
| [Удаление programControl](../api/programcontrol-delete.md) | Нет. | Удалите programControl из программы. |
| [Перечисление объектов programControls](../api/programcontrol-list.md) | [Коллекция programControl](programcontrol.md) | Вывод списка элементов управления во всех программах в клиенте. |
| [Перечисление programControls программы](../api/program-listcontrols.md) | [Коллекция programControl](programcontrol.md) |    Получение коллекции элементов управления программы. |
| [Перечисление programControlTypes](../api/programcontroltype-list.md) | [Коллекция programControlType](programcontroltype.md)| Перечисление типов элементов управления программой. |

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:-------- |:---- |:----------- |
| id | Строка | Назначенный компонентом идентификатор связи между программой и элементом управления. |
| programId | Строка | ProgramId программы, частью части этого элемента управления. Требуется при создании. |
| Controlid | Строка | Идентификатор элемента управления, в частности идентификатор проверки доступа. Требуется при создании. |
| controlTypeId | Строка | ProgramControlType определяет тип управления программой, например элемент управления, связывающий проверки гостевого доступа. Требуется при создании. |
| displayName | Строка | Имя элемента управления. |
| status | String | Состояние жизненного цикла элемента управления. |
| createdDateTime | DateTimeOffset | Дата и время создания элемента управления программой. |
| owner | [userIdentity](useridentity.md) | Пользователь, создавший элемент управления программой. |
| resource | [programResource](programresource.md) | Ресурс, группа или приложение, предназначенные для проверки доступа этого элемента управления программой. |

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:------------ |:---- |:----------- |
| Программа | [Программа](program.md) | Программа, частью функции управления. |

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


