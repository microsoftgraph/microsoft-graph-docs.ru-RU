---
title: Тип ресурса importedDeviceIdentity
description: Ресурс importedDeviceIdentity представляет identity уникальный оборудования устройства, заранее подготовленных для конфигурации предварительной регистрации.
author: tfitzmac
ms.openlocfilehash: f7b6b054eab3815203a208382a19fbd9974cfb37
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350514"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="2ab79-103">Тип ресурса importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2ab79-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="2ab79-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2ab79-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ab79-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ab79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ab79-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2ab79-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ab79-107">Ресурс importedDeviceIdentity представляет identity уникальный оборудования устройства, заранее подготовленных для конфигурации предварительной регистрации.</span><span class="sxs-lookup"><span data-stu-id="2ab79-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="2ab79-108">Методы</span><span class="sxs-lookup"><span data-stu-id="2ab79-108">Methods</span></span>
|<span data-ttu-id="2ab79-109">Метод</span><span class="sxs-lookup"><span data-stu-id="2ab79-109">Method</span></span>|<span data-ttu-id="2ab79-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2ab79-110">Return Type</span></span>|<span data-ttu-id="2ab79-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2ab79-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ab79-112">Список importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="2ab79-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="2ab79-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="2ab79-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="2ab79-114">Свойства списка и связей объектов [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="2ab79-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="2ab79-115">Получение importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2ab79-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="2ab79-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2ab79-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="2ab79-117">Чтение свойства и связи объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="2ab79-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="2ab79-118">Создание importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2ab79-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="2ab79-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2ab79-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="2ab79-120">Создание нового объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="2ab79-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="2ab79-121">Удаление importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2ab79-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="2ab79-122">Нет</span><span class="sxs-lookup"><span data-stu-id="2ab79-122">None</span></span>|<span data-ttu-id="2ab79-123">Удаляет [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="2ab79-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="2ab79-124">Обновление importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2ab79-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="2ab79-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2ab79-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="2ab79-126">Обновление свойства объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="2ab79-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="2ab79-127">Действие importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="2ab79-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="2ab79-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="2ab79-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="2ab79-129">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2ab79-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2ab79-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ab79-130">Properties</span></span>
|<span data-ttu-id="2ab79-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ab79-131">Property</span></span>|<span data-ttu-id="2ab79-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2ab79-132">Type</span></span>|<span data-ttu-id="2ab79-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2ab79-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ab79-134">id</span><span class="sxs-lookup"><span data-stu-id="2ab79-134">id</span></span>|<span data-ttu-id="2ab79-135">Строка</span><span class="sxs-lookup"><span data-stu-id="2ab79-135">String</span></span>|<span data-ttu-id="2ab79-136">Идентификатор идентификатор импортированных устройства</span><span class="sxs-lookup"><span data-stu-id="2ab79-136">Id of the imported device identity</span></span>|
|<span data-ttu-id="2ab79-137">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="2ab79-137">importedDeviceIdentifier</span></span>|<span data-ttu-id="2ab79-138">String.</span><span class="sxs-lookup"><span data-stu-id="2ab79-138">String</span></span>|<span data-ttu-id="2ab79-139">Идентификатор импортированных устройства</span><span class="sxs-lookup"><span data-stu-id="2ab79-139">Imported Device Identifier</span></span>|
|<span data-ttu-id="2ab79-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="2ab79-140">importedDeviceIdentityType</span></span>|[<span data-ttu-id="2ab79-141">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="2ab79-141">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="2ab79-142">Тип удостоверения импортированных устройства.</span><span class="sxs-lookup"><span data-stu-id="2ab79-142">Type of Imported Device Identity.</span></span> <span data-ttu-id="2ab79-143">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="2ab79-143">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="2ab79-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ab79-144">lastModifiedDateTime</span></span>|<span data-ttu-id="2ab79-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ab79-145">DateTimeOffset</span></span>|<span data-ttu-id="2ab79-146">Последние изменения даты и времени описания</span><span class="sxs-lookup"><span data-stu-id="2ab79-146">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="2ab79-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ab79-147">createdDateTime</span></span>|<span data-ttu-id="2ab79-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ab79-148">DateTimeOffset</span></span>|<span data-ttu-id="2ab79-149">Время создания даты устройства</span><span class="sxs-lookup"><span data-stu-id="2ab79-149">Created Date Time of the device</span></span>|
|<span data-ttu-id="2ab79-150">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ab79-150">lastContactedDateTime</span></span>|<span data-ttu-id="2ab79-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ab79-151">DateTimeOffset</span></span>|<span data-ttu-id="2ab79-152">Связаться с даты последнего устройства</span><span class="sxs-lookup"><span data-stu-id="2ab79-152">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="2ab79-153">описание</span><span class="sxs-lookup"><span data-stu-id="2ab79-153">description</span></span>|<span data-ttu-id="2ab79-154">Строка</span><span class="sxs-lookup"><span data-stu-id="2ab79-154">String</span></span>|<span data-ttu-id="2ab79-155">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="2ab79-155">The description of the device</span></span>|
|<span data-ttu-id="2ab79-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2ab79-156">enrollmentState</span></span>|[<span data-ttu-id="2ab79-157">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2ab79-157">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="2ab79-158">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="2ab79-158">The state of the device in Intune.</span></span> <span data-ttu-id="2ab79-159">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="2ab79-159">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="2ab79-160">platform</span><span class="sxs-lookup"><span data-stu-id="2ab79-160">platform</span></span>|[<span data-ttu-id="2ab79-161">Платформа</span><span class="sxs-lookup"><span data-stu-id="2ab79-161">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="2ab79-162">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="2ab79-162">The platform of the Device.</span></span> <span data-ttu-id="2ab79-163">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="2ab79-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ab79-164">Связи</span><span class="sxs-lookup"><span data-stu-id="2ab79-164">Relationships</span></span>
<span data-ttu-id="2ab79-165">Нет</span><span class="sxs-lookup"><span data-stu-id="2ab79-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2ab79-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ab79-166">JSON Representation</span></span>
<span data-ttu-id="2ab79-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ab79-167">Here is a JSON representation of the resource.</span></span>
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





