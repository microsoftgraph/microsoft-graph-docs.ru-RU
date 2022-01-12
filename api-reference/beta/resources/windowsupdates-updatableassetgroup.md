---
title: тип ресурсов updatableAssetGroup
description: Группа ресурсов azureADDevice, которые могут получать обновления.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 91e230fe3c158da0b02ce5af9df6f660855d253a
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861592"
---
# <a name="updatableassetgroup-resource-type"></a>тип ресурсов updatableAssetGroup

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Группа ресурсов [azureADDevice,](../resources/windowsupdates-azureaddevice.md) которые могут получать обновления.

Участники — это тип [ресурса azureADDevice.](../resources/windowsupdates-azureADDevice.md) Ресурс **updatableAssetGroup** не может быть членом другой **updatableAssetGroup.**

Наследует [от updatableAsset](../resources/windowsupdates-updatableasset.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список ресурсов updatableAssetGroup](../api/windowsupdates-updates-list-updatableassets-updatableassetgroup.md)|[коллекция microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)|Получите список объектов [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) и их свойств.|
|[Создание updatableAssetGroup](../api/windowsupdates-updates-post-updatableassets-updatableassetgroup.md)|[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)|Создание нового [объекта updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Get updatableAssetGroup](../api/windowsupdates-updatableassetgroup-get.md)|[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)|Ознакомьтесь с свойствами и отношениями объекта [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Удаление updatableAssetGroup](../api/windowsupdates-updatableassetgroup-delete.md)|Нет|Удаляет объект [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Добавление участников](../api/windowsupdates-updatableassetgroup-addmembers.md)|Нет|Добавление участников в [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Добавление участников (по ID)](../api/windowsupdates-updatableassetgroup-addmembers.md)|Нет|Добавление участников в [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Удаление участников](../api/windowsupdates-updatableassetgroup-removemembers.md)|Нет|Удаление участников [из updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Удаление участников (по ID)](../api/windowsupdates-updatableassetgroup-removemembers.md)|Нет|Удаление участников [из updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Перечисление участников](../api/windowsupdates-updatableassetgroup-list-members.md)|[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Получите [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсы из свойства навигации членов.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор для группы. Ключ. Значение null не допускается. Только для чтения. Возвращается по умолчанию. Унаследовано от [updatableAsset](../resources/windowsupdates-updatableasset.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|members|[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Члены группы. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup",
  "baseType": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
  "id": "String (identifier)"
}
```

