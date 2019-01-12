---
title: Тип ресурса deviceInstallState
description: Содержит свойства состояния установки для устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1b495bc41590ada44a9986dd9cc9cb262bcc68b6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959890"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="d6543-103">Тип ресурса deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="d6543-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="d6543-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d6543-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6543-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6543-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6543-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d6543-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6543-107">Содержит свойства состояния установки для устройства.</span><span class="sxs-lookup"><span data-stu-id="d6543-107">Contains properties for the installation state for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="d6543-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d6543-108">Methods</span></span>
|<span data-ttu-id="d6543-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d6543-109">Method</span></span>|<span data-ttu-id="d6543-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d6543-110">Return Type</span></span>|<span data-ttu-id="d6543-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d6543-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d6543-112">Список объектов deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="d6543-112">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="d6543-113">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="d6543-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="d6543-114">Список свойств и связей объектов [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="d6543-114">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="d6543-115">Получение объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="d6543-115">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="d6543-116">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="d6543-116">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="d6543-117">Чтение свойств и связей объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="d6543-117">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="d6543-118">Создание объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="d6543-118">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="d6543-119">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="d6543-119">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="d6543-120">Создание объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="d6543-120">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="d6543-121">Удаление объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="d6543-121">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="d6543-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d6543-122">None</span></span>|<span data-ttu-id="d6543-123">Удаляет объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="d6543-123">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="d6543-124">Обновление объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="d6543-124">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="d6543-125">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="d6543-125">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="d6543-126">Обновление свойств объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="d6543-126">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d6543-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6543-127">Properties</span></span>
|<span data-ttu-id="d6543-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6543-128">Property</span></span>|<span data-ttu-id="d6543-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d6543-129">Type</span></span>|<span data-ttu-id="d6543-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d6543-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6543-131">id</span><span class="sxs-lookup"><span data-stu-id="d6543-131">id</span></span>|<span data-ttu-id="d6543-132">Строка</span><span class="sxs-lookup"><span data-stu-id="d6543-132">String</span></span>|<span data-ttu-id="d6543-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d6543-133">Key of the entity.</span></span>|
|<span data-ttu-id="d6543-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="d6543-134">deviceName</span></span>|<span data-ttu-id="d6543-135">String</span><span class="sxs-lookup"><span data-stu-id="d6543-135">String</span></span>|<span data-ttu-id="d6543-136">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="d6543-136">Device name.</span></span>|
|<span data-ttu-id="d6543-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="d6543-137">deviceId</span></span>|<span data-ttu-id="d6543-138">String</span><span class="sxs-lookup"><span data-stu-id="d6543-138">String</span></span>|<span data-ttu-id="d6543-139">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="d6543-139">Device Id.</span></span>|
|<span data-ttu-id="d6543-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d6543-140">lastSyncDateTime</span></span>|<span data-ttu-id="d6543-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6543-141">DateTimeOffset</span></span>|<span data-ttu-id="d6543-142">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d6543-142">Last sync date and time.</span></span>|
|<span data-ttu-id="d6543-143">installState</span><span class="sxs-lookup"><span data-stu-id="d6543-143">installState</span></span>|[<span data-ttu-id="d6543-144">installState</span><span class="sxs-lookup"><span data-stu-id="d6543-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="d6543-145">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="d6543-145">The install state of the eBook.</span></span> <span data-ttu-id="d6543-146">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d6543-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="d6543-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="d6543-147">errorCode</span></span>|<span data-ttu-id="d6543-148">String</span><span class="sxs-lookup"><span data-stu-id="d6543-148">String</span></span>|<span data-ttu-id="d6543-149">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="d6543-149">The error code for install failures.</span></span>|
|<span data-ttu-id="d6543-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="d6543-150">osVersion</span></span>|<span data-ttu-id="d6543-151">String</span><span class="sxs-lookup"><span data-stu-id="d6543-151">String</span></span>|<span data-ttu-id="d6543-152">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="d6543-152">OS Version.</span></span>|
|<span data-ttu-id="d6543-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="d6543-153">osDescription</span></span>|<span data-ttu-id="d6543-154">String</span><span class="sxs-lookup"><span data-stu-id="d6543-154">String</span></span>|<span data-ttu-id="d6543-155">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="d6543-155">OS Description.</span></span>|
|<span data-ttu-id="d6543-156">userName</span><span class="sxs-lookup"><span data-stu-id="d6543-156">userName</span></span>|<span data-ttu-id="d6543-157">String</span><span class="sxs-lookup"><span data-stu-id="d6543-157">String</span></span>|<span data-ttu-id="d6543-158">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="d6543-158">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6543-159">Связи</span><span class="sxs-lookup"><span data-stu-id="d6543-159">Relationships</span></span>
<span data-ttu-id="d6543-160">Нет</span><span class="sxs-lookup"><span data-stu-id="d6543-160">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6543-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6543-161">JSON Representation</span></span>
<span data-ttu-id="d6543-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6543-162">Here is a JSON representation of the resource.</span></span>
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





