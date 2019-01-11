---
title: Тип ресурса importedDeviceIdentity
description: Ресурс importedDeviceIdentity представляет identity уникальный оборудования устройства, заранее подготовленных для конфигурации предварительной регистрации.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3c33069520913c7c750220ca8938459ba9bf96c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811671"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="f7697-103">Тип ресурса importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f7697-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="f7697-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f7697-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7697-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7697-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7697-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f7697-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7697-107">Ресурс importedDeviceIdentity представляет identity уникальный оборудования устройства, заранее подготовленных для конфигурации предварительной регистрации.</span><span class="sxs-lookup"><span data-stu-id="f7697-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="f7697-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f7697-108">Methods</span></span>
|<span data-ttu-id="f7697-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f7697-109">Method</span></span>|<span data-ttu-id="f7697-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f7697-110">Return Type</span></span>|<span data-ttu-id="f7697-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f7697-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f7697-112">Список importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="f7697-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="f7697-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f7697-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="f7697-114">Свойства списка и связей объектов [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="f7697-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="f7697-115">Получение importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f7697-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="f7697-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f7697-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="f7697-117">Чтение свойства и связи объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="f7697-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="f7697-118">Создание importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f7697-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="f7697-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f7697-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="f7697-120">Создание нового объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="f7697-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="f7697-121">Удаление importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f7697-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="f7697-122">Нет</span><span class="sxs-lookup"><span data-stu-id="f7697-122">None</span></span>|<span data-ttu-id="f7697-123">Удаляет [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="f7697-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="f7697-124">Обновление importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f7697-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="f7697-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f7697-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="f7697-126">Обновление свойства объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="f7697-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="f7697-127">Действие importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="f7697-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="f7697-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f7697-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="f7697-129">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f7697-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f7697-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7697-130">Properties</span></span>
|<span data-ttu-id="f7697-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7697-131">Property</span></span>|<span data-ttu-id="f7697-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f7697-132">Type</span></span>|<span data-ttu-id="f7697-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f7697-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7697-134">id</span><span class="sxs-lookup"><span data-stu-id="f7697-134">id</span></span>|<span data-ttu-id="f7697-135">Строка</span><span class="sxs-lookup"><span data-stu-id="f7697-135">String</span></span>|<span data-ttu-id="f7697-136">Идентификатор идентификатор импортированных устройства</span><span class="sxs-lookup"><span data-stu-id="f7697-136">Id of the imported device identity</span></span>|
|<span data-ttu-id="f7697-137">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f7697-137">importedDeviceIdentifier</span></span>|<span data-ttu-id="f7697-138">Строка</span><span class="sxs-lookup"><span data-stu-id="f7697-138">String</span></span>|<span data-ttu-id="f7697-139">Идентификатор импортированных устройства</span><span class="sxs-lookup"><span data-stu-id="f7697-139">Imported Device Identifier</span></span>|
|<span data-ttu-id="f7697-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="f7697-140">importedDeviceIdentityType</span></span>|[<span data-ttu-id="f7697-141">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="f7697-141">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="f7697-142">Тип удостоверения импортированных устройства.</span><span class="sxs-lookup"><span data-stu-id="f7697-142">Type of Imported Device Identity.</span></span> <span data-ttu-id="f7697-143">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="f7697-143">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="f7697-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7697-144">lastModifiedDateTime</span></span>|<span data-ttu-id="f7697-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7697-145">DateTimeOffset</span></span>|<span data-ttu-id="f7697-146">Последние изменения даты и времени описания</span><span class="sxs-lookup"><span data-stu-id="f7697-146">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="f7697-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7697-147">createdDateTime</span></span>|<span data-ttu-id="f7697-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7697-148">DateTimeOffset</span></span>|<span data-ttu-id="f7697-149">Время создания даты устройства</span><span class="sxs-lookup"><span data-stu-id="f7697-149">Created Date Time of the device</span></span>|
|<span data-ttu-id="f7697-150">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7697-150">lastContactedDateTime</span></span>|<span data-ttu-id="f7697-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7697-151">DateTimeOffset</span></span>|<span data-ttu-id="f7697-152">Связаться с даты последнего устройства</span><span class="sxs-lookup"><span data-stu-id="f7697-152">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="f7697-153">описание</span><span class="sxs-lookup"><span data-stu-id="f7697-153">description</span></span>|<span data-ttu-id="f7697-154">Строка</span><span class="sxs-lookup"><span data-stu-id="f7697-154">String</span></span>|<span data-ttu-id="f7697-155">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="f7697-155">The description of the device</span></span>|
|<span data-ttu-id="f7697-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="f7697-156">enrollmentState</span></span>|[<span data-ttu-id="f7697-157">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="f7697-157">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="f7697-158">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="f7697-158">The state of the device in Intune.</span></span> <span data-ttu-id="f7697-159">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="f7697-159">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="f7697-160">platform</span><span class="sxs-lookup"><span data-stu-id="f7697-160">platform</span></span>|[<span data-ttu-id="f7697-161">Платформа</span><span class="sxs-lookup"><span data-stu-id="f7697-161">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="f7697-162">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="f7697-162">The platform of the Device.</span></span> <span data-ttu-id="f7697-163">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="f7697-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7697-164">Связи</span><span class="sxs-lookup"><span data-stu-id="f7697-164">Relationships</span></span>
<span data-ttu-id="f7697-165">Нет</span><span class="sxs-lookup"><span data-stu-id="f7697-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f7697-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7697-166">JSON Representation</span></span>
<span data-ttu-id="f7697-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7697-167">Here is a JSON representation of the resource.</span></span>
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





