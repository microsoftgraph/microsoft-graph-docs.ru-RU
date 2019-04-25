---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3be91dd094258f0bf998521c058f1c62659fbcc8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581032"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="ce7bf-104">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ce7bf-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="ce7bf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce7bf-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce7bf-107">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="ce7bf-108">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="ce7bf-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ce7bf-109">Methods</span></span>
|<span data-ttu-id="ce7bf-110">Метод</span><span class="sxs-lookup"><span data-stu-id="ce7bf-110">Method</span></span>|<span data-ttu-id="ce7bf-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ce7bf-111">Return Type</span></span>|<span data-ttu-id="ce7bf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ce7bf-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ce7bf-113">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ce7bf-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="ce7bf-114">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="ce7bf-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="ce7bf-115">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ce7bf-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="ce7bf-116">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ce7bf-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="ce7bf-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ce7bf-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="ce7bf-118">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ce7bf-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="ce7bf-119">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ce7bf-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="ce7bf-120">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="ce7bf-120">String collection</span></span>|<span data-ttu-id="ce7bf-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ce7bf-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ce7bf-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce7bf-122">Properties</span></span>
|<span data-ttu-id="ce7bf-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce7bf-123">Property</span></span>|<span data-ttu-id="ce7bf-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ce7bf-124">Type</span></span>|<span data-ttu-id="ce7bf-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ce7bf-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce7bf-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce7bf-126">createdDateTime</span></span>|<span data-ttu-id="ce7bf-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce7bf-127">DateTimeOffset</span></span>|<span data-ttu-id="ce7bf-128">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-128">Date and time of creation</span></span>|
|<span data-ttu-id="ce7bf-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ce7bf-129">lastSyncDateTime</span></span>|<span data-ttu-id="ce7bf-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce7bf-130">DateTimeOffset</span></span>|<span data-ttu-id="ce7bf-131">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="ce7bf-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="ce7bf-132">applicationVersion</span></span>|<span data-ttu-id="ce7bf-133">String</span><span class="sxs-lookup"><span data-stu-id="ce7bf-133">String</span></span>|<span data-ttu-id="ce7bf-134">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-134">App version</span></span>|
|<span data-ttu-id="ce7bf-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="ce7bf-135">managementSdkVersion</span></span>|<span data-ttu-id="ce7bf-136">String</span><span class="sxs-lookup"><span data-stu-id="ce7bf-136">String</span></span>|<span data-ttu-id="ce7bf-137">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-137">App management SDK version</span></span>|
|<span data-ttu-id="ce7bf-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="ce7bf-138">platformVersion</span></span>|<span data-ttu-id="ce7bf-139">String</span><span class="sxs-lookup"><span data-stu-id="ce7bf-139">String</span></span>|<span data-ttu-id="ce7bf-140">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-140">Operating System version</span></span>|
|<span data-ttu-id="ce7bf-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="ce7bf-141">deviceType</span></span>|<span data-ttu-id="ce7bf-142">String</span><span class="sxs-lookup"><span data-stu-id="ce7bf-142">String</span></span>|<span data-ttu-id="ce7bf-143">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-143">Host device type</span></span>|
|<span data-ttu-id="ce7bf-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="ce7bf-144">deviceTag</span></span>|<span data-ttu-id="ce7bf-145">String</span><span class="sxs-lookup"><span data-stu-id="ce7bf-145">String</span></span>|<span data-ttu-id="ce7bf-146">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="ce7bf-147">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="ce7bf-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="ce7bf-148">deviceName</span></span>|<span data-ttu-id="ce7bf-149">String</span><span class="sxs-lookup"><span data-stu-id="ce7bf-149">String</span></span>|<span data-ttu-id="ce7bf-150">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-150">Host device name</span></span>|
|<span data-ttu-id="ce7bf-151">Манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="ce7bf-151">managedDeviceId</span></span>|<span data-ttu-id="ce7bf-152">String</span><span class="sxs-lookup"><span data-stu-id="ce7bf-152">String</span></span>|<span data-ttu-id="ce7bf-153">Управляемый идентификатор устройства хоста.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="ce7bf-154">Значение может быть пустым, даже если ведущее устройство управляется.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="ce7bf-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="ce7bf-155">azureADDeviceId</span></span>|<span data-ttu-id="ce7bf-156">String</span><span class="sxs-lookup"><span data-stu-id="ce7bf-156">String</span></span>|<span data-ttu-id="ce7bf-157">Идентификатор устройства Azure Active Directory ведущего устройства.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="ce7bf-158">Значение может быть пустым, даже если ведущее устройство является зарегистрированным Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="ce7bf-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="ce7bf-159">deviceModel</span></span>|<span data-ttu-id="ce7bf-160">String</span><span class="sxs-lookup"><span data-stu-id="ce7bf-160">String</span></span>|<span data-ttu-id="ce7bf-161">Модель устройства для регистрации текущего приложения</span><span class="sxs-lookup"><span data-stu-id="ce7bf-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="ce7bf-162">Девицемануфактурер</span><span class="sxs-lookup"><span data-stu-id="ce7bf-162">deviceManufacturer</span></span>|<span data-ttu-id="ce7bf-163">String</span><span class="sxs-lookup"><span data-stu-id="ce7bf-163">String</span></span>|<span data-ttu-id="ce7bf-164">Производитель устройства для регистрации текущего приложения</span><span class="sxs-lookup"><span data-stu-id="ce7bf-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="ce7bf-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="ce7bf-165">flaggedReasons</span></span>|<span data-ttu-id="ce7bf-166">Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="ce7bf-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="ce7bf-167">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="ce7bf-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="ce7bf-168">например</span><span class="sxs-lookup"><span data-stu-id="ce7bf-168">E.g.</span></span> <span data-ttu-id="ce7bf-169">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-169">app running on rooted device</span></span>|
|<span data-ttu-id="ce7bf-170">userId</span><span class="sxs-lookup"><span data-stu-id="ce7bf-170">userId</span></span>|<span data-ttu-id="ce7bf-171">String</span><span class="sxs-lookup"><span data-stu-id="ce7bf-171">String</span></span>|<span data-ttu-id="ce7bf-172">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="ce7bf-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="ce7bf-173">appIdentifier</span></span>|[<span data-ttu-id="ce7bf-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ce7bf-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="ce7bf-175">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-175">The app package Identifier</span></span>|
|<span data-ttu-id="ce7bf-176">id</span><span class="sxs-lookup"><span data-stu-id="ce7bf-176">id</span></span>|<span data-ttu-id="ce7bf-177">String</span><span class="sxs-lookup"><span data-stu-id="ce7bf-177">String</span></span>|<span data-ttu-id="ce7bf-178">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-178">Key of the entity.</span></span>|
|<span data-ttu-id="ce7bf-179">version</span><span class="sxs-lookup"><span data-stu-id="ce7bf-179">version</span></span>|<span data-ttu-id="ce7bf-180">Строка</span><span class="sxs-lookup"><span data-stu-id="ce7bf-180">String</span></span>|<span data-ttu-id="ce7bf-181">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce7bf-182">Связи</span><span class="sxs-lookup"><span data-stu-id="ce7bf-182">Relationships</span></span>
|<span data-ttu-id="ce7bf-183">Отношение</span><span class="sxs-lookup"><span data-stu-id="ce7bf-183">Relationship</span></span>|<span data-ttu-id="ce7bf-184">Тип</span><span class="sxs-lookup"><span data-stu-id="ce7bf-184">Type</span></span>|<span data-ttu-id="ce7bf-185">Описание</span><span class="sxs-lookup"><span data-stu-id="ce7bf-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce7bf-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="ce7bf-186">appliedPolicies</span></span>|<span data-ttu-id="ce7bf-187">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ce7bf-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="ce7bf-188">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="ce7bf-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="ce7bf-189">intendedPolicies</span></span>|<span data-ttu-id="ce7bf-190">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ce7bf-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="ce7bf-191">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="ce7bf-192">operations</span><span class="sxs-lookup"><span data-stu-id="ce7bf-192">operations</span></span>|<span data-ttu-id="ce7bf-193">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="ce7bf-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="ce7bf-194">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce7bf-195">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce7bf-195">JSON Representation</span></span>
<span data-ttu-id="ce7bf-196">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce7bf-196">Here is a JSON representation of the resource.</span></span>
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





