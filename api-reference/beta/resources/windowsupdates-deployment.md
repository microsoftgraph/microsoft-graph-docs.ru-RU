---
title: Тип ресурса развертывания
description: Представляет развертывание контента на наборе устройств.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: e34bca8fc1776c749e42e97caa1dd0d91fa51433
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068104"
---
# <a name="deployment-resource-type"></a>Тип ресурса развертывания

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет развертывание контента на наборе устройств.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Развертывание списков](../api/windowsupdates-updates-list-deployments.md)|[коллекция microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|Получите список объектов [развертывания](../resources/windowsupdates-deployment.md) и их свойств.|
|[Создание развертывания](../api/windowsupdates-updates-post-deployments.md)|[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|Создание нового [объекта развертывания.](../resources/windowsupdates-deployment.md)|
|[Развертывание](../api/windowsupdates-deployment-get.md)|[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|Ознакомьтесь с свойствами и отношениями объекта [развертывания.](../resources/windowsupdates-deployment.md)|
|[Обновление развертывания](../api/windowsupdates-deployment-update.md)|[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|Обновление свойств объекта [развертывания.](../resources/windowsupdates-deployment.md)|
|[Удаление развертывания](../api/windowsupdates-deployment-delete.md)|Нет|Удаляет объект [развертывания.](../resources/windowsupdates-deployment.md)|
|[Список участников аудитории](../api/windowsupdates-deploymentaudience-list-members.md)|[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Список участников аудитории развертывания.|
|[Исключения аудитории списка](../api/windowsupdates-deploymentaudience-list-exclusions.md)|[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Список исключений из аудитории развертывания.|
|[Обновление участников аудитории и исключений](../api/windowsupdates-deploymentaudience-updateaudience.md)|Нет|Добавление или удаление участников и исключений из аудитории развертывания.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|content|[microsoft.graph.windowsUpdates.deployableContent](../resources/windowsupdates-deployablecontent.md)|Указывает, какой контент развернуть. Невозможно изменить. Возвращается по умолчанию.|
|createdDateTime|DateTimeOffset|Дата и время создания развертывания. Возвращается по умолчанию. Только для чтения.|
|id|String|Уникальный идентификатор для развертывания. Возвращается по умолчанию. Ключ. Значение null не допускается. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения развертывания. Возвращается по умолчанию. Только для чтения.|
|settings|[microsoft.graph.windowsUpdates.deploymentSettings](../resources/windowsupdates-deploymentsettings.md)|Параметры конкретного развертывания, регулирующих развертывание **контента.** Возвращается по умолчанию.|
|state|[microsoft.graph.windowsUpdates.deploymentState](../resources/windowsupdates-deploymentstate.md)|Состояние выполнения развертывания. Возвращается по умолчанию.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|аудитория|[microsoft.graph.windowsUpdates.deploymentAudience](../resources/windowsupdates-deploymentaudience.md)|Указывает аудиторию, к которой развернут контент.|

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.deployment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "String (identifier)",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
  },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.deployableContent"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

