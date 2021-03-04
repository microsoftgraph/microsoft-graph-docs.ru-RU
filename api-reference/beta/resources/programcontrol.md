---
title: тип ресурса programControl
description: В функции обзоров доступа Azure AD объект управления программой представляет элемент управления, связывающий обзор доступа с программой.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 492dc57bfa332472cb7565580ffaa8a5260234c0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443981"
---
# <a name="programcontrol-resource-type"></a>тип ресурса programControl

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции обзоров доступа Azure [AD](accessreviews-root.md) объект управления программой представляет элемент управления, связывающий обзор доступа с программой.


## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:------ |:----------- |:----------- |
| [Создание programControl](../api/programcontrol-create.md) |    [programControl](programcontrol.md) |   Добавьте программуControl в программу. |
| [Удаление программыControl](../api/programcontrol-delete.md) | Нет. | Удаление программыControl из программы. |
| [List programControls](../api/programcontrol-list.md) | [коллекция programControl](programcontrol.md) | Элементы управления списками для всех программ в клиенте. |
| [Список программКонтроли программы](../api/program-listcontrols.md) | [коллекция programControl](programcontrol.md) |    Получите коллекцию элементов управления программы. |
| [List programControlTypes](../api/programcontroltype-list.md) | [коллекция programControlType](programcontroltype.md)| Типы управления программами списка. |

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:-------- |:---- |:----------- |
| id | String | Обозначенный функцией идентификатор связи между программой и элементом управления. |
| programId | String | ProgramId программы этот контроль является частью. Требуется при создании. |
| controlId | String | ControlId управления, в частности идентификатор обзора доступа. Требуется при создании. |
| controlTypeId | String | ПрограммаControlType определяет тип управления программой , например, контрольную ссылку на отзывы о доступе гостей. Требуется при создании. |
| displayName | String | Имя управления. |
| status | String | Состояние жизненного цикла управления. |
| createdDateTime | DateTimeOffset | Дата создания и время управления программой. |
| owner | [userIdentity](useridentity.md) | Пользователь, создавший управление программой. |
| resource | [programResource](programresource.md) | Ресурс, группа или приложение, которые ориентированы на обзор доступа управления этой программой. |

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:------------ |:---- |:----------- |
| программа | [программа](program.md) | Программа, частью этой системы управления. |

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


