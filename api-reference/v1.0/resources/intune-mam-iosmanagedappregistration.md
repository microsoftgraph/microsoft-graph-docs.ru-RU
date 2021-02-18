---
title: Тип ресурса iosManagedAppRegistration
description: Представляет собой сведения о синхронизации управляемого приложения iOS для определенного пользователя. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 58933395002bb4f63554e2a7225a89e64cfd8d02
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292506"
---
# <a name="iosmanagedappregistration-resource-type"></a><span data-ttu-id="bf711-104">Тип ресурса iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="bf711-104">iosManagedAppRegistration resource type</span></span>

<span data-ttu-id="bf711-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf711-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf711-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf711-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf711-107">Представляет собой сведения о синхронизации управляемого приложения iOS для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf711-107">Represents the synchronization details of an ios app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="bf711-108">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="bf711-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>


<span data-ttu-id="bf711-109">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-109">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="bf711-110">Методы</span><span class="sxs-lookup"><span data-stu-id="bf711-110">Methods</span></span>
|<span data-ttu-id="bf711-111">Метод</span><span class="sxs-lookup"><span data-stu-id="bf711-111">Method</span></span>|<span data-ttu-id="bf711-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bf711-112">Return Type</span></span>|<span data-ttu-id="bf711-113">Описание</span><span class="sxs-lookup"><span data-stu-id="bf711-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bf711-114">Перечисление iosManagedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="bf711-114">List iosManagedAppRegistrations</span></span>](../api/intune-mam-iosmanagedappregistration-list.md)|<span data-ttu-id="bf711-115">Коллекция [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="bf711-115">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) collection</span></span>|<span data-ttu-id="bf711-116">Список свойств и связей объектов [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-116">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="bf711-117">Получение iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="bf711-117">Get iosManagedAppRegistration</span></span>](../api/intune-mam-iosmanagedappregistration-get.md)|[<span data-ttu-id="bf711-118">iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="bf711-118">iosManagedAppRegistration</span></span>](../resources/intune-mam-iosmanagedappregistration.md)|<span data-ttu-id="bf711-119">Чтение свойств и связей объекта [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-119">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bf711-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf711-120">Properties</span></span>
|<span data-ttu-id="bf711-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf711-121">Property</span></span>|<span data-ttu-id="bf711-122">Тип</span><span class="sxs-lookup"><span data-stu-id="bf711-122">Type</span></span>|<span data-ttu-id="bf711-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bf711-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf711-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf711-124">createdDateTime</span></span>|<span data-ttu-id="bf711-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf711-125">DateTimeOffset</span></span>|<span data-ttu-id="bf711-126">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-126">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bf711-127">lastSyncDateTime</span></span>|<span data-ttu-id="bf711-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf711-128">DateTimeOffset</span></span>|<span data-ttu-id="bf711-129">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="bf711-129">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="bf711-130">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-130">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-131">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="bf711-131">applicationVersion</span></span>|<span data-ttu-id="bf711-132">String</span><span class="sxs-lookup"><span data-stu-id="bf711-132">String</span></span>|<span data-ttu-id="bf711-133">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-133">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-134">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="bf711-134">managementSdkVersion</span></span>|<span data-ttu-id="bf711-135">String</span><span class="sxs-lookup"><span data-stu-id="bf711-135">String</span></span>|<span data-ttu-id="bf711-136">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-136">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-137">platformVersion</span><span class="sxs-lookup"><span data-stu-id="bf711-137">platformVersion</span></span>|<span data-ttu-id="bf711-138">String</span><span class="sxs-lookup"><span data-stu-id="bf711-138">String</span></span>|<span data-ttu-id="bf711-139">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-139">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="bf711-140">deviceType</span></span>|<span data-ttu-id="bf711-141">String</span><span class="sxs-lookup"><span data-stu-id="bf711-141">String</span></span>|<span data-ttu-id="bf711-142">Тип устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-142">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-143">deviceTag</span><span class="sxs-lookup"><span data-stu-id="bf711-143">deviceTag</span></span>|<span data-ttu-id="bf711-144">String</span><span class="sxs-lookup"><span data-stu-id="bf711-144">String</span></span>|<span data-ttu-id="bf711-145">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="bf711-145">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="bf711-146">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="bf711-146">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="bf711-147">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-147">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="bf711-148">deviceName</span></span>|<span data-ttu-id="bf711-149">String</span><span class="sxs-lookup"><span data-stu-id="bf711-149">String</span></span>|<span data-ttu-id="bf711-150">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-150">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-151">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="bf711-151">flaggedReasons</span></span>|<span data-ttu-id="bf711-152">[Коллекция managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="bf711-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="bf711-153">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="bf711-153">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="bf711-154">Пример:</span><span class="sxs-lookup"><span data-stu-id="bf711-154">E.g.</span></span> <span data-ttu-id="bf711-155">приложение запускается на рутованном устройстве. Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-155">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-156">userId</span><span class="sxs-lookup"><span data-stu-id="bf711-156">userId</span></span>|<span data-ttu-id="bf711-157">String</span><span class="sxs-lookup"><span data-stu-id="bf711-157">String</span></span>|<span data-ttu-id="bf711-158">Идентификатор пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="bf711-158">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="bf711-159">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-159">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-160">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="bf711-160">appIdentifier</span></span>|[<span data-ttu-id="bf711-161">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="bf711-161">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="bf711-162">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-162">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-163">id</span><span class="sxs-lookup"><span data-stu-id="bf711-163">id</span></span>|<span data-ttu-id="bf711-164">String</span><span class="sxs-lookup"><span data-stu-id="bf711-164">String</span></span>|<span data-ttu-id="bf711-165">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bf711-165">Key of the entity.</span></span> <span data-ttu-id="bf711-166">Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-166">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-167">version</span><span class="sxs-lookup"><span data-stu-id="bf711-167">version</span></span>|<span data-ttu-id="bf711-168">String</span><span class="sxs-lookup"><span data-stu-id="bf711-168">String</span></span>|<span data-ttu-id="bf711-169">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="bf711-169">Version of the entity.</span></span> <span data-ttu-id="bf711-170">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-170">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf711-171">Связи</span><span class="sxs-lookup"><span data-stu-id="bf711-171">Relationships</span></span>
|<span data-ttu-id="bf711-172">Связь</span><span class="sxs-lookup"><span data-stu-id="bf711-172">Relationship</span></span>|<span data-ttu-id="bf711-173">Тип</span><span class="sxs-lookup"><span data-stu-id="bf711-173">Type</span></span>|<span data-ttu-id="bf711-174">Описание</span><span class="sxs-lookup"><span data-stu-id="bf711-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf711-175">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="bf711-175">appliedPolicies</span></span>|<span data-ttu-id="bf711-176">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bf711-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="bf711-177">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="bf711-177">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="bf711-178">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-178">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-179">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="bf711-179">intendedPolicies</span></span>|<span data-ttu-id="bf711-180">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bf711-180">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="bf711-181">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="bf711-181">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="bf711-182">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-182">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="bf711-183">operations</span><span class="sxs-lookup"><span data-stu-id="bf711-183">operations</span></span>|<span data-ttu-id="bf711-184">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="bf711-184">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="bf711-185">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="bf711-185">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="bf711-186">Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="bf711-186">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf711-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf711-187">JSON Representation</span></span>
<span data-ttu-id="bf711-188">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf711-188">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier",
    "bundleId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [
  ],
}
-->







