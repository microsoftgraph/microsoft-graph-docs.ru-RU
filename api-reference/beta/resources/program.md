---
title: Тип ресурса программы
description: 'В Azure AD access дается обзор компонента, программа является контейнером, удерживая программы элементов управления. Клиент может иметь одну или несколько программ.  Все элементы управления, привязывающего проверки доступа к программе, чтобы упростить поиск связанных с ними доступа дается обзор.  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515190"
---
# <a name="program-resource-type"></a>Тип ресурса программы

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD программы является контейнером, удерживая программы элементов управления. Клиент может иметь одну или несколько программ.  Все элементы управления, привязывающего проверки доступа к программе, чтобы упростить поиск связанных с ними доступа дается обзор.  

Каждый клиент, который на boarded Azure AD обзоры доступа имеет один программу `Default program`.  Глобальный администратор может создать дополнительные программы, например для представления соответствия. 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание программы](../api/program-create.md) |   [Программа](program.md)   |   Создание программы.|
|[Удаление программы](../api/program-delete.md) |   Нет.   |   Удаление программы.|
|[Список программ](../api/program-list.md) |  [программа](program.md) семейства сайтов|   Получите коллекцию всех программ.|
|[Список programControls программы](../api/program-listcontrols.md) |      [programControl](programcontrol.md) коллекции| Получите коллекцию элементов управления из программы.|
|[Обновите программу](../api/program-update.md) |   [Программа](program.md)|  Обновите программу.|

## <a name="permissions"></a>Разрешения

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | ProgramControl.Read.All ProgramControl.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  Функция назначенный идентификатор программы.                    |
| `displayName`               |`String`                              |  Имя программы.  Требуется при создании.                  |
| `description`               |`String`                              |  Описание программы.           |

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| `controls`                  |[programControl](programcontrol.md) | Элементы управления, связанные с программой. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/program.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
