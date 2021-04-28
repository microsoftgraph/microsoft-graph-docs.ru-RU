---
title: тип ресурса deploymentAudience
description: Набор updatableAsset ресурсов, к которым может применяться развертывание.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 98d295183f69012da6ea9fc5803bc440465854c8
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067526"
---
# <a name="deploymentaudience-resource-type"></a>тип ресурса deploymentAudience

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Набор [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсов, к которым [может применяться](../resources/windowsupdates-deployment.md) развертывание.

Если один и тот же ресурс **updatableAsset** включен в отношения исключений и участников, развертывание не будет применяться к ним.  

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление участников](../api/windowsupdates-deploymentaudience-list-members.md)|[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Список участников [развертыванияAudience](../resources/windowsupdates-deploymentaudience.md).|
|[Исключения списка](../api/windowsupdates-deploymentaudience-list-exclusions.md)|[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Список исключений [развертыванияAudience](../resources/windowsupdates-deploymentaudience.md).|
|[Обновление участников и исключений](../api/windowsupdates-deploymentaudience-updateaudience.md)|Нет|Добавление или удаление участников и исключений.|
|[Обновление участников и исключений (по ID)](../api/windowsupdates-deploymentaudience-updateaudiencebyid.md)|Нет|Добавление или удаление участников и исключений одного типа.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для аудитории развертывания. Возвращается по умолчанию. Ключ. Значение null не допускается. Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|исключения|[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Указывает ресурсы, которые необходимо исключить из аудитории.|
|members|[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Указывает активы, которые необходимо включить в аудиторию.|

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentAudience",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentAudience",
  "id": "String (identifier)"
}
```

