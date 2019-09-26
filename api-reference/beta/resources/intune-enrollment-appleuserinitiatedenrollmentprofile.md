---
title: Тип ресурса Апплеусеринитиатеденроллментпрофиле
description: Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ed568d5d8169623b5ff3e006d22cdfe5cecd4a47
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201284"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a><span data-ttu-id="97219-104">Тип ресурса Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="97219-104">appleUserInitiatedEnrollmentProfile resource type</span></span>

> <span data-ttu-id="97219-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97219-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97219-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97219-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97219-107">Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены.</span><span class="sxs-lookup"><span data-stu-id="97219-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="97219-108">Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.</span><span class="sxs-lookup"><span data-stu-id="97219-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="97219-109">Методы</span><span class="sxs-lookup"><span data-stu-id="97219-109">Methods</span></span>
|<span data-ttu-id="97219-110">Метод</span><span class="sxs-lookup"><span data-stu-id="97219-110">Method</span></span>|<span data-ttu-id="97219-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="97219-111">Return Type</span></span>|<span data-ttu-id="97219-112">Описание</span><span class="sxs-lookup"><span data-stu-id="97219-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="97219-113">Список Апплеусеринитиатеденроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="97219-113">List appleUserInitiatedEnrollmentProfiles</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|<span data-ttu-id="97219-114">Коллекция [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="97219-114">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) collection</span></span>|<span data-ttu-id="97219-115">Список свойств и связей объектов [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="97219-115">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="97219-116">Получение Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="97219-116">Get appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[<span data-ttu-id="97219-117">апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="97219-117">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="97219-118">Чтение свойств и связей объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="97219-118">Read properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="97219-119">Создание Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="97219-119">Create appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[<span data-ttu-id="97219-120">апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="97219-120">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="97219-121">Создание нового объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="97219-121">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="97219-122">Удаление Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="97219-122">Delete appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|<span data-ttu-id="97219-123">Нет</span><span class="sxs-lookup"><span data-stu-id="97219-123">None</span></span>|<span data-ttu-id="97219-124">Удаляет объект [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="97219-124">Deletes a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="97219-125">Обновление Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="97219-125">Update appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[<span data-ttu-id="97219-126">апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="97219-126">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="97219-127">Обновление свойств объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="97219-127">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="97219-128">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="97219-128">setPriority action</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|<span data-ttu-id="97219-129">Нет</span><span class="sxs-lookup"><span data-stu-id="97219-129">None</span></span>|<span data-ttu-id="97219-130">Н/Д</span><span class="sxs-lookup"><span data-stu-id="97219-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="97219-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="97219-131">Properties</span></span>
|<span data-ttu-id="97219-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="97219-132">Property</span></span>|<span data-ttu-id="97219-133">Тип</span><span class="sxs-lookup"><span data-stu-id="97219-133">Type</span></span>|<span data-ttu-id="97219-134">Описание</span><span class="sxs-lookup"><span data-stu-id="97219-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97219-135">дефаултенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="97219-135">defaultEnrollmentType</span></span>|[<span data-ttu-id="97219-136">апплеусеринитиатеденроллменттипе</span><span class="sxs-lookup"><span data-stu-id="97219-136">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="97219-137">Тип регистрации профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="97219-137">The default profile enrollment type.</span></span> <span data-ttu-id="97219-138">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="97219-138">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="97219-139">аваилаблинроллменттипеоптионс</span><span class="sxs-lookup"><span data-stu-id="97219-139">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="97219-140">Коллекция [апплеовнертипинроллменттипе](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="97219-140">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="97219-141">Список доступных параметров типа регистрации</span><span class="sxs-lookup"><span data-stu-id="97219-141">List of available enrollment type options</span></span>|
|<span data-ttu-id="97219-142">id</span><span class="sxs-lookup"><span data-stu-id="97219-142">id</span></span>|<span data-ttu-id="97219-143">Строка</span><span class="sxs-lookup"><span data-stu-id="97219-143">String</span></span>|<span data-ttu-id="97219-144">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="97219-144">The GUID for the object</span></span>|
|<span data-ttu-id="97219-145">displayName</span><span class="sxs-lookup"><span data-stu-id="97219-145">displayName</span></span>|<span data-ttu-id="97219-146">Строка</span><span class="sxs-lookup"><span data-stu-id="97219-146">String</span></span>|<span data-ttu-id="97219-147">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="97219-147">Name of the profile</span></span>|
|<span data-ttu-id="97219-148">description</span><span class="sxs-lookup"><span data-stu-id="97219-148">description</span></span>|<span data-ttu-id="97219-149">String</span><span class="sxs-lookup"><span data-stu-id="97219-149">String</span></span>|<span data-ttu-id="97219-150">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="97219-150">Description of the profile</span></span>|
|<span data-ttu-id="97219-151">priority</span><span class="sxs-lookup"><span data-stu-id="97219-151">priority</span></span>|<span data-ttu-id="97219-152">Int32</span><span class="sxs-lookup"><span data-stu-id="97219-152">Int32</span></span>|<span data-ttu-id="97219-153">Приоритет, 0 — самый высокий</span><span class="sxs-lookup"><span data-stu-id="97219-153">Priority, 0 is highest</span></span>|
|<span data-ttu-id="97219-154">platform</span><span class="sxs-lookup"><span data-stu-id="97219-154">platform</span></span>|[<span data-ttu-id="97219-155">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="97219-155">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="97219-156">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="97219-156">The platform of the Device.</span></span> <span data-ttu-id="97219-157">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="97219-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="97219-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97219-158">createdDateTime</span></span>|<span data-ttu-id="97219-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97219-159">DateTimeOffset</span></span>|<span data-ttu-id="97219-160">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="97219-160">Profile creation time</span></span>|
|<span data-ttu-id="97219-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97219-161">lastModifiedDateTime</span></span>|<span data-ttu-id="97219-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97219-162">DateTimeOffset</span></span>|<span data-ttu-id="97219-163">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="97219-163">Profile last modified time</span></span>|

## <a name="relationships"></a><span data-ttu-id="97219-164">Отношения</span><span class="sxs-lookup"><span data-stu-id="97219-164">Relationships</span></span>
|<span data-ttu-id="97219-165">Отношение</span><span class="sxs-lookup"><span data-stu-id="97219-165">Relationship</span></span>|<span data-ttu-id="97219-166">Тип</span><span class="sxs-lookup"><span data-stu-id="97219-166">Type</span></span>|<span data-ttu-id="97219-167">Описание</span><span class="sxs-lookup"><span data-stu-id="97219-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97219-168">assignments</span><span class="sxs-lookup"><span data-stu-id="97219-168">assignments</span></span>|<span data-ttu-id="97219-169">Коллекция [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="97219-169">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) collection</span></span>|<span data-ttu-id="97219-170">Список назначений для этого профиля.</span><span class="sxs-lookup"><span data-stu-id="97219-170">The list of assignments for this profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97219-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97219-171">JSON Representation</span></span>
<span data-ttu-id="97219-172">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97219-172">Here is a JSON representation of the resource.</span></span>
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



