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
# <a name="azureaddevice-resource-type"></a><span data-ttu-id="a6c7f-103">тип ресурса azureADDevice</span><span class="sxs-lookup"><span data-stu-id="a6c7f-103">azureADDevice resource type</span></span>

<span data-ttu-id="a6c7f-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="a6c7f-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6c7f-105">Представляет устройство в Azure Active Directory Azure AD, которое регистрируется в службе развертывания.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-105">Represents a device in Azure Active Directory (Azure AD) that is registered with the deployment service.</span></span>

<span data-ttu-id="a6c7f-106">Устройство Azure AD автоматически создается с помощью одного из следующих методов:</span><span class="sxs-lookup"><span data-stu-id="a6c7f-106">An Azure AD device is automatically created through one of the following methods:</span></span>
* [<span data-ttu-id="a6c7f-107">updatableAsset: регистрацияAssets</span><span class="sxs-lookup"><span data-stu-id="a6c7f-107">updatableAsset: enrollAssets</span></span>](../api/windowsupdates-updatableasset-enrollassets.md)
* [<span data-ttu-id="a6c7f-108">updatableAsset: регистрацияAssetsById</span><span class="sxs-lookup"><span data-stu-id="a6c7f-108">updatableAsset: enrollAssetsById</span></span>](../api/windowsupdates-updatableasset-enrollassetsbyid.md)
* [<span data-ttu-id="a6c7f-109">deploymentAudience: updateAudience</span><span class="sxs-lookup"><span data-stu-id="a6c7f-109">deploymentAudience: updateAudience</span></span>](../api/windowsupdates-deploymentaudience-updateaudience.md)
* [<span data-ttu-id="a6c7f-110">deploymentAudience: updateAudienceById</span><span class="sxs-lookup"><span data-stu-id="a6c7f-110">deploymentAudience: updateAudienceById</span></span>](../api/windowsupdates-deploymentaudience-updateaudiencebyid.md)
* [<span data-ttu-id="a6c7f-111">updatableAssetGroup: addMembers</span><span class="sxs-lookup"><span data-stu-id="a6c7f-111">updatableAssetGroup: addMembers</span></span>](../api/windowsupdates-updatableassetgroup-addmembers.md)
* [<span data-ttu-id="a6c7f-112">updatableAssetGroup: addMembersById</span><span class="sxs-lookup"><span data-stu-id="a6c7f-112">updatableAssetGroup: addMembersById</span></span>](../api/windowsupdates-updatableassetgroup-addmembersbyid.md)

