---
title: Тип ресурса Програмконтрол
description: В функции рецензирования Access в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.
localization_priority: Normal
ms.openlocfilehash: 3d9829b8e2585d4deda95551021e2fd9b8d14c7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563385"
---
# <a name="programcontrol-resource-type"></a>Тип ресурса Програмконтрол

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции рецензирования [Access](accessreviews-root.md) в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание Програмконтрол](../api/programcontrol-create.md) |     [Програмконтрол](programcontrol.md) |   Добавление Програмконтрол в программу.|
|[Удаление Програмконтрол](../api/programcontrol-delete.md) |     Нет.   |   Удаление Програмконтрол из программы.|
|[Список Програмконтролс](../api/programcontrol-list.md) | Коллекция [програмконтрол](programcontrol.md)| ПереЧисление элементов управления для всех программ в клиенте.|

## <a name="permissions"></a>Разрешения

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

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
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
| `program`                |[Программа](program.md)               | Программа, частью которой является этот элемент управления.                                                |

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список Програмконтролс программы](../api/program-listcontrols.md) |      Коллекция [програмконтрол](programcontrol.md)| Получение коллекции элементов управления программы.|
|[Список Програмконтролтипес](../api/programcontroltype-list.md) | Коллекция [програмконтролтипе](programcontroltype.md)| Список типов элементов управления программы. |

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

## <a name="the-programresource-complex-type"></a>Сложный тип Програмресаурце

Ресурс Program, содержащийся в объекте Program Control, представляет собой ссылку на объект, который является целевым объектом проверки доступа.

Этот тип наследуется `microsoft.graph.identity` от и обладает одним дополнительным свойством:

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `type`               |`String`  | Тип ресурса, указывающий, является ли он группой или приложением. |     


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
