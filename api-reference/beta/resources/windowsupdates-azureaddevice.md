---
title: тип ресурса azureADDevice
description: Представляет устройство в Azure Active Directory Azure AD, которое регистрируется в службе развертывания.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a055c944c1b7a5f2bd4bbd23a9edc8d9c3b3ff88
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792192"
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