<span data-ttu-id="a6c7f-113">Наследует [от updatableAsset](../resources/windowsupdates-updatableasset.md).</span><span class="sxs-lookup"><span data-stu-id="a6c7f-113">Inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a6c7f-114">Методы</span><span class="sxs-lookup"><span data-stu-id="a6c7f-114">Methods</span></span>
|<span data-ttu-id="a6c7f-115">Метод</span><span class="sxs-lookup"><span data-stu-id="a6c7f-115">Method</span></span>|<span data-ttu-id="a6c7f-116">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="a6c7f-116">Return type</span></span>|<span data-ttu-id="a6c7f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="a6c7f-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a6c7f-118">Список ресурсов azureADDevice</span><span class="sxs-lookup"><span data-stu-id="a6c7f-118">List azureADDevice resources</span></span>](../api/windowsupdates-updates-list-updatableassets-azureaddevice.md)|<span data-ttu-id="a6c7f-119">[коллекция microsoft.graph.windowsUpdates.azureADDevice](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="a6c7f-119">[microsoft.graph.windowsUpdates.azureADDevice](../resources/windowsupdates-azureaddevice.md) collection</span></span>|<span data-ttu-id="a6c7f-120">Получите список объектов [AzureADDevice](../resources/windowsupdates-azureaddevice.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-120">Get a list of the [azureADDevice](../resources/windowsupdates-azureaddevice.md) objects and their properties.</span></span>|
|[<span data-ttu-id="a6c7f-121">Get azureADDevice</span><span class="sxs-lookup"><span data-stu-id="a6c7f-121">Get azureADDevice</span></span>](../api/windowsupdates-azureaddevice-get.md)|[<span data-ttu-id="a6c7f-122">microsoft.graph.windowsUpdates.azureADDevice</span><span class="sxs-lookup"><span data-stu-id="a6c7f-122">microsoft.graph.windowsUpdates.azureADDevice</span></span>](../resources/windowsupdates-azureaddevice.md)|<span data-ttu-id="a6c7f-123">Ознакомьтесь с свойствами и отношениями объекта [azureADDevice.](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="a6c7f-123">Read the properties and relationships of an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>|
|[<span data-ttu-id="a6c7f-124">Удаление azureADDevice</span><span class="sxs-lookup"><span data-stu-id="a6c7f-124">Delete azureADDevice</span></span>](../api/windowsupdates-azureaddevice-delete.md)|<span data-ttu-id="a6c7f-125">Нет</span><span class="sxs-lookup"><span data-stu-id="a6c7f-125">None</span></span>|<span data-ttu-id="a6c7f-126">Удаление [объекта azureADDevice.](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="a6c7f-126">Delete an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>|
|[<span data-ttu-id="a6c7f-127">Регистрация ресурсов azureADDevice в управлении</span><span class="sxs-lookup"><span data-stu-id="a6c7f-127">Enroll azureADDevice resources in management</span></span>](../api/windowsupdates-updatableasset-enrollassets.md)|<span data-ttu-id="a6c7f-128">Нет</span><span class="sxs-lookup"><span data-stu-id="a6c7f-128">None</span></span>|<span data-ttu-id="a6c7f-129">Регистрация [ресурсов azureADDevice](../resources/windowsupdates-azureaddevice.md) в управлении обновлениями службой развертывания.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-129">Enroll [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources in update management by the deployment service.</span></span>|
|[<span data-ttu-id="a6c7f-130">Регистрация ресурсов azureADDevice в управлении (по ID)</span><span class="sxs-lookup"><span data-stu-id="a6c7f-130">Enroll azureADDevice resources in management (by ID)</span></span>](../api/windowsupdates-updatableasset-enrollassetsbyid.md)|<span data-ttu-id="a6c7f-131">Нет</span><span class="sxs-lookup"><span data-stu-id="a6c7f-131">None</span></span>|<span data-ttu-id="a6c7f-132">Регистрация [ресурсов azureADDevice](../resources/windowsupdates-azureaddevice.md) в управлении обновлениями службой развертывания.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-132">Enroll [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources in update management by the deployment service.</span></span>|
|[<span data-ttu-id="a6c7f-133">Unenroll azureADDevice resources from management</span><span class="sxs-lookup"><span data-stu-id="a6c7f-133">Unenroll azureADDevice resources from management</span></span>](../api/windowsupdates-updatableasset-unenrollassets.md)|<span data-ttu-id="a6c7f-134">Нет</span><span class="sxs-lookup"><span data-stu-id="a6c7f-134">None</span></span>|<span data-ttu-id="a6c7f-135">Unenroll [azureADDevice resources](../resources/windowsupdates-azureaddevice.md) from update management by the deployment service.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-135">Unenroll [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources from update management by the deployment service.</span></span>|
|[<span data-ttu-id="a6c7f-136">Unenroll azureADDevice resources from management (by ID)</span><span class="sxs-lookup"><span data-stu-id="a6c7f-136">Unenroll azureADDevice resources from management (by ID)</span></span>](../api/windowsupdates-updatableasset-unenrollassetsbyid.md)|<span data-ttu-id="a6c7f-137">Нет</span><span class="sxs-lookup"><span data-stu-id="a6c7f-137">None</span></span>|<span data-ttu-id="a6c7f-138">Unenroll [azureADDevice resources](../resources/windowsupdates-azureaddevice.md) from update management by the deployment service.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-138">Unenroll [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources from update management by the deployment service.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6c7f-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6c7f-139">Properties</span></span>
|<span data-ttu-id="a6c7f-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6c7f-140">Property</span></span>|<span data-ttu-id="a6c7f-141">Тип</span><span class="sxs-lookup"><span data-stu-id="a6c7f-141">Type</span></span>|<span data-ttu-id="a6c7f-142">Описание</span><span class="sxs-lookup"><span data-stu-id="a6c7f-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6c7f-143">регистрация</span><span class="sxs-lookup"><span data-stu-id="a6c7f-143">enrollments</span></span>|<span data-ttu-id="a6c7f-144">[коллекция microsoft.graph.windowsUpdates.updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md)</span><span class="sxs-lookup"><span data-stu-id="a6c7f-144">[microsoft.graph.windowsUpdates.updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md) collection</span></span>|<span data-ttu-id="a6c7f-145">Указывает области службы, в которую зачислилось устройство.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-145">Specifies areas of the service in which the device is enrolled.</span></span> <span data-ttu-id="a6c7f-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-146">Read-only.</span></span> <span data-ttu-id="a6c7f-147">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-147">Returned by default.</span></span>|
|<span data-ttu-id="a6c7f-148">ошибки</span><span class="sxs-lookup"><span data-stu-id="a6c7f-148">errors</span></span>|<span data-ttu-id="a6c7f-149">[коллекция microsoft.graph.windowsUpdates.updatableAssetError](../resources/windowsupdates-updatableasseterror.md)</span><span class="sxs-lookup"><span data-stu-id="a6c7f-149">[microsoft.graph.windowsUpdates.updatableAssetError](../resources/windowsupdates-updatableasseterror.md) collection</span></span>|<span data-ttu-id="a6c7f-150">Указывает все ошибки, которые мешают устройству быть зарегистрированным в управлении обновлениями или пересчете развернутого контента.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-150">Specifies any errors that prevent the device from being enrolled in update management or receving deployed content.</span></span> <span data-ttu-id="a6c7f-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-151">Read-only.</span></span> <span data-ttu-id="a6c7f-152">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-152">Returned by default.</span></span>|
|<span data-ttu-id="a6c7f-153">id</span><span class="sxs-lookup"><span data-stu-id="a6c7f-153">id</span></span>|<span data-ttu-id="a6c7f-154">String</span><span class="sxs-lookup"><span data-stu-id="a6c7f-154">String</span></span>|<span data-ttu-id="a6c7f-155">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-155">An identifier for the device.</span></span> <span data-ttu-id="a6c7f-156">Ключ.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-156">Key.</span></span> <span data-ttu-id="a6c7f-157">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-157">Not nullable.</span></span> <span data-ttu-id="a6c7f-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-158">Read-only.</span></span> <span data-ttu-id="a6c7f-159">Возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-159">Returned by default.</span></span> <span data-ttu-id="a6c7f-160">Унаследованный от [updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="a6c7f-160">Inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6c7f-161">Связи</span><span class="sxs-lookup"><span data-stu-id="a6c7f-161">Relationships</span></span>
<span data-ttu-id="a6c7f-162">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-162">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6c7f-163">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a6c7f-163">JSON representation</span></span>
<span data-ttu-id="a6c7f-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6c7f-164">The following is a JSON representation of the resource.</span></span>
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

