---
title: teamTemplateDefinition
description: Универсальное представление определения шаблона команды для команды с определенной структурой и конфигурацией.
author: Charlieforce
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 9df396be7eca713cd407c253af8285528e6587f8
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690127"
---
# <a name="teamtemplatedefinition-resource-type"></a>Тип ресурса teamTemplateDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Универсальное представление определения шаблона команды для команды с определенной структурой и конфигурацией.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение teamTemplateDefinition](../api/teamtemplatedefinition-get.md)|[teamTemplateDefinition](../resources/teamtemplatedefinition.md)|Чтение свойств и связей объекта [teamTemplateDefinition](../resources/teamtemplatedefinition.md) .|
| [Перечисление teamTemplateDefinitions](../api/teamtemplate-list-definitions.md) | [Коллекция teamTemplateDefinition](../resources/teamtemplatedefinition.md) | Список объектов **teamTemplateDefinition** , связанных с **teamTemplate**.  |
| [Получение teamDefinition](../api/teamtemplatedefinition-get-teamdefinition.md) | [team](../resources/team.md) | Чтение свойств команды **объекта** **teamTemplateDefinition** |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Аудитории|teamTemplateAudience|Описание аудитории, доступной для шаблона команды. Допустимые значения: `organization`, `user`, `public`, `unknownFutureValue`.|
|categories|Коллекция String|Назначенные категории для шаблона команды.|
|description|Строка|Краткое описание шаблона команды, которое будет отображаться пользователям в Microsoft Teams.|
|displayName|String|Определяемое пользователем имя шаблона команды.|
|iconUrl|Строка|URL-адрес значка для шаблона команды.|
|id|Строка|Кодировка 64 `templateId` +  + `audience``locale` для шаблона команды. Наследуется от [сущности](../resources/entity.md).|
|languageTag|Строка|Язык, на который доступен шаблон.|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Удостоверение пользователя, который последним изменил шаблон команды.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения шаблона команды.|
|parentTemplateId|Строка|Шаблон `templateId` команды|
|publisherName|String|Организация, опубликовав шаблон команды.|
|shortDescription|String|Краткое описание шаблона команды, которое будет отображаться пользователям в Microsoft Teams.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|teamDefinition|[team](../resources/team.md)|Коллекция [объектов канала](../resources/channel.md) . Канал представляет тему и логически обособляет обсуждение в команде.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamtemplatedefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamTemplateDefinition",
  "id": "String (identifier)",
  "parentTemplateId": "String",
  "displayName": "String",
  "languageTag": "String",
  "audience": "String",
  "description": "String",
  "shortDescription": "String",
  "iconUrl": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "publisherName": "String",
  "categories": [
    "String"
  ]
}
```
## <a name="see-also"></a>См. также

- [team](team.md)
- [teamsTemplate](teamsTemplate.md)
