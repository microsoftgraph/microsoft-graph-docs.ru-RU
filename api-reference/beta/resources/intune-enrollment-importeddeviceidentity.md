---
title: Тип ресурса Импортеддевицеидентити
description: Ресурс Импортеддевицеидентити представляет уникальное аппаратное удостоверение устройства, которое было предварительно подготовлено для настройки предварительной регистрации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7ef77b550060d5544a6ee0eda4e6b11923d3571
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151228"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="01d3d-103">Тип ресурса Импортеддевицеидентити</span><span class="sxs-lookup"><span data-stu-id="01d3d-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="01d3d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01d3d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01d3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01d3d-106">Ресурс Импортеддевицеидентити представляет уникальное аппаратное удостоверение устройства, которое было предварительно подготовлено для настройки предварительной регистрации.</span><span class="sxs-lookup"><span data-stu-id="01d3d-106">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="01d3d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="01d3d-107">Methods</span></span>
|<span data-ttu-id="01d3d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="01d3d-108">Method</span></span>|<span data-ttu-id="01d3d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="01d3d-109">Return Type</span></span>|<span data-ttu-id="01d3d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="01d3d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="01d3d-111">Список Импортеддевицеидентитиес</span><span class="sxs-lookup"><span data-stu-id="01d3d-111">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="01d3d-112">Коллекция [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="01d3d-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="01d3d-113">Список свойств и связей объектов [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="01d3d-113">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="01d3d-114">Получение Импортеддевицеидентити</span><span class="sxs-lookup"><span data-stu-id="01d3d-114">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="01d3d-115">Импортеддевицеидентити</span><span class="sxs-lookup"><span data-stu-id="01d3d-115">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="01d3d-116">Чтение свойств и связей объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="01d3d-116">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="01d3d-117">Создание Импортеддевицеидентити</span><span class="sxs-lookup"><span data-stu-id="01d3d-117">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="01d3d-118">Импортеддевицеидентити</span><span class="sxs-lookup"><span data-stu-id="01d3d-118">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="01d3d-119">Создание нового объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="01d3d-119">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="01d3d-120">Удаление Импортеддевицеидентити</span><span class="sxs-lookup"><span data-stu-id="01d3d-120">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="01d3d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="01d3d-121">None</span></span>|<span data-ttu-id="01d3d-122">Удаляет объект [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="01d3d-122">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="01d3d-123">Обновление Импортеддевицеидентити</span><span class="sxs-lookup"><span data-stu-id="01d3d-123">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="01d3d-124">Импортеддевицеидентити</span><span class="sxs-lookup"><span data-stu-id="01d3d-124">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="01d3d-125">Обновление свойств объекта [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="01d3d-125">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="01d3d-126">Действие importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="01d3d-126">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="01d3d-127">Коллекция [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md)</span><span class="sxs-lookup"><span data-stu-id="01d3d-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="01d3d-128">Н/Д</span><span class="sxs-lookup"><span data-stu-id="01d3d-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="01d3d-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="01d3d-129">Properties</span></span>
|<span data-ttu-id="01d3d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="01d3d-130">Property</span></span>|<span data-ttu-id="01d3d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="01d3d-131">Type</span></span>|<span data-ttu-id="01d3d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="01d3d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01d3d-133">id</span><span class="sxs-lookup"><span data-stu-id="01d3d-133">id</span></span>|<span data-ttu-id="01d3d-134">String</span><span class="sxs-lookup"><span data-stu-id="01d3d-134">String</span></span>|<span data-ttu-id="01d3d-135">Идентификатор импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="01d3d-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="01d3d-136">Импортеддевицеидентифиер</span><span class="sxs-lookup"><span data-stu-id="01d3d-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="01d3d-137">String</span><span class="sxs-lookup"><span data-stu-id="01d3d-137">String</span></span>|<span data-ttu-id="01d3d-138">Импортированный идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="01d3d-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="01d3d-139">Импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="01d3d-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="01d3d-140">Импортеддевицеидентититипе</span><span class="sxs-lookup"><span data-stu-id="01d3d-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="01d3d-141">Тип импортированного удостоверения устройства.</span><span class="sxs-lookup"><span data-stu-id="01d3d-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="01d3d-142">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="01d3d-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="01d3d-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01d3d-143">lastModifiedDateTime</span></span>|<span data-ttu-id="01d3d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d3d-144">DateTimeOffset</span></span>|<span data-ttu-id="01d3d-145">Дата и время последнего изменения описания</span><span class="sxs-lookup"><span data-stu-id="01d3d-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="01d3d-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01d3d-146">createdDateTime</span></span>|<span data-ttu-id="01d3d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d3d-147">DateTimeOffset</span></span>|<span data-ttu-id="01d3d-148">Дата и время создания устройства</span><span class="sxs-lookup"><span data-stu-id="01d3d-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="01d3d-149">Ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="01d3d-149">lastContactedDateTime</span></span>|<span data-ttu-id="01d3d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d3d-150">DateTimeOffset</span></span>|<span data-ttu-id="01d3d-151">Дата и время последнего обращения к устройству</span><span class="sxs-lookup"><span data-stu-id="01d3d-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="01d3d-152">description</span><span class="sxs-lookup"><span data-stu-id="01d3d-152">description</span></span>|<span data-ttu-id="01d3d-153">String</span><span class="sxs-lookup"><span data-stu-id="01d3d-153">String</span></span>|<span data-ttu-id="01d3d-154">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="01d3d-154">The description of the device</span></span>|
|<span data-ttu-id="01d3d-155">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="01d3d-155">enrollmentState</span></span>|[<span data-ttu-id="01d3d-156">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="01d3d-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="01d3d-157">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="01d3d-157">The state of the device in Intune.</span></span> <span data-ttu-id="01d3d-158">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="01d3d-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="01d3d-159">platform</span><span class="sxs-lookup"><span data-stu-id="01d3d-159">platform</span></span>|[<span data-ttu-id="01d3d-160">управляем</span><span class="sxs-lookup"><span data-stu-id="01d3d-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="01d3d-161">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="01d3d-161">The platform of the Device.</span></span> <span data-ttu-id="01d3d-162">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="01d3d-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01d3d-163">Отношения</span><span class="sxs-lookup"><span data-stu-id="01d3d-163">Relationships</span></span>
<span data-ttu-id="01d3d-164">Нет</span><span class="sxs-lookup"><span data-stu-id="01d3d-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01d3d-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01d3d-165">JSON Representation</span></span>
<span data-ttu-id="01d3d-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01d3d-166">Here is a JSON representation of the resource.</span></span>
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




