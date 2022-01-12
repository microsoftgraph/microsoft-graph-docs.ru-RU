---
title: тип ресурса updatableAsset
description: Представляет актив, который может получать обновления.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: af8759504e5b79a28686a9070de23c522b9eb0e3
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61859969"
---
# <a name="updatableasset-resource-type"></a>тип ресурса updatableAsset

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет актив, который может получать обновления.

Все updatable assets существуют как один из следующих производных типов: [azureADDevice](../resources/windowsupdates-azureaddevice.md) и [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)

Базовый тип [azureADDevice](../resources/windowsupdates-azureaddevice.md) и [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)

Это абстрактный тип.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список ресурсов updatableAsset](../api/windowsupdates-updates-list-updatableassets.md)|[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Получите список объектов [updatableAsset](../resources/windowsupdates-updatableasset.md) и их свойств.|
|[Создание updatableAssetGroup](../api/windowsupdates-updates-post-updatableassets-updatableassetgroup.md)|[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)|Создание нового [объекта updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Get updatableAsset](../api/windowsupdates-updatableasset-get.md)|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Ознакомьтесь с свойствами и отношениями [объекта updatableAsset.](../resources/windowsupdates-updatableasset.md)|
|[Удаление updatableAsset](../api/windowsupdates-updatableasset-delete.md)|Нет|Удаление [объекта updatableAsset.](../resources/windowsupdates-updatableasset.md)|
|[Регистрация активов в управлении](../api/windowsupdates-updatableasset-enrollassets.md)|Нет|Регистрация [updatableAssets в](../resources/windowsupdates-updatableasset.md) управлении обновлениями службой развертывания.|
|[Регистрация активов в управлении (по ID)](../api/windowsupdates-updatableasset-enrollassetsbyid.md)|Нет|Регистрация [updatableAssets](../resources/windowsupdates-updatableasset.md) того же типа в управлении обновлениями службой развертывания.|
|[Unenroll asset from management](../api/windowsupdates-updatableasset-unenrollassets.md)|Нет|Unenroll [updatableAssets](../resources/windowsupdates-updatableasset.md) from update management by the deployment service.|
|[Unenroll asset from management (by ID)](../api/windowsupdates-updatableasset-unenrollassetsbyid.md)|Нет|Unenroll [updatableAssets](../resources/windowsupdates-updatableasset.md) того же типа из управления обновлениями службой развертывания.|
|[Добавление участников в группу](../api/windowsupdates-updatableassetgroup-addmembers.md)|Нет|Добавление участников в [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Добавление участников в группу (по ID)](../api/windowsupdates-updatableassetgroup-addmembersbyid.md)|Нет|Добавьте членов одного типа в [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Удаление участников из группы](../api/windowsupdates-updatableassetgroup-removemembers.md)|Нет|Удаление участников [из updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)|
|[Удаление участников из группы (по ID)](../api/windowsupdates-updatableassetgroup-removemembersbyid.md)|Нет|Удалите членов одного типа из [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор для актива. Ключ. Значение null не допускается. Только для чтения. Возвращается по умолчанию.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
  "id": "String (identifier)"
}
```

