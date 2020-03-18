---
title: Тип ресурса Апплеусеринитиатеденроллментпрофиле
description: Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b6bf6eefeb94156b85affa3df72665fbe4c3f7bb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783573"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a><span data-ttu-id="0cebf-104">Тип ресурса Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="0cebf-104">appleUserInitiatedEnrollmentProfile resource type</span></span>

> <span data-ttu-id="0cebf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cebf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cebf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cebf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cebf-107">Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены.</span><span class="sxs-lookup"><span data-stu-id="0cebf-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="0cebf-108">Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.</span><span class="sxs-lookup"><span data-stu-id="0cebf-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="0cebf-109">Методы</span><span class="sxs-lookup"><span data-stu-id="0cebf-109">Methods</span></span>
|<span data-ttu-id="0cebf-110">Метод</span><span class="sxs-lookup"><span data-stu-id="0cebf-110">Method</span></span>|<span data-ttu-id="0cebf-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0cebf-111">Return Type</span></span>|<span data-ttu-id="0cebf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0cebf-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0cebf-113">Список Апплеусеринитиатеденроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="0cebf-113">List appleUserInitiatedEnrollmentProfiles</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|<span data-ttu-id="0cebf-114">Коллекция [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0cebf-114">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) collection</span></span>|<span data-ttu-id="0cebf-115">Список свойств и связей объектов [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0cebf-115">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="0cebf-116">Получение Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="0cebf-116">Get appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[<span data-ttu-id="0cebf-117">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="0cebf-117">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="0cebf-118">Чтение свойств и связей объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0cebf-118">Read properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="0cebf-119">Создание Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="0cebf-119">Create appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[<span data-ttu-id="0cebf-120">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="0cebf-120">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="0cebf-121">Создание нового объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0cebf-121">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="0cebf-122">Удаление Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="0cebf-122">Delete appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|<span data-ttu-id="0cebf-123">Нет</span><span class="sxs-lookup"><span data-stu-id="0cebf-123">None</span></span>|<span data-ttu-id="0cebf-124">Удаляет объект [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0cebf-124">Deletes a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="0cebf-125">Обновление Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="0cebf-125">Update appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[<span data-ttu-id="0cebf-126">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="0cebf-126">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="0cebf-127">Обновление свойств объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0cebf-127">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="0cebf-128">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="0cebf-128">setPriority action</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|<span data-ttu-id="0cebf-129">Нет</span><span class="sxs-lookup"><span data-stu-id="0cebf-129">None</span></span>|<span data-ttu-id="0cebf-130">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0cebf-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0cebf-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cebf-131">Properties</span></span>
|<span data-ttu-id="0cebf-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cebf-132">Property</span></span>|<span data-ttu-id="0cebf-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0cebf-133">Type</span></span>|<span data-ttu-id="0cebf-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0cebf-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cebf-135">дефаултенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="0cebf-135">defaultEnrollmentType</span></span>|[<span data-ttu-id="0cebf-136">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0cebf-136">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="0cebf-137">Тип регистрации профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0cebf-137">The default profile enrollment type.</span></span> <span data-ttu-id="0cebf-138">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="0cebf-138">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="0cebf-139">аваилаблинроллменттипеоптионс</span><span class="sxs-lookup"><span data-stu-id="0cebf-139">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="0cebf-140">Коллекция [апплеовнертипинроллменттипе](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="0cebf-140">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="0cebf-141">Список доступных параметров типа регистрации</span><span class="sxs-lookup"><span data-stu-id="0cebf-141">List of available enrollment type options</span></span>|
|<span data-ttu-id="0cebf-142">id</span><span class="sxs-lookup"><span data-stu-id="0cebf-142">id</span></span>|<span data-ttu-id="0cebf-143">Строка</span><span class="sxs-lookup"><span data-stu-id="0cebf-143">String</span></span>|<span data-ttu-id="0cebf-144">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="0cebf-144">The GUID for the object</span></span>|
|<span data-ttu-id="0cebf-145">displayName</span><span class="sxs-lookup"><span data-stu-id="0cebf-145">displayName</span></span>|<span data-ttu-id="0cebf-146">Строка</span><span class="sxs-lookup"><span data-stu-id="0cebf-146">String</span></span>|<span data-ttu-id="0cebf-147">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="0cebf-147">Name of the profile</span></span>|
|<span data-ttu-id="0cebf-148">description</span><span class="sxs-lookup"><span data-stu-id="0cebf-148">description</span></span>|<span data-ttu-id="0cebf-149">String</span><span class="sxs-lookup"><span data-stu-id="0cebf-149">String</span></span>|<span data-ttu-id="0cebf-150">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="0cebf-150">Description of the profile</span></span>|
|<span data-ttu-id="0cebf-151">priority</span><span class="sxs-lookup"><span data-stu-id="0cebf-151">priority</span></span>|<span data-ttu-id="0cebf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0cebf-152">Int32</span></span>|<span data-ttu-id="0cebf-153">Приоритет, 0 — самый высокий</span><span class="sxs-lookup"><span data-stu-id="0cebf-153">Priority, 0 is highest</span></span>|
|<span data-ttu-id="0cebf-154">platform</span><span class="sxs-lookup"><span data-stu-id="0cebf-154">platform</span></span>|[<span data-ttu-id="0cebf-155">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="0cebf-155">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="0cebf-156">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="0cebf-156">The platform of the Device.</span></span> <span data-ttu-id="0cebf-157">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0cebf-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="0cebf-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0cebf-158">createdDateTime</span></span>|<span data-ttu-id="0cebf-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cebf-159">DateTimeOffset</span></span>|<span data-ttu-id="0cebf-160">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="0cebf-160">Profile creation time</span></span>|
|<span data-ttu-id="0cebf-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cebf-161">lastModifiedDateTime</span></span>|<span data-ttu-id="0cebf-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cebf-162">DateTimeOffset</span></span>|<span data-ttu-id="0cebf-163">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="0cebf-163">Profile last modified time</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cebf-164">Связи</span><span class="sxs-lookup"><span data-stu-id="0cebf-164">Relationships</span></span>
|<span data-ttu-id="0cebf-165">Связь</span><span class="sxs-lookup"><span data-stu-id="0cebf-165">Relationship</span></span>|<span data-ttu-id="0cebf-166">Тип</span><span class="sxs-lookup"><span data-stu-id="0cebf-166">Type</span></span>|<span data-ttu-id="0cebf-167">Описание</span><span class="sxs-lookup"><span data-stu-id="0cebf-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cebf-168">assignments</span><span class="sxs-lookup"><span data-stu-id="0cebf-168">assignments</span></span>|<span data-ttu-id="0cebf-169">Коллекция [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0cebf-169">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) collection</span></span>|<span data-ttu-id="0cebf-170">Список назначений для этого профиля.</span><span class="sxs-lookup"><span data-stu-id="0cebf-170">The list of assignments for this profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cebf-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cebf-171">JSON Representation</span></span>
<span data-ttu-id="0cebf-172">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cebf-172">Here is a JSON representation of the resource.</span></span>
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



