---
title: Тип ресурса programControl
description: В Azure AD access дается обзор компонента, объект элемента управления программа представляет элемент управления, связывание проверки доступа к программе.
localization_priority: Normal
ms.openlocfilehash: 3d9829b8e2585d4deda95551021e2fd9b8d14c7a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511417"
---
# <a name="programcontrol-resource-type"></a>Тип ресурса programControl

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD объект элемента управления программа представляет элемент управления, связывание проверки доступа к программе.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Добавьте programControl программы.|
|[Удаление programControl](../api/programcontrol-delete.md) |     Нет.   |   Удалите programControl из программы.|
|[Список programControls](../api/programcontrol-list.md) | [programControl](programcontrol.md) коллекции| Список элементов управления для всех программ в клиентов.|

## <a name="permissions"></a>Разрешения

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | ProgramControl.Read.All ProgramControl.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `id`                     |`String`                | Идентификатор компонента назначенных связи между программы и элемента управления                                      |
| `programId`              |`String`                | ProgramId программа этот элемент управления является частью. Требуется при создании.                            |
| `controlId`              |`String`                | ControlId элемента управления, в частности идентификатор доступа просмотрите. Требуется при создании.                                                |
| `controlTypeId`          |`String`                | ProgramControlType определяет тип элемента управления, программа -, например дается обзор элемента управления, создание ссылок на доступ в качестве гостя. Требуется при создании. |
| `displayName`            |`String`                | Имя элемента управления.                                                             |
| `status`                 |`String`                | Состояние жизненного цикла элемента управления.                                                 |
| `createdDateTime`        |`DateTimeOffset`        | Дату и время создания элемента управления программы.                                        |
| `owner`                  |[удостоверению пользователя](useridentity.md)   | Пользователь, создавший элемент управления программы.                                               |
| `resource`               |`programResource`       | Ресурс, группы или приложения, входят в целевую этот элемент управления программы проверки доступа.                   |

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `program`                |[Программа](program.md)               | Программа этот элемент управления является частью.                                                |

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список programControls программы](../api/program-listcontrols.md) |      [programControl](programcontrol.md) коллекции| Получите коллекцию элементов управления из программы.|
|[Список programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md) коллекции| Список типов элементов управления программы. |

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса в формате JSON.

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
 "owner": "microsoft.graph.userIdentity",
 "resource":"microsoft.graph.programResource"
}

```

## <a name="the-programresource-complex-type"></a>Сложный тип programResource

Программа ресурсов, содержащихся в объект элемента управления программа представляет ссылку на объект, который является целевым для проверки доступа.

Этот тип наследует от `microsoft.graph.identity` и имеет один дополнительные свойства:

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `type`               |`String`  | Тип ресурса, которое показывает, является ли группы или приложения. |     


<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontrol.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
