---
title: Тип ресурса Апплеусеринитиатеденроллментпрофиле
description: Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fb8e521826d0dc5123f86ad6fe99c098dfff8969
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080364"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a><span data-ttu-id="16d7a-104">Тип ресурса Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="16d7a-104">appleUserInitiatedEnrollmentProfile resource type</span></span>

<span data-ttu-id="16d7a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16d7a-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16d7a-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16d7a-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16d7a-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16d7a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16d7a-108">Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены.</span><span class="sxs-lookup"><span data-stu-id="16d7a-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="16d7a-109">Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.</span><span class="sxs-lookup"><span data-stu-id="16d7a-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="16d7a-110">Методы</span><span class="sxs-lookup"><span data-stu-id="16d7a-110">Methods</span></span>
|<span data-ttu-id="16d7a-111">Метод</span><span class="sxs-lookup"><span data-stu-id="16d7a-111">Method</span></span>|<span data-ttu-id="16d7a-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="16d7a-112">Return Type</span></span>|<span data-ttu-id="16d7a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="16d7a-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="16d7a-114">Список Апплеусеринитиатеденроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="16d7a-114">List appleUserInitiatedEnrollmentProfiles</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|<span data-ttu-id="16d7a-115">Коллекция [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-115">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) collection</span></span>|<span data-ttu-id="16d7a-116">Список свойств и связей объектов [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="16d7a-116">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="16d7a-117">Получение Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="16d7a-117">Get appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[<span data-ttu-id="16d7a-118">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="16d7a-118">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="16d7a-119">Чтение свойств и связей объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="16d7a-119">Read properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="16d7a-120">Создание Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="16d7a-120">Create appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[<span data-ttu-id="16d7a-121">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="16d7a-121">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="16d7a-122">Создание нового объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="16d7a-122">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="16d7a-123">Удаление Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="16d7a-123">Delete appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|<span data-ttu-id="16d7a-124">Нет</span><span class="sxs-lookup"><span data-stu-id="16d7a-124">None</span></span>|<span data-ttu-id="16d7a-125">Удаляет объект [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="16d7a-125">Deletes a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="16d7a-126">Обновление Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="16d7a-126">Update appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[<span data-ttu-id="16d7a-127">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="16d7a-127">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="16d7a-128">Обновление свойств объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="16d7a-128">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="16d7a-129">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="16d7a-129">setPriority action</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|<span data-ttu-id="16d7a-130">Нет</span><span class="sxs-lookup"><span data-stu-id="16d7a-130">None</span></span>|<span data-ttu-id="16d7a-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="16d7a-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="16d7a-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="16d7a-132">Properties</span></span>
|<span data-ttu-id="16d7a-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="16d7a-133">Property</span></span>|<span data-ttu-id="16d7a-134">Тип</span><span class="sxs-lookup"><span data-stu-id="16d7a-134">Type</span></span>|<span data-ttu-id="16d7a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="16d7a-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16d7a-136">дефаултенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="16d7a-136">defaultEnrollmentType</span></span>|[<span data-ttu-id="16d7a-137">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="16d7a-137">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="16d7a-138">Тип регистрации профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="16d7a-138">The default profile enrollment type.</span></span> <span data-ttu-id="16d7a-139">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="16d7a-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="16d7a-140">аваилаблинроллменттипеоптионс</span><span class="sxs-lookup"><span data-stu-id="16d7a-140">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="16d7a-141">Коллекция [апплеовнертипинроллменттипе](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-141">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="16d7a-142">Список доступных параметров типа регистрации</span><span class="sxs-lookup"><span data-stu-id="16d7a-142">List of available enrollment type options</span></span>|
|<span data-ttu-id="16d7a-143">id</span><span class="sxs-lookup"><span data-stu-id="16d7a-143">id</span></span>|<span data-ttu-id="16d7a-144">String</span><span class="sxs-lookup"><span data-stu-id="16d7a-144">String</span></span>|<span data-ttu-id="16d7a-145">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="16d7a-145">The GUID for the object</span></span>|
|<span data-ttu-id="16d7a-146">displayName</span><span class="sxs-lookup"><span data-stu-id="16d7a-146">displayName</span></span>|<span data-ttu-id="16d7a-147">String</span><span class="sxs-lookup"><span data-stu-id="16d7a-147">String</span></span>|<span data-ttu-id="16d7a-148">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="16d7a-148">Name of the profile</span></span>|
|<span data-ttu-id="16d7a-149">description</span><span class="sxs-lookup"><span data-stu-id="16d7a-149">description</span></span>|<span data-ttu-id="16d7a-150">String</span><span class="sxs-lookup"><span data-stu-id="16d7a-150">String</span></span>|<span data-ttu-id="16d7a-151">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="16d7a-151">Description of the profile</span></span>|
|<span data-ttu-id="16d7a-152">priority</span><span class="sxs-lookup"><span data-stu-id="16d7a-152">priority</span></span>|<span data-ttu-id="16d7a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="16d7a-153">Int32</span></span>|<span data-ttu-id="16d7a-154">Приоритет, 0 — самый высокий</span><span class="sxs-lookup"><span data-stu-id="16d7a-154">Priority, 0 is highest</span></span>|
|<span data-ttu-id="16d7a-155">платформа</span><span class="sxs-lookup"><span data-stu-id="16d7a-155">platform</span></span>|[<span data-ttu-id="16d7a-156">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="16d7a-156">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="16d7a-157">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="16d7a-157">The platform of the Device.</span></span> <span data-ttu-id="16d7a-158">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="16d7a-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="16d7a-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16d7a-159">createdDateTime</span></span>|<span data-ttu-id="16d7a-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16d7a-160">DateTimeOffset</span></span>|<span data-ttu-id="16d7a-161">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="16d7a-161">Profile creation time</span></span>|
|<span data-ttu-id="16d7a-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16d7a-162">lastModifiedDateTime</span></span>|<span data-ttu-id="16d7a-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16d7a-163">DateTimeOffset</span></span>|<span data-ttu-id="16d7a-164">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="16d7a-164">Profile last modified time</span></span>|

## <a name="relationships"></a><span data-ttu-id="16d7a-165">Отношения</span><span class="sxs-lookup"><span data-stu-id="16d7a-165">Relationships</span></span>
|<span data-ttu-id="16d7a-166">Связь</span><span class="sxs-lookup"><span data-stu-id="16d7a-166">Relationship</span></span>|<span data-ttu-id="16d7a-167">Тип</span><span class="sxs-lookup"><span data-stu-id="16d7a-167">Type</span></span>|<span data-ttu-id="16d7a-168">Описание</span><span class="sxs-lookup"><span data-stu-id="16d7a-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16d7a-169">assignments</span><span class="sxs-lookup"><span data-stu-id="16d7a-169">assignments</span></span>|<span data-ttu-id="16d7a-170">Коллекция [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="16d7a-170">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) collection</span></span>|<span data-ttu-id="16d7a-171">Список назначений для этого профиля.</span><span class="sxs-lookup"><span data-stu-id="16d7a-171">The list of assignments for this profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16d7a-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16d7a-172">JSON Representation</span></span>
<span data-ttu-id="16d7a-173">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16d7a-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleUserInitiatedEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "String",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "String",
      "enrollmentType": "String"
    }
  ],
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "platform": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```






