---
title: Тип ресурса importedDeviceIdentity
description: Ресурс importedDeviceIdentity представляет identity уникальный оборудования устройства, заранее подготовленных для конфигурации предварительной регистрации.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c151257a95d1161e07de17ed6d9fc01fc021146e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421447"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="a8e83-103">Тип ресурса importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a8e83-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="a8e83-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8e83-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a8e83-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8e83-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8e83-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8e83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8e83-107">Ресурс importedDeviceIdentity представляет identity уникальный оборудования устройства, заранее подготовленных для конфигурации предварительной регистрации.</span><span class="sxs-lookup"><span data-stu-id="a8e83-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="a8e83-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a8e83-108">Methods</span></span>
|<span data-ttu-id="a8e83-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a8e83-109">Method</span></span>|<span data-ttu-id="a8e83-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a8e83-110">Return Type</span></span>|<span data-ttu-id="a8e83-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a8e83-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a8e83-112">Список importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="a8e83-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="a8e83-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a8e83-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="a8e83-114">Свойства списка и связей объектов [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="a8e83-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="a8e83-115">Получение importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a8e83-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="a8e83-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a8e83-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="a8e83-117">Чтение свойства и связи объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="a8e83-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="a8e83-118">Создание importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a8e83-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="a8e83-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a8e83-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="a8e83-120">Создание нового объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="a8e83-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="a8e83-121">Удаление importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a8e83-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="a8e83-122">Нет</span><span class="sxs-lookup"><span data-stu-id="a8e83-122">None</span></span>|<span data-ttu-id="a8e83-123">Удаляет [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="a8e83-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="a8e83-124">Обновление importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a8e83-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="a8e83-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a8e83-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="a8e83-126">Обновление свойства объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="a8e83-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="a8e83-127">Действие importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="a8e83-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="a8e83-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a8e83-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="a8e83-129">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a8e83-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a8e83-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8e83-130">Properties</span></span>
|<span data-ttu-id="a8e83-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8e83-131">Property</span></span>|<span data-ttu-id="a8e83-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a8e83-132">Type</span></span>|<span data-ttu-id="a8e83-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a8e83-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8e83-134">id</span><span class="sxs-lookup"><span data-stu-id="a8e83-134">id</span></span>|<span data-ttu-id="a8e83-135">String</span><span class="sxs-lookup"><span data-stu-id="a8e83-135">String</span></span>|<span data-ttu-id="a8e83-136">Идентификатор идентификатор импортированных устройства</span><span class="sxs-lookup"><span data-stu-id="a8e83-136">Id of the imported device identity</span></span>|
|<span data-ttu-id="a8e83-137">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a8e83-137">importedDeviceIdentifier</span></span>|<span data-ttu-id="a8e83-138">String</span><span class="sxs-lookup"><span data-stu-id="a8e83-138">String</span></span>|<span data-ttu-id="a8e83-139">Идентификатор импортированных устройства</span><span class="sxs-lookup"><span data-stu-id="a8e83-139">Imported Device Identifier</span></span>|
|<span data-ttu-id="a8e83-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="a8e83-140">importedDeviceIdentityType</span></span>|[<span data-ttu-id="a8e83-141">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="a8e83-141">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="a8e83-142">Тип удостоверения импортированных устройства.</span><span class="sxs-lookup"><span data-stu-id="a8e83-142">Type of Imported Device Identity.</span></span> <span data-ttu-id="a8e83-143">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="a8e83-143">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="a8e83-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8e83-144">lastModifiedDateTime</span></span>|<span data-ttu-id="a8e83-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8e83-145">DateTimeOffset</span></span>|<span data-ttu-id="a8e83-146">Последние изменения даты и времени описания</span><span class="sxs-lookup"><span data-stu-id="a8e83-146">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="a8e83-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8e83-147">createdDateTime</span></span>|<span data-ttu-id="a8e83-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8e83-148">DateTimeOffset</span></span>|<span data-ttu-id="a8e83-149">Время создания даты устройства</span><span class="sxs-lookup"><span data-stu-id="a8e83-149">Created Date Time of the device</span></span>|
|<span data-ttu-id="a8e83-150">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8e83-150">lastContactedDateTime</span></span>|<span data-ttu-id="a8e83-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8e83-151">DateTimeOffset</span></span>|<span data-ttu-id="a8e83-152">Связаться с даты последнего устройства</span><span class="sxs-lookup"><span data-stu-id="a8e83-152">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="a8e83-153">description</span><span class="sxs-lookup"><span data-stu-id="a8e83-153">description</span></span>|<span data-ttu-id="a8e83-154">String</span><span class="sxs-lookup"><span data-stu-id="a8e83-154">String</span></span>|<span data-ttu-id="a8e83-155">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="a8e83-155">The description of the device</span></span>|
|<span data-ttu-id="a8e83-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="a8e83-156">enrollmentState</span></span>|[<span data-ttu-id="a8e83-157">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="a8e83-157">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="a8e83-158">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="a8e83-158">The state of the device in Intune.</span></span> <span data-ttu-id="a8e83-159">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="a8e83-159">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="a8e83-160">platform</span><span class="sxs-lookup"><span data-stu-id="a8e83-160">platform</span></span>|[<span data-ttu-id="a8e83-161">Платформа</span><span class="sxs-lookup"><span data-stu-id="a8e83-161">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="a8e83-162">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="a8e83-162">The platform of the Device.</span></span> <span data-ttu-id="a8e83-163">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="a8e83-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8e83-164">Отношения</span><span class="sxs-lookup"><span data-stu-id="a8e83-164">Relationships</span></span>
<span data-ttu-id="a8e83-165">Нет</span><span class="sxs-lookup"><span data-stu-id="a8e83-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8e83-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8e83-166">JSON Representation</span></span>
<span data-ttu-id="a8e83-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8e83-167">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```




