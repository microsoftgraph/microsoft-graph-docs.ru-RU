---
title: Тип ресурса teamwork
description: Контейнер для набора функциональных возможностей Microsoft Teams, доступных для организации.
author: charlieforce
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 3c5282ff44f2ae56d40e666548e222ccfb6e13f4
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690016"
---
# <a name="teamwork-resource-type"></a>Тип ресурса teamwork

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для набора функциональных возможностей Microsoft Teams, доступных для организации. 

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список deletedTeams](../api/teamwork-list-deletedteams.md)|Коллекция [deletedTeam](../resources/deletedteam.md)|Получение списка объектов [deletedTeam](../resources/deletedteam.md) и их свойств.|
|[Перечисление teamTemplates](../api/teamwork-list-teamtemplates.md)|[Коллекция teamTemplate](../resources/teamtemplate.md)|Получение списка объектов [teamTemplate](../resources/teamtemplate.md) , доступных для клиента. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String| Уникальный идентификатор. Наследуется от [сущности](../resources/entity.md).|

## <a name="relationships"></a>Связи
| Связь | Тип | Описание |
|:---------------|:--------|:----------|
|deletedTeams|Коллекция [deletedTeam](../resources/deletedteam.md)| Коллекция удаленных команд.|
|devices|коллекция [teamworkDevice](../resources/teamworkdevice.md)|Устройства Teams, подготовленные для клиента.|
|teamsAppSettings|[teamsAppSettings](../resources/teamsappsettings.md)|Представляет параметры на уровне клиента для всех [приложений Teams](teamsapp.md) в клиенте.|
|teamTemplates|[коллекция teamtemplate](../resources/teamtemplate.md)| Шаблоны, связанные с командой.|
|workforceIntegrations|коллекция [workforceIntegration](../resources/workforceintegration.md)| Интеграция рабочих ресурсов со сменами.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamwork",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
    "@odata.type": "#microsoft.graph.teamwork",
    "id": "String (identifier)"
}
```

## <a name="see-also"></a>См. также

- [Ресурс userTeamwork](userteamwork.md)

