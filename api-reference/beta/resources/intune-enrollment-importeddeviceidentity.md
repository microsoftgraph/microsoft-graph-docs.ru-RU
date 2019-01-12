---
title: Тип ресурса importedDeviceIdentity
description: Ресурс importedDeviceIdentity представляет identity уникальный оборудования устройства, заранее подготовленных для конфигурации предварительной регистрации.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6fe03159f79bb1198db80cbba130601614df8865
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966568"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="2c828-103">Тип ресурса importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2c828-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="2c828-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2c828-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c828-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c828-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c828-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2c828-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c828-107">Ресурс importedDeviceIdentity представляет identity уникальный оборудования устройства, заранее подготовленных для конфигурации предварительной регистрации.</span><span class="sxs-lookup"><span data-stu-id="2c828-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="2c828-108">Методы</span><span class="sxs-lookup"><span data-stu-id="2c828-108">Methods</span></span>
|<span data-ttu-id="2c828-109">Метод</span><span class="sxs-lookup"><span data-stu-id="2c828-109">Method</span></span>|<span data-ttu-id="2c828-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2c828-110">Return Type</span></span>|<span data-ttu-id="2c828-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2c828-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2c828-112">Список importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="2c828-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="2c828-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="2c828-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="2c828-114">Свойства списка и связей объектов [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="2c828-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="2c828-115">Получение importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2c828-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="2c828-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2c828-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="2c828-117">Чтение свойства и связи объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="2c828-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="2c828-118">Создание importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2c828-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="2c828-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2c828-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="2c828-120">Создание нового объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="2c828-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="2c828-121">Удаление importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2c828-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="2c828-122">Нет</span><span class="sxs-lookup"><span data-stu-id="2c828-122">None</span></span>|<span data-ttu-id="2c828-123">Удаляет [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="2c828-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="2c828-124">Обновление importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2c828-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="2c828-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2c828-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="2c828-126">Обновление свойства объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="2c828-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="2c828-127">Действие importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="2c828-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="2c828-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="2c828-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="2c828-129">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2c828-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2c828-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c828-130">Properties</span></span>
|<span data-ttu-id="2c828-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c828-131">Property</span></span>|<span data-ttu-id="2c828-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2c828-132">Type</span></span>|<span data-ttu-id="2c828-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2c828-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c828-134">id</span><span class="sxs-lookup"><span data-stu-id="2c828-134">id</span></span>|<span data-ttu-id="2c828-135">String</span><span class="sxs-lookup"><span data-stu-id="2c828-135">String</span></span>|<span data-ttu-id="2c828-136">Идентификатор идентификатор импортированных устройства</span><span class="sxs-lookup"><span data-stu-id="2c828-136">Id of the imported device identity</span></span>|
|<span data-ttu-id="2c828-137">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="2c828-137">importedDeviceIdentifier</span></span>|<span data-ttu-id="2c828-138">String</span><span class="sxs-lookup"><span data-stu-id="2c828-138">String</span></span>|<span data-ttu-id="2c828-139">Идентификатор импортированных устройства</span><span class="sxs-lookup"><span data-stu-id="2c828-139">Imported Device Identifier</span></span>|
|<span data-ttu-id="2c828-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="2c828-140">importedDeviceIdentityType</span></span>|[<span data-ttu-id="2c828-141">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="2c828-141">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="2c828-142">Тип удостоверения импортированных устройства.</span><span class="sxs-lookup"><span data-stu-id="2c828-142">Type of Imported Device Identity.</span></span> <span data-ttu-id="2c828-143">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="2c828-143">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="2c828-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c828-144">lastModifiedDateTime</span></span>|<span data-ttu-id="2c828-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c828-145">DateTimeOffset</span></span>|<span data-ttu-id="2c828-146">Последние изменения даты и времени описания</span><span class="sxs-lookup"><span data-stu-id="2c828-146">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="2c828-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c828-147">createdDateTime</span></span>|<span data-ttu-id="2c828-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c828-148">DateTimeOffset</span></span>|<span data-ttu-id="2c828-149">Время создания даты устройства</span><span class="sxs-lookup"><span data-stu-id="2c828-149">Created Date Time of the device</span></span>|
|<span data-ttu-id="2c828-150">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c828-150">lastContactedDateTime</span></span>|<span data-ttu-id="2c828-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c828-151">DateTimeOffset</span></span>|<span data-ttu-id="2c828-152">Связаться с даты последнего устройства</span><span class="sxs-lookup"><span data-stu-id="2c828-152">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="2c828-153">описание</span><span class="sxs-lookup"><span data-stu-id="2c828-153">description</span></span>|<span data-ttu-id="2c828-154">String</span><span class="sxs-lookup"><span data-stu-id="2c828-154">String</span></span>|<span data-ttu-id="2c828-155">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="2c828-155">The description of the device</span></span>|
|<span data-ttu-id="2c828-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2c828-156">enrollmentState</span></span>|[<span data-ttu-id="2c828-157">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2c828-157">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="2c828-158">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="2c828-158">The state of the device in Intune.</span></span> <span data-ttu-id="2c828-159">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="2c828-159">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="2c828-160">platform</span><span class="sxs-lookup"><span data-stu-id="2c828-160">platform</span></span>|[<span data-ttu-id="2c828-161">Платформа</span><span class="sxs-lookup"><span data-stu-id="2c828-161">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="2c828-162">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="2c828-162">The platform of the Device.</span></span> <span data-ttu-id="2c828-163">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="2c828-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c828-164">Связи</span><span class="sxs-lookup"><span data-stu-id="2c828-164">Relationships</span></span>
<span data-ttu-id="2c828-165">Нет</span><span class="sxs-lookup"><span data-stu-id="2c828-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2c828-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c828-166">JSON Representation</span></span>
<span data-ttu-id="2c828-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c828-167">Here is a JSON representation of the resource.</span></span>
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





