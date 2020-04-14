---
title: Тип ресурса Апплеусеринитиатеденроллментпрофиле
description: Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f6f7d28d1c5684793891bc8bee08300f67ebeec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419482"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a><span data-ttu-id="24cb8-104">Тип ресурса Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="24cb8-104">appleUserInitiatedEnrollmentProfile resource type</span></span>

<span data-ttu-id="24cb8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24cb8-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24cb8-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24cb8-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24cb8-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24cb8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24cb8-108">Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены.</span><span class="sxs-lookup"><span data-stu-id="24cb8-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="24cb8-109">Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.</span><span class="sxs-lookup"><span data-stu-id="24cb8-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="24cb8-110">Методы</span><span class="sxs-lookup"><span data-stu-id="24cb8-110">Methods</span></span>
|<span data-ttu-id="24cb8-111">Метод</span><span class="sxs-lookup"><span data-stu-id="24cb8-111">Method</span></span>|<span data-ttu-id="24cb8-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="24cb8-112">Return Type</span></span>|<span data-ttu-id="24cb8-113">Описание</span><span class="sxs-lookup"><span data-stu-id="24cb8-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="24cb8-114">Список Апплеусеринитиатеденроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="24cb8-114">List appleUserInitiatedEnrollmentProfiles</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|<span data-ttu-id="24cb8-115">Коллекция [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="24cb8-115">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) collection</span></span>|<span data-ttu-id="24cb8-116">Список свойств и связей объектов [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="24cb8-116">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="24cb8-117">Получение Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="24cb8-117">Get appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[<span data-ttu-id="24cb8-118">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="24cb8-118">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="24cb8-119">Чтение свойств и связей объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="24cb8-119">Read properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="24cb8-120">Создание Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="24cb8-120">Create appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[<span data-ttu-id="24cb8-121">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="24cb8-121">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="24cb8-122">Создание нового объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="24cb8-122">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="24cb8-123">Удаление Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="24cb8-123">Delete appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|<span data-ttu-id="24cb8-124">Нет</span><span class="sxs-lookup"><span data-stu-id="24cb8-124">None</span></span>|<span data-ttu-id="24cb8-125">Удаляет объект [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="24cb8-125">Deletes a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="24cb8-126">Обновление Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="24cb8-126">Update appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[<span data-ttu-id="24cb8-127">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="24cb8-127">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="24cb8-128">Обновление свойств объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="24cb8-128">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="24cb8-129">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="24cb8-129">setPriority action</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|<span data-ttu-id="24cb8-130">Нет</span><span class="sxs-lookup"><span data-stu-id="24cb8-130">None</span></span>|<span data-ttu-id="24cb8-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="24cb8-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="24cb8-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="24cb8-132">Properties</span></span>
|<span data-ttu-id="24cb8-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="24cb8-133">Property</span></span>|<span data-ttu-id="24cb8-134">Тип</span><span class="sxs-lookup"><span data-stu-id="24cb8-134">Type</span></span>|<span data-ttu-id="24cb8-135">Описание</span><span class="sxs-lookup"><span data-stu-id="24cb8-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24cb8-136">дефаултенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="24cb8-136">defaultEnrollmentType</span></span>|[<span data-ttu-id="24cb8-137">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="24cb8-137">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="24cb8-138">Тип регистрации профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="24cb8-138">The default profile enrollment type.</span></span> <span data-ttu-id="24cb8-139">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="24cb8-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="24cb8-140">аваилаблинроллменттипеоптионс</span><span class="sxs-lookup"><span data-stu-id="24cb8-140">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="24cb8-141">Коллекция [апплеовнертипинроллменттипе](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="24cb8-141">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="24cb8-142">Список доступных параметров типа регистрации</span><span class="sxs-lookup"><span data-stu-id="24cb8-142">List of available enrollment type options</span></span>|
|<span data-ttu-id="24cb8-143">id</span><span class="sxs-lookup"><span data-stu-id="24cb8-143">id</span></span>|<span data-ttu-id="24cb8-144">Строка</span><span class="sxs-lookup"><span data-stu-id="24cb8-144">String</span></span>|<span data-ttu-id="24cb8-145">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="24cb8-145">The GUID for the object</span></span>|
|<span data-ttu-id="24cb8-146">displayName</span><span class="sxs-lookup"><span data-stu-id="24cb8-146">displayName</span></span>|<span data-ttu-id="24cb8-147">Строка</span><span class="sxs-lookup"><span data-stu-id="24cb8-147">String</span></span>|<span data-ttu-id="24cb8-148">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="24cb8-148">Name of the profile</span></span>|
|<span data-ttu-id="24cb8-149">description</span><span class="sxs-lookup"><span data-stu-id="24cb8-149">description</span></span>|<span data-ttu-id="24cb8-150">String</span><span class="sxs-lookup"><span data-stu-id="24cb8-150">String</span></span>|<span data-ttu-id="24cb8-151">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="24cb8-151">Description of the profile</span></span>|
|<span data-ttu-id="24cb8-152">priority</span><span class="sxs-lookup"><span data-stu-id="24cb8-152">priority</span></span>|<span data-ttu-id="24cb8-153">Int32</span><span class="sxs-lookup"><span data-stu-id="24cb8-153">Int32</span></span>|<span data-ttu-id="24cb8-154">Приоритет, 0 — самый высокий</span><span class="sxs-lookup"><span data-stu-id="24cb8-154">Priority, 0 is highest</span></span>|
|<span data-ttu-id="24cb8-155">platform</span><span class="sxs-lookup"><span data-stu-id="24cb8-155">platform</span></span>|[<span data-ttu-id="24cb8-156">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="24cb8-156">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="24cb8-157">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="24cb8-157">The platform of the Device.</span></span> <span data-ttu-id="24cb8-158">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="24cb8-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="24cb8-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24cb8-159">createdDateTime</span></span>|<span data-ttu-id="24cb8-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24cb8-160">DateTimeOffset</span></span>|<span data-ttu-id="24cb8-161">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="24cb8-161">Profile creation time</span></span>|
|<span data-ttu-id="24cb8-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24cb8-162">lastModifiedDateTime</span></span>|<span data-ttu-id="24cb8-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24cb8-163">DateTimeOffset</span></span>|<span data-ttu-id="24cb8-164">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="24cb8-164">Profile last modified time</span></span>|

## <a name="relationships"></a><span data-ttu-id="24cb8-165">Связи</span><span class="sxs-lookup"><span data-stu-id="24cb8-165">Relationships</span></span>
|<span data-ttu-id="24cb8-166">Связь</span><span class="sxs-lookup"><span data-stu-id="24cb8-166">Relationship</span></span>|<span data-ttu-id="24cb8-167">Тип</span><span class="sxs-lookup"><span data-stu-id="24cb8-167">Type</span></span>|<span data-ttu-id="24cb8-168">Описание</span><span class="sxs-lookup"><span data-stu-id="24cb8-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24cb8-169">assignments</span><span class="sxs-lookup"><span data-stu-id="24cb8-169">assignments</span></span>|<span data-ttu-id="24cb8-170">Коллекция [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="24cb8-170">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) collection</span></span>|<span data-ttu-id="24cb8-171">Список назначений для этого профиля.</span><span class="sxs-lookup"><span data-stu-id="24cb8-171">The list of assignments for this profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24cb8-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24cb8-172">JSON Representation</span></span>
<span data-ttu-id="24cb8-173">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24cb8-173">Here is a JSON representation of the resource.</span></span>
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



