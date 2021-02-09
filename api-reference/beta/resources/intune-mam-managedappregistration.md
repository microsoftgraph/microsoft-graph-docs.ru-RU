---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b7c762c2477439010562c0e7e1b7ddf565d3203e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157563"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="a7459-104">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="a7459-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="a7459-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7459-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7459-106">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7459-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7459-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7459-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7459-108">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="a7459-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="a7459-109">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="a7459-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="a7459-110">Методы</span><span class="sxs-lookup"><span data-stu-id="a7459-110">Methods</span></span>
|<span data-ttu-id="a7459-111">Метод</span><span class="sxs-lookup"><span data-stu-id="a7459-111">Method</span></span>|<span data-ttu-id="a7459-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a7459-112">Return Type</span></span>|<span data-ttu-id="a7459-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a7459-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7459-114">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="a7459-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="a7459-115">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="a7459-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="a7459-116">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a7459-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="a7459-117">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="a7459-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="a7459-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="a7459-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="a7459-119">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a7459-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="a7459-120">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="a7459-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="a7459-121">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a7459-121">String collection</span></span>|<span data-ttu-id="a7459-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a7459-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a7459-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7459-123">Properties</span></span>
|<span data-ttu-id="a7459-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7459-124">Property</span></span>|<span data-ttu-id="a7459-125">Тип</span><span class="sxs-lookup"><span data-stu-id="a7459-125">Type</span></span>|<span data-ttu-id="a7459-126">Описание</span><span class="sxs-lookup"><span data-stu-id="a7459-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7459-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7459-127">createdDateTime</span></span>|<span data-ttu-id="a7459-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7459-128">DateTimeOffset</span></span>|<span data-ttu-id="a7459-129">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="a7459-129">Date and time of creation</span></span>|
|<span data-ttu-id="a7459-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a7459-130">lastSyncDateTime</span></span>|<span data-ttu-id="a7459-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7459-131">DateTimeOffset</span></span>|<span data-ttu-id="a7459-132">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="a7459-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="a7459-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="a7459-133">applicationVersion</span></span>|<span data-ttu-id="a7459-134">String</span><span class="sxs-lookup"><span data-stu-id="a7459-134">String</span></span>|<span data-ttu-id="a7459-135">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="a7459-135">App version</span></span>|
|<span data-ttu-id="a7459-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="a7459-136">managementSdkVersion</span></span>|<span data-ttu-id="a7459-137">String</span><span class="sxs-lookup"><span data-stu-id="a7459-137">String</span></span>|<span data-ttu-id="a7459-138">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="a7459-138">App management SDK version</span></span>|
|<span data-ttu-id="a7459-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="a7459-139">platformVersion</span></span>|<span data-ttu-id="a7459-140">String</span><span class="sxs-lookup"><span data-stu-id="a7459-140">String</span></span>|<span data-ttu-id="a7459-141">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="a7459-141">Operating System version</span></span>|
|<span data-ttu-id="a7459-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="a7459-142">deviceType</span></span>|<span data-ttu-id="a7459-143">String</span><span class="sxs-lookup"><span data-stu-id="a7459-143">String</span></span>|<span data-ttu-id="a7459-144">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="a7459-144">Host device type</span></span>|
|<span data-ttu-id="a7459-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="a7459-145">deviceTag</span></span>|<span data-ttu-id="a7459-146">String</span><span class="sxs-lookup"><span data-stu-id="a7459-146">String</span></span>|<span data-ttu-id="a7459-147">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="a7459-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="a7459-148">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="a7459-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="a7459-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="a7459-149">deviceName</span></span>|<span data-ttu-id="a7459-150">String</span><span class="sxs-lookup"><span data-stu-id="a7459-150">String</span></span>|<span data-ttu-id="a7459-151">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="a7459-151">Host device name</span></span>|
|<span data-ttu-id="a7459-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="a7459-152">managedDeviceId</span></span>|<span data-ttu-id="a7459-153">String</span><span class="sxs-lookup"><span data-stu-id="a7459-153">String</span></span>|<span data-ttu-id="a7459-154">Идентификатор управляемого устройства на хост-устройстве.</span><span class="sxs-lookup"><span data-stu-id="a7459-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="a7459-155">Значение может быть пустым, даже если устройством управляет хост-устройство.</span><span class="sxs-lookup"><span data-stu-id="a7459-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="a7459-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="a7459-156">azureADDeviceId</span></span>|<span data-ttu-id="a7459-157">String</span><span class="sxs-lookup"><span data-stu-id="a7459-157">String</span></span>|<span data-ttu-id="a7459-158">Идентификатор устройства Azure Active Directory для хост-устройства.</span><span class="sxs-lookup"><span data-stu-id="a7459-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="a7459-159">Значение может быть пустым, даже если на хост-устройстве зарегистрирован Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a7459-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="a7459-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a7459-160">deviceModel</span></span>|<span data-ttu-id="a7459-161">String</span><span class="sxs-lookup"><span data-stu-id="a7459-161">String</span></span>|<span data-ttu-id="a7459-162">Модель устройства для текущей регистрации приложения</span><span class="sxs-lookup"><span data-stu-id="a7459-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="a7459-163">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="a7459-163">deviceManufacturer</span></span>|<span data-ttu-id="a7459-164">String</span><span class="sxs-lookup"><span data-stu-id="a7459-164">String</span></span>|<span data-ttu-id="a7459-165">Производитель устройства для текущей регистрации приложения</span><span class="sxs-lookup"><span data-stu-id="a7459-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="a7459-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="a7459-166">flaggedReasons</span></span>|<span data-ttu-id="a7459-167">[Коллекция managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="a7459-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="a7459-168">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="a7459-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="a7459-169">например</span><span class="sxs-lookup"><span data-stu-id="a7459-169">E.g.</span></span> <span data-ttu-id="a7459-170">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="a7459-170">app running on rooted device</span></span>|
|<span data-ttu-id="a7459-171">userId</span><span class="sxs-lookup"><span data-stu-id="a7459-171">userId</span></span>|<span data-ttu-id="a7459-172">String</span><span class="sxs-lookup"><span data-stu-id="a7459-172">String</span></span>|<span data-ttu-id="a7459-173">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="a7459-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="a7459-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="a7459-174">appIdentifier</span></span>|[<span data-ttu-id="a7459-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a7459-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="a7459-176">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="a7459-176">The app package Identifier</span></span>|
|<span data-ttu-id="a7459-177">id</span><span class="sxs-lookup"><span data-stu-id="a7459-177">id</span></span>|<span data-ttu-id="a7459-178">String</span><span class="sxs-lookup"><span data-stu-id="a7459-178">String</span></span>|<span data-ttu-id="a7459-179">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a7459-179">Key of the entity.</span></span>|
|<span data-ttu-id="a7459-180">version</span><span class="sxs-lookup"><span data-stu-id="a7459-180">version</span></span>|<span data-ttu-id="a7459-181">String</span><span class="sxs-lookup"><span data-stu-id="a7459-181">String</span></span>|<span data-ttu-id="a7459-182">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="a7459-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7459-183">Связи</span><span class="sxs-lookup"><span data-stu-id="a7459-183">Relationships</span></span>
|<span data-ttu-id="a7459-184">Связь</span><span class="sxs-lookup"><span data-stu-id="a7459-184">Relationship</span></span>|<span data-ttu-id="a7459-185">Тип</span><span class="sxs-lookup"><span data-stu-id="a7459-185">Type</span></span>|<span data-ttu-id="a7459-186">Описание</span><span class="sxs-lookup"><span data-stu-id="a7459-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7459-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="a7459-187">appliedPolicies</span></span>|<span data-ttu-id="a7459-188">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a7459-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="a7459-189">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="a7459-189">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="a7459-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="a7459-190">intendedPolicies</span></span>|<span data-ttu-id="a7459-191">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a7459-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="a7459-192">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="a7459-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="a7459-193">operations</span><span class="sxs-lookup"><span data-stu-id="a7459-193">operations</span></span>|<span data-ttu-id="a7459-194">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="a7459-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="a7459-195">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="a7459-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7459-196">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7459-196">JSON Representation</span></span>
<span data-ttu-id="a7459-197">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7459-197">Here is a JSON representation of the resource.</span></span>
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




