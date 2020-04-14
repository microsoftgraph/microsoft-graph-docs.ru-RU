---
title: Тип ресурса deviceInstallState
description: Содержит свойства состояния установки для устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dab43efe955dfbcbe4a7f7e2f028fac0c0ec48ca
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441200"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="bd8de-103">Тип ресурса deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="bd8de-103">deviceInstallState resource type</span></span>

<span data-ttu-id="bd8de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd8de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd8de-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd8de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd8de-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd8de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd8de-107">Содержит свойства состояния установки для устройства.</span><span class="sxs-lookup"><span data-stu-id="bd8de-107">Contains properties for the installation state for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="bd8de-108">Методы</span><span class="sxs-lookup"><span data-stu-id="bd8de-108">Methods</span></span>
|<span data-ttu-id="bd8de-109">Метод</span><span class="sxs-lookup"><span data-stu-id="bd8de-109">Method</span></span>|<span data-ttu-id="bd8de-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bd8de-110">Return Type</span></span>|<span data-ttu-id="bd8de-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bd8de-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bd8de-112">Список объектов deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="bd8de-112">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="bd8de-113">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="bd8de-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="bd8de-114">Список свойств и связей объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="bd8de-114">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="bd8de-115">Получение объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="bd8de-115">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|<span data-ttu-id="bd8de-116">[deviceInstallState](../resources/intune-books-deviceinstallstate.md);</span><span class="sxs-lookup"><span data-stu-id="bd8de-116">[deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span></span>|<span data-ttu-id="bd8de-117">Чтение свойств и связей объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="bd8de-117">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="bd8de-118">Создание объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="bd8de-118">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|<span data-ttu-id="bd8de-119">[deviceInstallState](../resources/intune-books-deviceinstallstate.md);</span><span class="sxs-lookup"><span data-stu-id="bd8de-119">[deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span></span>|<span data-ttu-id="bd8de-120">Создание объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="bd8de-120">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="bd8de-121">Удаление объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="bd8de-121">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="bd8de-122">Нет</span><span class="sxs-lookup"><span data-stu-id="bd8de-122">None</span></span>|<span data-ttu-id="bd8de-123">Удаляет объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="bd8de-123">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="bd8de-124">Обновление объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="bd8de-124">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="bd8de-125">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="bd8de-125">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="bd8de-126">Обновление свойств объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="bd8de-126">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bd8de-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd8de-127">Properties</span></span>
|<span data-ttu-id="bd8de-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd8de-128">Property</span></span>|<span data-ttu-id="bd8de-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bd8de-129">Type</span></span>|<span data-ttu-id="bd8de-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bd8de-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd8de-131">id</span><span class="sxs-lookup"><span data-stu-id="bd8de-131">id</span></span>|<span data-ttu-id="bd8de-132">String</span><span class="sxs-lookup"><span data-stu-id="bd8de-132">String</span></span>|<span data-ttu-id="bd8de-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bd8de-133">Key of the entity.</span></span>|
|<span data-ttu-id="bd8de-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="bd8de-134">deviceName</span></span>|<span data-ttu-id="bd8de-135">String</span><span class="sxs-lookup"><span data-stu-id="bd8de-135">String</span></span>|<span data-ttu-id="bd8de-136">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="bd8de-136">Device name.</span></span>|
|<span data-ttu-id="bd8de-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="bd8de-137">deviceId</span></span>|<span data-ttu-id="bd8de-138">String</span><span class="sxs-lookup"><span data-stu-id="bd8de-138">String</span></span>|<span data-ttu-id="bd8de-139">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="bd8de-139">Device Id.</span></span>|
|<span data-ttu-id="bd8de-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bd8de-140">lastSyncDateTime</span></span>|<span data-ttu-id="bd8de-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd8de-141">DateTimeOffset</span></span>|<span data-ttu-id="bd8de-142">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bd8de-142">Last sync date and time.</span></span>|
|<span data-ttu-id="bd8de-143">installState</span><span class="sxs-lookup"><span data-stu-id="bd8de-143">installState</span></span>|[<span data-ttu-id="bd8de-144">installState</span><span class="sxs-lookup"><span data-stu-id="bd8de-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="bd8de-145">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="bd8de-145">The install state of the eBook.</span></span> <span data-ttu-id="bd8de-146">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="bd8de-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="bd8de-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="bd8de-147">errorCode</span></span>|<span data-ttu-id="bd8de-148">String</span><span class="sxs-lookup"><span data-stu-id="bd8de-148">String</span></span>|<span data-ttu-id="bd8de-149">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="bd8de-149">The error code for install failures.</span></span>|
|<span data-ttu-id="bd8de-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="bd8de-150">osVersion</span></span>|<span data-ttu-id="bd8de-151">String</span><span class="sxs-lookup"><span data-stu-id="bd8de-151">String</span></span>|<span data-ttu-id="bd8de-152">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="bd8de-152">OS Version.</span></span>|
|<span data-ttu-id="bd8de-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="bd8de-153">osDescription</span></span>|<span data-ttu-id="bd8de-154">String</span><span class="sxs-lookup"><span data-stu-id="bd8de-154">String</span></span>|<span data-ttu-id="bd8de-155">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="bd8de-155">OS Description.</span></span>|
|<span data-ttu-id="bd8de-156">userName</span><span class="sxs-lookup"><span data-stu-id="bd8de-156">userName</span></span>|<span data-ttu-id="bd8de-157">String</span><span class="sxs-lookup"><span data-stu-id="bd8de-157">String</span></span>|<span data-ttu-id="bd8de-158">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="bd8de-158">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd8de-159">Связи</span><span class="sxs-lookup"><span data-stu-id="bd8de-159">Relationships</span></span>
<span data-ttu-id="bd8de-160">Нет</span><span class="sxs-lookup"><span data-stu-id="bd8de-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd8de-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd8de-161">JSON Representation</span></span>
<span data-ttu-id="bd8de-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd8de-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```



