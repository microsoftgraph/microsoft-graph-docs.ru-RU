---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1e97a238c758f4fdc3130c2527f82ce4445980fc
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178222"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="e481e-104">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e481e-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="e481e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e481e-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e481e-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e481e-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e481e-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e481e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e481e-108">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="e481e-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="e481e-109">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="e481e-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="e481e-110">Методы</span><span class="sxs-lookup"><span data-stu-id="e481e-110">Methods</span></span>
|<span data-ttu-id="e481e-111">Метод</span><span class="sxs-lookup"><span data-stu-id="e481e-111">Method</span></span>|<span data-ttu-id="e481e-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e481e-112">Return Type</span></span>|<span data-ttu-id="e481e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e481e-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e481e-114">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e481e-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="e481e-115">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="e481e-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="e481e-116">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e481e-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="e481e-117">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e481e-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="e481e-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e481e-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="e481e-119">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e481e-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="e481e-120">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e481e-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="e481e-121">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e481e-121">String collection</span></span>|<span data-ttu-id="e481e-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e481e-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e481e-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="e481e-123">Properties</span></span>
|<span data-ttu-id="e481e-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="e481e-124">Property</span></span>|<span data-ttu-id="e481e-125">Тип</span><span class="sxs-lookup"><span data-stu-id="e481e-125">Type</span></span>|<span data-ttu-id="e481e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e481e-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e481e-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e481e-127">createdDateTime</span></span>|<span data-ttu-id="e481e-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e481e-128">DateTimeOffset</span></span>|<span data-ttu-id="e481e-129">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="e481e-129">Date and time of creation</span></span>|
|<span data-ttu-id="e481e-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e481e-130">lastSyncDateTime</span></span>|<span data-ttu-id="e481e-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e481e-131">DateTimeOffset</span></span>|<span data-ttu-id="e481e-132">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="e481e-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="e481e-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="e481e-133">applicationVersion</span></span>|<span data-ttu-id="e481e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e481e-134">String</span></span>|<span data-ttu-id="e481e-135">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="e481e-135">App version</span></span>|
|<span data-ttu-id="e481e-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="e481e-136">managementSdkVersion</span></span>|<span data-ttu-id="e481e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e481e-137">String</span></span>|<span data-ttu-id="e481e-138">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="e481e-138">App management SDK version</span></span>|
|<span data-ttu-id="e481e-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="e481e-139">platformVersion</span></span>|<span data-ttu-id="e481e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="e481e-140">String</span></span>|<span data-ttu-id="e481e-141">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e481e-141">Operating System version</span></span>|
|<span data-ttu-id="e481e-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="e481e-142">deviceType</span></span>|<span data-ttu-id="e481e-143">Строка</span><span class="sxs-lookup"><span data-stu-id="e481e-143">String</span></span>|<span data-ttu-id="e481e-144">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="e481e-144">Host device type</span></span>|
|<span data-ttu-id="e481e-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="e481e-145">deviceTag</span></span>|<span data-ttu-id="e481e-146">String</span><span class="sxs-lookup"><span data-stu-id="e481e-146">String</span></span>|<span data-ttu-id="e481e-147">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="e481e-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="e481e-148">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="e481e-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="e481e-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="e481e-149">deviceName</span></span>|<span data-ttu-id="e481e-150">String</span><span class="sxs-lookup"><span data-stu-id="e481e-150">String</span></span>|<span data-ttu-id="e481e-151">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="e481e-151">Host device name</span></span>|
|<span data-ttu-id="e481e-152">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="e481e-152">managedDeviceId</span></span>|<span data-ttu-id="e481e-153">Строка</span><span class="sxs-lookup"><span data-stu-id="e481e-153">String</span></span>|<span data-ttu-id="e481e-154">Управляемый идентификатор устройства хоста.</span><span class="sxs-lookup"><span data-stu-id="e481e-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="e481e-155">Значение может быть пустым, даже если ведущее устройство управляется.</span><span class="sxs-lookup"><span data-stu-id="e481e-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="e481e-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="e481e-156">azureADDeviceId</span></span>|<span data-ttu-id="e481e-157">Строка</span><span class="sxs-lookup"><span data-stu-id="e481e-157">String</span></span>|<span data-ttu-id="e481e-158">Идентификатор устройства Azure Active Directory ведущего устройства.</span><span class="sxs-lookup"><span data-stu-id="e481e-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="e481e-159">Значение может быть пустым, даже если ведущее устройство является зарегистрированным Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e481e-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="e481e-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="e481e-160">deviceModel</span></span>|<span data-ttu-id="e481e-161">Строка</span><span class="sxs-lookup"><span data-stu-id="e481e-161">String</span></span>|<span data-ttu-id="e481e-162">Модель устройства для регистрации текущего приложения</span><span class="sxs-lookup"><span data-stu-id="e481e-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="e481e-163">девицемануфактурер</span><span class="sxs-lookup"><span data-stu-id="e481e-163">deviceManufacturer</span></span>|<span data-ttu-id="e481e-164">Строка</span><span class="sxs-lookup"><span data-stu-id="e481e-164">String</span></span>|<span data-ttu-id="e481e-165">Производитель устройства для регистрации текущего приложения</span><span class="sxs-lookup"><span data-stu-id="e481e-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="e481e-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="e481e-166">flaggedReasons</span></span>|<span data-ttu-id="e481e-167">Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="e481e-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="e481e-168">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="e481e-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="e481e-169">например</span><span class="sxs-lookup"><span data-stu-id="e481e-169">E.g.</span></span> <span data-ttu-id="e481e-170">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="e481e-170">app running on rooted device</span></span>|
|<span data-ttu-id="e481e-171">userId</span><span class="sxs-lookup"><span data-stu-id="e481e-171">userId</span></span>|<span data-ttu-id="e481e-172">String</span><span class="sxs-lookup"><span data-stu-id="e481e-172">String</span></span>|<span data-ttu-id="e481e-173">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="e481e-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="e481e-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="e481e-174">appIdentifier</span></span>|[<span data-ttu-id="e481e-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e481e-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="e481e-176">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="e481e-176">The app package Identifier</span></span>|
|<span data-ttu-id="e481e-177">id</span><span class="sxs-lookup"><span data-stu-id="e481e-177">id</span></span>|<span data-ttu-id="e481e-178">Строка</span><span class="sxs-lookup"><span data-stu-id="e481e-178">String</span></span>|<span data-ttu-id="e481e-179">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e481e-179">Key of the entity.</span></span>|
|<span data-ttu-id="e481e-180">version</span><span class="sxs-lookup"><span data-stu-id="e481e-180">version</span></span>|<span data-ttu-id="e481e-181">Строка</span><span class="sxs-lookup"><span data-stu-id="e481e-181">String</span></span>|<span data-ttu-id="e481e-182">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="e481e-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e481e-183">Связи</span><span class="sxs-lookup"><span data-stu-id="e481e-183">Relationships</span></span>
|<span data-ttu-id="e481e-184">Связь</span><span class="sxs-lookup"><span data-stu-id="e481e-184">Relationship</span></span>|<span data-ttu-id="e481e-185">Тип</span><span class="sxs-lookup"><span data-stu-id="e481e-185">Type</span></span>|<span data-ttu-id="e481e-186">Описание</span><span class="sxs-lookup"><span data-stu-id="e481e-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e481e-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="e481e-187">appliedPolicies</span></span>|<span data-ttu-id="e481e-188">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e481e-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="e481e-189">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="e481e-189">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="e481e-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="e481e-190">intendedPolicies</span></span>|<span data-ttu-id="e481e-191">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e481e-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="e481e-192">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="e481e-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="e481e-193">operations</span><span class="sxs-lookup"><span data-stu-id="e481e-193">operations</span></span>|<span data-ttu-id="e481e-194">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="e481e-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="e481e-195">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="e481e-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e481e-196">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e481e-196">JSON Representation</span></span>
<span data-ttu-id="e481e-197">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e481e-197">Here is a JSON representation of the resource.</span></span>
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



