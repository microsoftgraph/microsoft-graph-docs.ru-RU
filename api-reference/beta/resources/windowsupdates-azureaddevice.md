---
title: тип ресурса azureADDevice
description: Представляет устройство в Azure Active Directory Azure AD, которое регистрируется в службе развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a9d7b68257895674530acfbafcd0fb6b6c9c7b02
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068152"
---
# <a name="azureaddevice-resource-type"></a>тип ресурса azureADDevice

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет устройство в Azure Active Directory Azure AD, которое регистрируется в службе развертывания.

Устройство Azure AD автоматически создается с помощью одного из следующих методов:
* [updatableAsset: регистрацияAssets](../api/windowsupdates-updatableasset-enrollassets.md)
* [updatableAsset: регистрацияAssetsById](../api/windowsupdates-updatableasset-enrollassetsbyid.md)
* [deploymentAudience: updateAudience](../api/windowsupdates-deploymentaudience-updateaudience.md)
* [deploymentAudience: updateAudienceById](../api/windowsupdates-deploymentaudience-updateaudiencebyid.md)
* [updatableAssetGroup: addMembers](../api/windowsupdates-updatableassetgroup-addmembers.md)
* [updatableAssetGroup: addMembersById](../api/windowsupdates-updatableassetgroup-addmembersbyid.md)

Наследует [от updatableAsset](../resources/windowsupdates-updatableasset.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список ресурсов azureADDevice](../api/windowsupdates-updates-list-updatableassets-azureaddevice.md)|[коллекция microsoft.graph.windowsUpdates.azureADDevice](../resources/windowsupdates-azureaddevice.md)|Получите список объектов [AzureADDevice](../resources/windowsupdates-azureaddevice.md) и их свойств.|
|[Get azureADDevice](../api/windowsupdates-azureaddevice-get.md)|[microsoft.graph.windowsUpdates.azureADDevice](../resources/windowsupdates-azureaddevice.md)|Ознакомьтесь с свойствами и отношениями объекта [azureADDevice.](../resources/windowsupdates-azureaddevice.md)|
|[Удаление azureADDevice](../api/windowsupdates-azureaddevice-delete.md)|Нет|Удаление [объекта azureADDevice.](../resources/windowsupdates-azureaddevice.md)|
|[Регистрация ресурсов azureADDevice в управлении](../api/windowsupdates-updatableasset-enrollassets.md)|Нет|Регистрация [ресурсов azureADDevice](../resources/windowsupdates-azureaddevice.md) в управлении обновлениями службой развертывания.|
|[Регистрация ресурсов azureADDevice в управлении (по ID)](../api/windowsupdates-updatableasset-enrollassetsbyid.md)|Нет|Регистрация [ресурсов azureADDevice](../resources/windowsupdates-azureaddevice.md) в управлении обновлениями службой развертывания.|
|[Unenroll azureADDevice resources from management](../api/windowsupdates-updatableasset-unenrollassets.md)|Нет|Unenroll [azureADDevice resources](../resources/windowsupdates-azureaddevice.md) from update management by the deployment service.|
|[Unenroll azureADDevice resources from management (by ID)](../api/windowsupdates-updatableasset-unenrollassetsbyid.md)|Нет|Unenroll [azureADDevice resources](../resources/windowsupdates-azureaddevice.md) from update management by the deployment service.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|регистрация|[коллекция microsoft.graph.windowsUpdates.updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md)|Указывает области службы, в которую зачислилось устройство. Только для чтения. Возвращается по умолчанию.|
|ошибки|[коллекция microsoft.graph.windowsUpdates.updatableAssetError](../resources/windowsupdates-updatableasseterror.md)|Указывает все ошибки, которые мешают устройству быть зарегистрированным в управлении обновлениями или пересчете развернутого контента. Только для чтения. Возвращается по умолчанию.|
|id|String|Идентификатор устройства. Ключ. Значение null не допускается. Только для чтения. Возвращается по умолчанию. Унаследованный от [updatableAsset](../resources/windowsupdates-updatableasset.md)|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDevice",
  "baseType": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
  "id": "String (identifier)",
  "errors": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
    }
  ],
  "enrollments": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
    }
  ]
}
```

