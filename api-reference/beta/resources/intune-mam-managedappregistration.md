---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2d527b4d0a6da5a54a6e167db063b8c4e06a6062
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444184"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="31e15-104">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="31e15-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="31e15-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31e15-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31e15-106">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31e15-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31e15-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31e15-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31e15-108">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="31e15-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="31e15-109">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="31e15-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="31e15-110">Методы</span><span class="sxs-lookup"><span data-stu-id="31e15-110">Methods</span></span>
|<span data-ttu-id="31e15-111">Метод</span><span class="sxs-lookup"><span data-stu-id="31e15-111">Method</span></span>|<span data-ttu-id="31e15-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="31e15-112">Return Type</span></span>|<span data-ttu-id="31e15-113">Описание</span><span class="sxs-lookup"><span data-stu-id="31e15-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="31e15-114">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="31e15-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="31e15-115">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="31e15-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="31e15-116">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="31e15-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="31e15-117">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="31e15-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="31e15-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="31e15-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="31e15-119">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="31e15-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="31e15-120">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="31e15-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="31e15-121">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="31e15-121">String collection</span></span>|<span data-ttu-id="31e15-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="31e15-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="31e15-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="31e15-123">Properties</span></span>
|<span data-ttu-id="31e15-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="31e15-124">Property</span></span>|<span data-ttu-id="31e15-125">Тип</span><span class="sxs-lookup"><span data-stu-id="31e15-125">Type</span></span>|<span data-ttu-id="31e15-126">Описание</span><span class="sxs-lookup"><span data-stu-id="31e15-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31e15-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31e15-127">createdDateTime</span></span>|<span data-ttu-id="31e15-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31e15-128">DateTimeOffset</span></span>|<span data-ttu-id="31e15-129">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="31e15-129">Date and time of creation</span></span>|
|<span data-ttu-id="31e15-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="31e15-130">lastSyncDateTime</span></span>|<span data-ttu-id="31e15-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31e15-131">DateTimeOffset</span></span>|<span data-ttu-id="31e15-132">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="31e15-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="31e15-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="31e15-133">applicationVersion</span></span>|<span data-ttu-id="31e15-134">String</span><span class="sxs-lookup"><span data-stu-id="31e15-134">String</span></span>|<span data-ttu-id="31e15-135">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="31e15-135">App version</span></span>|
|<span data-ttu-id="31e15-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="31e15-136">managementSdkVersion</span></span>|<span data-ttu-id="31e15-137">String</span><span class="sxs-lookup"><span data-stu-id="31e15-137">String</span></span>|<span data-ttu-id="31e15-138">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="31e15-138">App management SDK version</span></span>|
|<span data-ttu-id="31e15-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="31e15-139">platformVersion</span></span>|<span data-ttu-id="31e15-140">String</span><span class="sxs-lookup"><span data-stu-id="31e15-140">String</span></span>|<span data-ttu-id="31e15-141">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="31e15-141">Operating System version</span></span>|
|<span data-ttu-id="31e15-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="31e15-142">deviceType</span></span>|<span data-ttu-id="31e15-143">String</span><span class="sxs-lookup"><span data-stu-id="31e15-143">String</span></span>|<span data-ttu-id="31e15-144">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="31e15-144">Host device type</span></span>|
|<span data-ttu-id="31e15-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="31e15-145">deviceTag</span></span>|<span data-ttu-id="31e15-146">String</span><span class="sxs-lookup"><span data-stu-id="31e15-146">String</span></span>|<span data-ttu-id="31e15-147">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="31e15-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="31e15-148">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="31e15-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="31e15-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="31e15-149">deviceName</span></span>|<span data-ttu-id="31e15-150">String</span><span class="sxs-lookup"><span data-stu-id="31e15-150">String</span></span>|<span data-ttu-id="31e15-151">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="31e15-151">Host device name</span></span>|
|<span data-ttu-id="31e15-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="31e15-152">managedDeviceId</span></span>|<span data-ttu-id="31e15-153">String</span><span class="sxs-lookup"><span data-stu-id="31e15-153">String</span></span>|<span data-ttu-id="31e15-154">Идентификатор управляемого устройства хост-устройства.</span><span class="sxs-lookup"><span data-stu-id="31e15-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="31e15-155">Значение может быть пустым даже при управляемом устройстве хост-устройства.</span><span class="sxs-lookup"><span data-stu-id="31e15-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="31e15-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="31e15-156">azureADDeviceId</span></span>|<span data-ttu-id="31e15-157">String</span><span class="sxs-lookup"><span data-stu-id="31e15-157">String</span></span>|<span data-ttu-id="31e15-158">Идентификатор устройства Azure Active Directory для хост-устройства.</span><span class="sxs-lookup"><span data-stu-id="31e15-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="31e15-159">Значение может быть пустым даже при регистрации устройства Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="31e15-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="31e15-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="31e15-160">deviceModel</span></span>|<span data-ttu-id="31e15-161">String</span><span class="sxs-lookup"><span data-stu-id="31e15-161">String</span></span>|<span data-ttu-id="31e15-162">Модель устройства для текущей регистрации приложений</span><span class="sxs-lookup"><span data-stu-id="31e15-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="31e15-163">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="31e15-163">deviceManufacturer</span></span>|<span data-ttu-id="31e15-164">String</span><span class="sxs-lookup"><span data-stu-id="31e15-164">String</span></span>|<span data-ttu-id="31e15-165">Производитель устройств для текущей регистрации приложений</span><span class="sxs-lookup"><span data-stu-id="31e15-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="31e15-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="31e15-166">flaggedReasons</span></span>|<span data-ttu-id="31e15-167">[коллекция managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="31e15-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="31e15-168">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="31e15-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="31e15-169">например</span><span class="sxs-lookup"><span data-stu-id="31e15-169">E.g.</span></span> <span data-ttu-id="31e15-170">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="31e15-170">app running on rooted device</span></span>|
|<span data-ttu-id="31e15-171">userId</span><span class="sxs-lookup"><span data-stu-id="31e15-171">userId</span></span>|<span data-ttu-id="31e15-172">String</span><span class="sxs-lookup"><span data-stu-id="31e15-172">String</span></span>|<span data-ttu-id="31e15-173">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="31e15-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="31e15-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="31e15-174">appIdentifier</span></span>|[<span data-ttu-id="31e15-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="31e15-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="31e15-176">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="31e15-176">The app package Identifier</span></span>|
|<span data-ttu-id="31e15-177">id</span><span class="sxs-lookup"><span data-stu-id="31e15-177">id</span></span>|<span data-ttu-id="31e15-178">String</span><span class="sxs-lookup"><span data-stu-id="31e15-178">String</span></span>|<span data-ttu-id="31e15-179">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="31e15-179">Key of the entity.</span></span>|
|<span data-ttu-id="31e15-180">version</span><span class="sxs-lookup"><span data-stu-id="31e15-180">version</span></span>|<span data-ttu-id="31e15-181">String</span><span class="sxs-lookup"><span data-stu-id="31e15-181">String</span></span>|<span data-ttu-id="31e15-182">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="31e15-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31e15-183">Связи</span><span class="sxs-lookup"><span data-stu-id="31e15-183">Relationships</span></span>
|<span data-ttu-id="31e15-184">Связь</span><span class="sxs-lookup"><span data-stu-id="31e15-184">Relationship</span></span>|<span data-ttu-id="31e15-185">Тип</span><span class="sxs-lookup"><span data-stu-id="31e15-185">Type</span></span>|<span data-ttu-id="31e15-186">Описание</span><span class="sxs-lookup"><span data-stu-id="31e15-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31e15-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="31e15-187">appliedPolicies</span></span>|<span data-ttu-id="31e15-188">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="31e15-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="31e15-189">При последней синхронизации с службой управления в зарегистрированном приложении уже применены политики zero или более.</span><span class="sxs-lookup"><span data-stu-id="31e15-189">Zero or more policys already applied on the registered app when it last synchronized with management service.</span></span>|
|<span data-ttu-id="31e15-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="31e15-190">intendedPolicies</span></span>|<span data-ttu-id="31e15-191">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="31e15-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="31e15-192">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="31e15-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="31e15-193">operations</span><span class="sxs-lookup"><span data-stu-id="31e15-193">operations</span></span>|<span data-ttu-id="31e15-194">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="31e15-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="31e15-195">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="31e15-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31e15-196">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31e15-196">JSON Representation</span></span>
<span data-ttu-id="31e15-197">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31e15-197">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.windowsAppIdentifier",
    "windowsAppId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




