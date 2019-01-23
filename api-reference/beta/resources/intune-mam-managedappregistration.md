---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a343dba3df1274693449b8f7cbefd83b131138c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421440"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="9ee56-104">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="9ee56-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="9ee56-105">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9ee56-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9ee56-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ee56-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ee56-107">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ee56-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ee56-108">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="9ee56-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="9ee56-109">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="9ee56-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="9ee56-110">Методы</span><span class="sxs-lookup"><span data-stu-id="9ee56-110">Methods</span></span>
|<span data-ttu-id="9ee56-111">Метод</span><span class="sxs-lookup"><span data-stu-id="9ee56-111">Method</span></span>|<span data-ttu-id="9ee56-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9ee56-112">Return Type</span></span>|<span data-ttu-id="9ee56-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9ee56-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ee56-114">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="9ee56-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="9ee56-115">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="9ee56-116">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9ee56-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="9ee56-117">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="9ee56-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="9ee56-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="9ee56-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="9ee56-119">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9ee56-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="9ee56-120">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="9ee56-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="9ee56-121">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="9ee56-121">String collection</span></span>|<span data-ttu-id="9ee56-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9ee56-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9ee56-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ee56-123">Properties</span></span>
|<span data-ttu-id="9ee56-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ee56-124">Property</span></span>|<span data-ttu-id="9ee56-125">Тип</span><span class="sxs-lookup"><span data-stu-id="9ee56-125">Type</span></span>|<span data-ttu-id="9ee56-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9ee56-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ee56-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ee56-127">createdDateTime</span></span>|<span data-ttu-id="9ee56-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ee56-128">DateTimeOffset</span></span>|<span data-ttu-id="9ee56-129">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="9ee56-129">Date and time of creation</span></span>|
|<span data-ttu-id="9ee56-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9ee56-130">lastSyncDateTime</span></span>|<span data-ttu-id="9ee56-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ee56-131">DateTimeOffset</span></span>|<span data-ttu-id="9ee56-132">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="9ee56-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="9ee56-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="9ee56-133">applicationVersion</span></span>|<span data-ttu-id="9ee56-134">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-134">String</span></span>|<span data-ttu-id="9ee56-135">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="9ee56-135">App version</span></span>|
|<span data-ttu-id="9ee56-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="9ee56-136">managementSdkVersion</span></span>|<span data-ttu-id="9ee56-137">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-137">String</span></span>|<span data-ttu-id="9ee56-138">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="9ee56-138">App management SDK version</span></span>|
|<span data-ttu-id="9ee56-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="9ee56-139">platformVersion</span></span>|<span data-ttu-id="9ee56-140">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-140">String</span></span>|<span data-ttu-id="9ee56-141">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="9ee56-141">Operating System version</span></span>|
|<span data-ttu-id="9ee56-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="9ee56-142">deviceType</span></span>|<span data-ttu-id="9ee56-143">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-143">String</span></span>|<span data-ttu-id="9ee56-144">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="9ee56-144">Host device type</span></span>|
|<span data-ttu-id="9ee56-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="9ee56-145">deviceTag</span></span>|<span data-ttu-id="9ee56-146">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-146">String</span></span>|<span data-ttu-id="9ee56-147">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="9ee56-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="9ee56-148">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="9ee56-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="9ee56-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="9ee56-149">deviceName</span></span>|<span data-ttu-id="9ee56-150">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-150">String</span></span>|<span data-ttu-id="9ee56-151">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="9ee56-151">Host device name</span></span>|
|<span data-ttu-id="9ee56-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="9ee56-152">managedDeviceId</span></span>|<span data-ttu-id="9ee56-153">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-153">String</span></span>|<span data-ttu-id="9ee56-154">Управляемые устройства идентификатор устройства узла.</span><span class="sxs-lookup"><span data-stu-id="9ee56-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="9ee56-155">Значение может быть пустой, даже в том случае, если управляемые устройства узла.</span><span class="sxs-lookup"><span data-stu-id="9ee56-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="9ee56-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="9ee56-156">azureADDeviceId</span></span>|<span data-ttu-id="9ee56-157">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-157">String</span></span>|<span data-ttu-id="9ee56-158">Идентификатор Azure Active Directory устройства устройства узла.</span><span class="sxs-lookup"><span data-stu-id="9ee56-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="9ee56-159">Значение может быть пустым, даже в том случае, если устройство узла — это Azure Active Directory зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="9ee56-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="9ee56-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="9ee56-160">deviceModel</span></span>|<span data-ttu-id="9ee56-161">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-161">String</span></span>|<span data-ttu-id="9ee56-162">Модель устройства для текущего Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="9ee56-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="9ee56-163">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="9ee56-163">deviceManufacturer</span></span>|<span data-ttu-id="9ee56-164">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-164">String</span></span>|<span data-ttu-id="9ee56-165">Производитель устройства для текущего Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="9ee56-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="9ee56-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="9ee56-166">flaggedReasons</span></span>|<span data-ttu-id="9ee56-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9ee56-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="9ee56-168">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="9ee56-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="9ee56-169">например</span><span class="sxs-lookup"><span data-stu-id="9ee56-169">E.g.</span></span> <span data-ttu-id="9ee56-170">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="9ee56-170">app running on rooted device</span></span>|
|<span data-ttu-id="9ee56-171">userId</span><span class="sxs-lookup"><span data-stu-id="9ee56-171">userId</span></span>|<span data-ttu-id="9ee56-172">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-172">String</span></span>|<span data-ttu-id="9ee56-173">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="9ee56-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="9ee56-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="9ee56-174">appIdentifier</span></span>|[<span data-ttu-id="9ee56-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9ee56-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="9ee56-176">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="9ee56-176">The app package Identifier</span></span>|
|<span data-ttu-id="9ee56-177">id</span><span class="sxs-lookup"><span data-stu-id="9ee56-177">id</span></span>|<span data-ttu-id="9ee56-178">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-178">String</span></span>|<span data-ttu-id="9ee56-179">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9ee56-179">Key of the entity.</span></span>|
|<span data-ttu-id="9ee56-180">version</span><span class="sxs-lookup"><span data-stu-id="9ee56-180">version</span></span>|<span data-ttu-id="9ee56-181">String</span><span class="sxs-lookup"><span data-stu-id="9ee56-181">String</span></span>|<span data-ttu-id="9ee56-182">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="9ee56-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ee56-183">Связи</span><span class="sxs-lookup"><span data-stu-id="9ee56-183">Relationships</span></span>
|<span data-ttu-id="9ee56-184">Связь</span><span class="sxs-lookup"><span data-stu-id="9ee56-184">Relationship</span></span>|<span data-ttu-id="9ee56-185">Тип</span><span class="sxs-lookup"><span data-stu-id="9ee56-185">Type</span></span>|<span data-ttu-id="9ee56-186">Описание</span><span class="sxs-lookup"><span data-stu-id="9ee56-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ee56-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="9ee56-187">appliedPolicies</span></span>|<span data-ttu-id="9ee56-188">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="9ee56-189">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="9ee56-189">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="9ee56-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="9ee56-190">intendedPolicies</span></span>|<span data-ttu-id="9ee56-191">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="9ee56-192">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="9ee56-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="9ee56-193">operations</span><span class="sxs-lookup"><span data-stu-id="9ee56-193">operations</span></span>|<span data-ttu-id="9ee56-194">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="9ee56-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="9ee56-195">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="9ee56-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ee56-196">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9ee56-196">JSON Representation</span></span>
<span data-ttu-id="9ee56-197">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ee56-197">Here is a JSON representation of the resource.</span></span>
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




