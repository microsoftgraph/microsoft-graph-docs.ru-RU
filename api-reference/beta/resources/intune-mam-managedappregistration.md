---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2212281ddcf388c1719d317836d8863432591eb5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524310"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="57149-104">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="57149-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="57149-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="57149-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57149-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57149-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57149-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57149-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57149-108">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="57149-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="57149-109">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="57149-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="57149-110">Методы</span><span class="sxs-lookup"><span data-stu-id="57149-110">Methods</span></span>
|<span data-ttu-id="57149-111">Метод</span><span class="sxs-lookup"><span data-stu-id="57149-111">Method</span></span>|<span data-ttu-id="57149-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="57149-112">Return Type</span></span>|<span data-ttu-id="57149-113">Описание</span><span class="sxs-lookup"><span data-stu-id="57149-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="57149-114">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="57149-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="57149-115">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="57149-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="57149-116">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="57149-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="57149-117">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="57149-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="57149-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="57149-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="57149-119">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="57149-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="57149-120">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="57149-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="57149-121">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="57149-121">String collection</span></span>|<span data-ttu-id="57149-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="57149-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="57149-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="57149-123">Properties</span></span>
|<span data-ttu-id="57149-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="57149-124">Property</span></span>|<span data-ttu-id="57149-125">Тип</span><span class="sxs-lookup"><span data-stu-id="57149-125">Type</span></span>|<span data-ttu-id="57149-126">Описание</span><span class="sxs-lookup"><span data-stu-id="57149-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57149-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57149-127">createdDateTime</span></span>|<span data-ttu-id="57149-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57149-128">DateTimeOffset</span></span>|<span data-ttu-id="57149-129">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="57149-129">Date and time of creation</span></span>|
|<span data-ttu-id="57149-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="57149-130">lastSyncDateTime</span></span>|<span data-ttu-id="57149-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57149-131">DateTimeOffset</span></span>|<span data-ttu-id="57149-132">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="57149-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="57149-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="57149-133">applicationVersion</span></span>|<span data-ttu-id="57149-134">String</span><span class="sxs-lookup"><span data-stu-id="57149-134">String</span></span>|<span data-ttu-id="57149-135">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="57149-135">App version</span></span>|
|<span data-ttu-id="57149-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="57149-136">managementSdkVersion</span></span>|<span data-ttu-id="57149-137">String</span><span class="sxs-lookup"><span data-stu-id="57149-137">String</span></span>|<span data-ttu-id="57149-138">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="57149-138">App management SDK version</span></span>|
|<span data-ttu-id="57149-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="57149-139">platformVersion</span></span>|<span data-ttu-id="57149-140">String</span><span class="sxs-lookup"><span data-stu-id="57149-140">String</span></span>|<span data-ttu-id="57149-141">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="57149-141">Operating System version</span></span>|
|<span data-ttu-id="57149-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="57149-142">deviceType</span></span>|<span data-ttu-id="57149-143">String</span><span class="sxs-lookup"><span data-stu-id="57149-143">String</span></span>|<span data-ttu-id="57149-144">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="57149-144">Host device type</span></span>|
|<span data-ttu-id="57149-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="57149-145">deviceTag</span></span>|<span data-ttu-id="57149-146">String</span><span class="sxs-lookup"><span data-stu-id="57149-146">String</span></span>|<span data-ttu-id="57149-147">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="57149-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="57149-148">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="57149-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="57149-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="57149-149">deviceName</span></span>|<span data-ttu-id="57149-150">String</span><span class="sxs-lookup"><span data-stu-id="57149-150">String</span></span>|<span data-ttu-id="57149-151">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="57149-151">Host device name</span></span>|
|<span data-ttu-id="57149-152">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="57149-152">managedDeviceId</span></span>|<span data-ttu-id="57149-153">String</span><span class="sxs-lookup"><span data-stu-id="57149-153">String</span></span>|<span data-ttu-id="57149-154">Управляемый идентификатор устройства хоста.</span><span class="sxs-lookup"><span data-stu-id="57149-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="57149-155">Значение может быть пустым, даже если ведущее устройство управляется.</span><span class="sxs-lookup"><span data-stu-id="57149-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="57149-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="57149-156">azureADDeviceId</span></span>|<span data-ttu-id="57149-157">String</span><span class="sxs-lookup"><span data-stu-id="57149-157">String</span></span>|<span data-ttu-id="57149-158">Идентификатор устройства Azure Active Directory ведущего устройства.</span><span class="sxs-lookup"><span data-stu-id="57149-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="57149-159">Значение может быть пустым, даже если ведущее устройство является зарегистрированным Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="57149-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="57149-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="57149-160">deviceModel</span></span>|<span data-ttu-id="57149-161">String</span><span class="sxs-lookup"><span data-stu-id="57149-161">String</span></span>|<span data-ttu-id="57149-162">Модель устройства для регистрации текущего приложения</span><span class="sxs-lookup"><span data-stu-id="57149-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="57149-163">девицемануфактурер</span><span class="sxs-lookup"><span data-stu-id="57149-163">deviceManufacturer</span></span>|<span data-ttu-id="57149-164">String</span><span class="sxs-lookup"><span data-stu-id="57149-164">String</span></span>|<span data-ttu-id="57149-165">Производитель устройства для регистрации текущего приложения</span><span class="sxs-lookup"><span data-stu-id="57149-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="57149-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="57149-166">flaggedReasons</span></span>|<span data-ttu-id="57149-167">Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="57149-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="57149-168">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="57149-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="57149-169">например</span><span class="sxs-lookup"><span data-stu-id="57149-169">E.g.</span></span> <span data-ttu-id="57149-170">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="57149-170">app running on rooted device</span></span>|
|<span data-ttu-id="57149-171">userId</span><span class="sxs-lookup"><span data-stu-id="57149-171">userId</span></span>|<span data-ttu-id="57149-172">String</span><span class="sxs-lookup"><span data-stu-id="57149-172">String</span></span>|<span data-ttu-id="57149-173">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="57149-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="57149-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="57149-174">appIdentifier</span></span>|[<span data-ttu-id="57149-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="57149-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="57149-176">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="57149-176">The app package Identifier</span></span>|
|<span data-ttu-id="57149-177">id</span><span class="sxs-lookup"><span data-stu-id="57149-177">id</span></span>|<span data-ttu-id="57149-178">Строка</span><span class="sxs-lookup"><span data-stu-id="57149-178">String</span></span>|<span data-ttu-id="57149-179">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="57149-179">Key of the entity.</span></span>|
|<span data-ttu-id="57149-180">version</span><span class="sxs-lookup"><span data-stu-id="57149-180">version</span></span>|<span data-ttu-id="57149-181">Строка</span><span class="sxs-lookup"><span data-stu-id="57149-181">String</span></span>|<span data-ttu-id="57149-182">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="57149-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57149-183">Связи</span><span class="sxs-lookup"><span data-stu-id="57149-183">Relationships</span></span>
|<span data-ttu-id="57149-184">Связь</span><span class="sxs-lookup"><span data-stu-id="57149-184">Relationship</span></span>|<span data-ttu-id="57149-185">Тип</span><span class="sxs-lookup"><span data-stu-id="57149-185">Type</span></span>|<span data-ttu-id="57149-186">Описание</span><span class="sxs-lookup"><span data-stu-id="57149-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57149-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="57149-187">appliedPolicies</span></span>|<span data-ttu-id="57149-188">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="57149-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="57149-189">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="57149-189">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="57149-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="57149-190">intendedPolicies</span></span>|<span data-ttu-id="57149-191">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="57149-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="57149-192">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="57149-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="57149-193">operations</span><span class="sxs-lookup"><span data-stu-id="57149-193">operations</span></span>|<span data-ttu-id="57149-194">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="57149-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="57149-195">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="57149-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57149-196">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57149-196">JSON Representation</span></span>
<span data-ttu-id="57149-197">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57149-197">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```



