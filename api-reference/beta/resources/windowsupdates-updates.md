---
title: обновляет тип ресурса
description: Сущность, которая выступает в качестве контейнера для всех функций клиентский компонент Центра обновления Windows развертывания для бизнеса.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a315516e8ded53cfacbe94c0ace2d9c12c5b3f78
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856416"
---
# <a name="updates-resource-type"></a>обновляет тип ресурса

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сущность, которая выступает в качестве контейнера для всех функций клиентский компонент Центра обновления Windows развертывания для бизнеса.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Только для чтения. Наследуется [от сущности](../resources/entity.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|Каталог|[microsoft.graph.windowsUpdates.catalog](../resources/windowsupdates-catalog.md)|Каталог содержимого, который может быть утвержден для развертывания службой развертывания. Только для чтения.|
|Развертывания|[Коллекция microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|Развертывания, созданные с помощью службы развертывания. Только для чтения.|
|resourceConnections|[Коллекция microsoft.graph.windowsUpdates.resourceConnection](../resources/windowsupdates-resourceconnection.md)|Подключения служб к внешним ресурсам, таким как рабочие области аналитики.|
|updatableAssets|[Коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Ресурсы, зарегистрированные в службе развертывания, которые могут получать обновления. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updates",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updates",
  "id": "String (identifier)"
}
```

