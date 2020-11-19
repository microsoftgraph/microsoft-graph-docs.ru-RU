---
title: Тип ресурса Апплеусеринитиатеденроллментпрофиле
description: Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 17b1a2eeff960e7d926c795026f50e43eaf044a3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207507"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a><span data-ttu-id="a82ef-104">Тип ресурса Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="a82ef-104">appleUserInitiatedEnrollmentProfile resource type</span></span>

<span data-ttu-id="a82ef-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a82ef-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a82ef-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a82ef-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a82ef-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a82ef-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a82ef-108">Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены.</span><span class="sxs-lookup"><span data-stu-id="a82ef-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="a82ef-109">Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.</span><span class="sxs-lookup"><span data-stu-id="a82ef-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="a82ef-110">Методы</span><span class="sxs-lookup"><span data-stu-id="a82ef-110">Methods</span></span>
|<span data-ttu-id="a82ef-111">Метод</span><span class="sxs-lookup"><span data-stu-id="a82ef-111">Method</span></span>|<span data-ttu-id="a82ef-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a82ef-112">Return Type</span></span>|<span data-ttu-id="a82ef-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a82ef-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a82ef-114">Список Апплеусеринитиатеденроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="a82ef-114">List appleUserInitiatedEnrollmentProfiles</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|<span data-ttu-id="a82ef-115">Коллекция [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a82ef-115">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) collection</span></span>|<span data-ttu-id="a82ef-116">Список свойств и связей объектов [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a82ef-116">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="a82ef-117">Получение Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="a82ef-117">Get appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[<span data-ttu-id="a82ef-118">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a82ef-118">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="a82ef-119">Чтение свойств и связей объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a82ef-119">Read properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="a82ef-120">Создание Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="a82ef-120">Create appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[<span data-ttu-id="a82ef-121">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a82ef-121">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="a82ef-122">Создание нового объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a82ef-122">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="a82ef-123">Удаление Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="a82ef-123">Delete appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|<span data-ttu-id="a82ef-124">Нет</span><span class="sxs-lookup"><span data-stu-id="a82ef-124">None</span></span>|<span data-ttu-id="a82ef-125">Удаляет объект [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="a82ef-125">Deletes a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="a82ef-126">Обновление Апплеусеринитиатеденроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="a82ef-126">Update appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[<span data-ttu-id="a82ef-127">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a82ef-127">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="a82ef-128">Обновление свойств объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a82ef-128">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="a82ef-129">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="a82ef-129">setPriority action</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|<span data-ttu-id="a82ef-130">Нет</span><span class="sxs-lookup"><span data-stu-id="a82ef-130">None</span></span>|<span data-ttu-id="a82ef-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a82ef-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a82ef-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="a82ef-132">Properties</span></span>
|<span data-ttu-id="a82ef-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="a82ef-133">Property</span></span>|<span data-ttu-id="a82ef-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a82ef-134">Type</span></span>|<span data-ttu-id="a82ef-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a82ef-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a82ef-136">дефаултенроллменттипе</span><span class="sxs-lookup"><span data-stu-id="a82ef-136">defaultEnrollmentType</span></span>|[<span data-ttu-id="a82ef-137">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a82ef-137">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="a82ef-138">Тип регистрации профиля по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a82ef-138">The default profile enrollment type.</span></span> <span data-ttu-id="a82ef-139">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="a82ef-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="a82ef-140">аваилаблинроллменттипеоптионс</span><span class="sxs-lookup"><span data-stu-id="a82ef-140">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="a82ef-141">Коллекция [апплеовнертипинроллменттипе](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="a82ef-141">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="a82ef-142">Список доступных параметров типа регистрации</span><span class="sxs-lookup"><span data-stu-id="a82ef-142">List of available enrollment type options</span></span>|
|<span data-ttu-id="a82ef-143">id</span><span class="sxs-lookup"><span data-stu-id="a82ef-143">id</span></span>|<span data-ttu-id="a82ef-144">String</span><span class="sxs-lookup"><span data-stu-id="a82ef-144">String</span></span>|<span data-ttu-id="a82ef-145">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="a82ef-145">The GUID for the object</span></span>|
|<span data-ttu-id="a82ef-146">displayName</span><span class="sxs-lookup"><span data-stu-id="a82ef-146">displayName</span></span>|<span data-ttu-id="a82ef-147">String</span><span class="sxs-lookup"><span data-stu-id="a82ef-147">String</span></span>|<span data-ttu-id="a82ef-148">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="a82ef-148">Name of the profile</span></span>|
|<span data-ttu-id="a82ef-149">description</span><span class="sxs-lookup"><span data-stu-id="a82ef-149">description</span></span>|<span data-ttu-id="a82ef-150">String</span><span class="sxs-lookup"><span data-stu-id="a82ef-150">String</span></span>|<span data-ttu-id="a82ef-151">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="a82ef-151">Description of the profile</span></span>|
|<span data-ttu-id="a82ef-152">priority</span><span class="sxs-lookup"><span data-stu-id="a82ef-152">priority</span></span>|<span data-ttu-id="a82ef-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a82ef-153">Int32</span></span>|<span data-ttu-id="a82ef-154">Приоритет, 0 — самый высокий</span><span class="sxs-lookup"><span data-stu-id="a82ef-154">Priority, 0 is highest</span></span>|
|<span data-ttu-id="a82ef-155">платформа</span><span class="sxs-lookup"><span data-stu-id="a82ef-155">platform</span></span>|[<span data-ttu-id="a82ef-156">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="a82ef-156">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="a82ef-157">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="a82ef-157">The platform of the Device.</span></span> <span data-ttu-id="a82ef-158">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a82ef-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="a82ef-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a82ef-159">createdDateTime</span></span>|<span data-ttu-id="a82ef-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a82ef-160">DateTimeOffset</span></span>|<span data-ttu-id="a82ef-161">Время создания профиля</span><span class="sxs-lookup"><span data-stu-id="a82ef-161">Profile creation time</span></span>|
|<span data-ttu-id="a82ef-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a82ef-162">lastModifiedDateTime</span></span>|<span data-ttu-id="a82ef-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a82ef-163">DateTimeOffset</span></span>|<span data-ttu-id="a82ef-164">Время последнего изменения профиля</span><span class="sxs-lookup"><span data-stu-id="a82ef-164">Profile last modified time</span></span>|

## <a name="relationships"></a><span data-ttu-id="a82ef-165">Связи</span><span class="sxs-lookup"><span data-stu-id="a82ef-165">Relationships</span></span>
|<span data-ttu-id="a82ef-166">Связь</span><span class="sxs-lookup"><span data-stu-id="a82ef-166">Relationship</span></span>|<span data-ttu-id="a82ef-167">Тип</span><span class="sxs-lookup"><span data-stu-id="a82ef-167">Type</span></span>|<span data-ttu-id="a82ef-168">Описание</span><span class="sxs-lookup"><span data-stu-id="a82ef-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a82ef-169">assignments</span><span class="sxs-lookup"><span data-stu-id="a82ef-169">assignments</span></span>|<span data-ttu-id="a82ef-170">Коллекция [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a82ef-170">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) collection</span></span>|<span data-ttu-id="a82ef-171">Список назначений для этого профиля.</span><span class="sxs-lookup"><span data-stu-id="a82ef-171">The list of assignments for this profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a82ef-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a82ef-172">JSON Representation</span></span>
<span data-ttu-id="a82ef-173">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a82ef-173">Here is a JSON representation of the resource.</span></span>
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




