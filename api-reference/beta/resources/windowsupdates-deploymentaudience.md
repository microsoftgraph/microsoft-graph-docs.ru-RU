---
title: тип ресурса deploymentAudience
description: Набор updatableAsset ресурсов, к которым может применяться развертывание.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ab436c0fa9f726528b190fa6fe2f638890447ce4
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863366"
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

## <a name="json-representation"></a>Представление JSON
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

