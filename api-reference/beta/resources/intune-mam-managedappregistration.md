---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3c2ea9eaf64a4d198ca37fa7c485ee6817c9d749
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030201"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="50fb3-104">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="50fb3-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="50fb3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50fb3-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50fb3-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50fb3-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50fb3-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50fb3-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50fb3-108">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="50fb3-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="50fb3-109">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="50fb3-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="50fb3-110">Методы</span><span class="sxs-lookup"><span data-stu-id="50fb3-110">Methods</span></span>
|<span data-ttu-id="50fb3-111">Метод</span><span class="sxs-lookup"><span data-stu-id="50fb3-111">Method</span></span>|<span data-ttu-id="50fb3-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="50fb3-112">Return Type</span></span>|<span data-ttu-id="50fb3-113">Описание</span><span class="sxs-lookup"><span data-stu-id="50fb3-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50fb3-114">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="50fb3-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="50fb3-115">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="50fb3-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="50fb3-116">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="50fb3-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="50fb3-117">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="50fb3-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="50fb3-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="50fb3-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="50fb3-119">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="50fb3-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="50fb3-120">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="50fb3-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="50fb3-121">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="50fb3-121">String collection</span></span>|<span data-ttu-id="50fb3-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="50fb3-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="50fb3-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="50fb3-123">Properties</span></span>
|<span data-ttu-id="50fb3-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="50fb3-124">Property</span></span>|<span data-ttu-id="50fb3-125">Тип</span><span class="sxs-lookup"><span data-stu-id="50fb3-125">Type</span></span>|<span data-ttu-id="50fb3-126">Описание</span><span class="sxs-lookup"><span data-stu-id="50fb3-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50fb3-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50fb3-127">createdDateTime</span></span>|<span data-ttu-id="50fb3-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50fb3-128">DateTimeOffset</span></span>|<span data-ttu-id="50fb3-129">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="50fb3-129">Date and time of creation</span></span>|
|<span data-ttu-id="50fb3-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="50fb3-130">lastSyncDateTime</span></span>|<span data-ttu-id="50fb3-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50fb3-131">DateTimeOffset</span></span>|<span data-ttu-id="50fb3-132">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="50fb3-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="50fb3-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="50fb3-133">applicationVersion</span></span>|<span data-ttu-id="50fb3-134">String</span><span class="sxs-lookup"><span data-stu-id="50fb3-134">String</span></span>|<span data-ttu-id="50fb3-135">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="50fb3-135">App version</span></span>|
|<span data-ttu-id="50fb3-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="50fb3-136">managementSdkVersion</span></span>|<span data-ttu-id="50fb3-137">String</span><span class="sxs-lookup"><span data-stu-id="50fb3-137">String</span></span>|<span data-ttu-id="50fb3-138">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="50fb3-138">App management SDK version</span></span>|
|<span data-ttu-id="50fb3-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="50fb3-139">platformVersion</span></span>|<span data-ttu-id="50fb3-140">String</span><span class="sxs-lookup"><span data-stu-id="50fb3-140">String</span></span>|<span data-ttu-id="50fb3-141">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="50fb3-141">Operating System version</span></span>|
|<span data-ttu-id="50fb3-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="50fb3-142">deviceType</span></span>|<span data-ttu-id="50fb3-143">String</span><span class="sxs-lookup"><span data-stu-id="50fb3-143">String</span></span>|<span data-ttu-id="50fb3-144">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="50fb3-144">Host device type</span></span>|
|<span data-ttu-id="50fb3-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="50fb3-145">deviceTag</span></span>|<span data-ttu-id="50fb3-146">String</span><span class="sxs-lookup"><span data-stu-id="50fb3-146">String</span></span>|<span data-ttu-id="50fb3-147">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="50fb3-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="50fb3-148">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="50fb3-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="50fb3-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="50fb3-149">deviceName</span></span>|<span data-ttu-id="50fb3-150">String</span><span class="sxs-lookup"><span data-stu-id="50fb3-150">String</span></span>|<span data-ttu-id="50fb3-151">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="50fb3-151">Host device name</span></span>|
|<span data-ttu-id="50fb3-152">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="50fb3-152">managedDeviceId</span></span>|<span data-ttu-id="50fb3-153">String</span><span class="sxs-lookup"><span data-stu-id="50fb3-153">String</span></span>|<span data-ttu-id="50fb3-154">Управляемый идентификатор устройства хоста.</span><span class="sxs-lookup"><span data-stu-id="50fb3-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="50fb3-155">Значение может быть пустым, даже если ведущее устройство управляется.</span><span class="sxs-lookup"><span data-stu-id="50fb3-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="50fb3-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="50fb3-156">azureADDeviceId</span></span>|<span data-ttu-id="50fb3-157">String</span><span class="sxs-lookup"><span data-stu-id="50fb3-157">String</span></span>|<span data-ttu-id="50fb3-158">Идентификатор устройства Azure Active Directory ведущего устройства.</span><span class="sxs-lookup"><span data-stu-id="50fb3-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="50fb3-159">Значение может быть пустым, даже если ведущее устройство является зарегистрированным Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="50fb3-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="50fb3-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="50fb3-160">deviceModel</span></span>|<span data-ttu-id="50fb3-161">String</span><span class="sxs-lookup"><span data-stu-id="50fb3-161">String</span></span>|<span data-ttu-id="50fb3-162">Модель устройства для регистрации текущего приложения</span><span class="sxs-lookup"><span data-stu-id="50fb3-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="50fb3-163">девицемануфактурер</span><span class="sxs-lookup"><span data-stu-id="50fb3-163">deviceManufacturer</span></span>|<span data-ttu-id="50fb3-164">String</span><span class="sxs-lookup"><span data-stu-id="50fb3-164">String</span></span>|<span data-ttu-id="50fb3-165">Производитель устройства для регистрации текущего приложения</span><span class="sxs-lookup"><span data-stu-id="50fb3-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="50fb3-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="50fb3-166">flaggedReasons</span></span>|<span data-ttu-id="50fb3-167">Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="50fb3-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="50fb3-168">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="50fb3-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="50fb3-169">например</span><span class="sxs-lookup"><span data-stu-id="50fb3-169">E.g.</span></span> <span data-ttu-id="50fb3-170">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="50fb3-170">app running on rooted device</span></span>|
|<span data-ttu-id="50fb3-171">userId</span><span class="sxs-lookup"><span data-stu-id="50fb3-171">userId</span></span>|<span data-ttu-id="50fb3-172">String</span><span class="sxs-lookup"><span data-stu-id="50fb3-172">String</span></span>|<span data-ttu-id="50fb3-173">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="50fb3-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="50fb3-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="50fb3-174">appIdentifier</span></span>|[<span data-ttu-id="50fb3-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="50fb3-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="50fb3-176">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="50fb3-176">The app package Identifier</span></span>|
|<span data-ttu-id="50fb3-177">id</span><span class="sxs-lookup"><span data-stu-id="50fb3-177">id</span></span>|<span data-ttu-id="50fb3-178">String</span><span class="sxs-lookup"><span data-stu-id="50fb3-178">String</span></span>|<span data-ttu-id="50fb3-179">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="50fb3-179">Key of the entity.</span></span>|
|<span data-ttu-id="50fb3-180">version</span><span class="sxs-lookup"><span data-stu-id="50fb3-180">version</span></span>|<span data-ttu-id="50fb3-181">String</span><span class="sxs-lookup"><span data-stu-id="50fb3-181">String</span></span>|<span data-ttu-id="50fb3-182">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="50fb3-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50fb3-183">Отношения</span><span class="sxs-lookup"><span data-stu-id="50fb3-183">Relationships</span></span>
|<span data-ttu-id="50fb3-184">Связь</span><span class="sxs-lookup"><span data-stu-id="50fb3-184">Relationship</span></span>|<span data-ttu-id="50fb3-185">Тип</span><span class="sxs-lookup"><span data-stu-id="50fb3-185">Type</span></span>|<span data-ttu-id="50fb3-186">Описание</span><span class="sxs-lookup"><span data-stu-id="50fb3-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50fb3-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="50fb3-187">appliedPolicies</span></span>|<span data-ttu-id="50fb3-188">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="50fb3-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="50fb3-189">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="50fb3-189">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="50fb3-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="50fb3-190">intendedPolicies</span></span>|<span data-ttu-id="50fb3-191">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="50fb3-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="50fb3-192">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="50fb3-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="50fb3-193">operations</span><span class="sxs-lookup"><span data-stu-id="50fb3-193">operations</span></span>|<span data-ttu-id="50fb3-194">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="50fb3-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="50fb3-195">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="50fb3-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50fb3-196">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50fb3-196">JSON Representation</span></span>
<span data-ttu-id="50fb3-197">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50fb3-197">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "managedDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```






