---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f825eb1c432490f0fa638e7f753d7db052adee5f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066427"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="32b18-104">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="32b18-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="32b18-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32b18-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32b18-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32b18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32b18-107">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="32b18-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="32b18-108">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="32b18-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="32b18-109">Методы</span><span class="sxs-lookup"><span data-stu-id="32b18-109">Methods</span></span>
|<span data-ttu-id="32b18-110">Метод</span><span class="sxs-lookup"><span data-stu-id="32b18-110">Method</span></span>|<span data-ttu-id="32b18-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="32b18-111">Return Type</span></span>|<span data-ttu-id="32b18-112">Описание</span><span class="sxs-lookup"><span data-stu-id="32b18-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="32b18-113">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="32b18-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="32b18-114">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="32b18-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="32b18-115">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="32b18-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="32b18-116">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="32b18-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="32b18-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="32b18-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="32b18-118">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="32b18-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="32b18-119">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="32b18-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="32b18-120">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="32b18-120">String collection</span></span>|<span data-ttu-id="32b18-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="32b18-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="32b18-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="32b18-122">Properties</span></span>
|<span data-ttu-id="32b18-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="32b18-123">Property</span></span>|<span data-ttu-id="32b18-124">Тип</span><span class="sxs-lookup"><span data-stu-id="32b18-124">Type</span></span>|<span data-ttu-id="32b18-125">Описание</span><span class="sxs-lookup"><span data-stu-id="32b18-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32b18-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32b18-126">createdDateTime</span></span>|<span data-ttu-id="32b18-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32b18-127">DateTimeOffset</span></span>|<span data-ttu-id="32b18-128">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="32b18-128">Date and time of creation</span></span>|
|<span data-ttu-id="32b18-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="32b18-129">lastSyncDateTime</span></span>|<span data-ttu-id="32b18-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32b18-130">DateTimeOffset</span></span>|<span data-ttu-id="32b18-131">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="32b18-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="32b18-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="32b18-132">applicationVersion</span></span>|<span data-ttu-id="32b18-133">String</span><span class="sxs-lookup"><span data-stu-id="32b18-133">String</span></span>|<span data-ttu-id="32b18-134">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="32b18-134">App version</span></span>|
|<span data-ttu-id="32b18-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="32b18-135">managementSdkVersion</span></span>|<span data-ttu-id="32b18-136">String</span><span class="sxs-lookup"><span data-stu-id="32b18-136">String</span></span>|<span data-ttu-id="32b18-137">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="32b18-137">App management SDK version</span></span>|
|<span data-ttu-id="32b18-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="32b18-138">platformVersion</span></span>|<span data-ttu-id="32b18-139">String</span><span class="sxs-lookup"><span data-stu-id="32b18-139">String</span></span>|<span data-ttu-id="32b18-140">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="32b18-140">Operating System version</span></span>|
|<span data-ttu-id="32b18-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="32b18-141">deviceType</span></span>|<span data-ttu-id="32b18-142">String</span><span class="sxs-lookup"><span data-stu-id="32b18-142">String</span></span>|<span data-ttu-id="32b18-143">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="32b18-143">Host device type</span></span>|
|<span data-ttu-id="32b18-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="32b18-144">deviceTag</span></span>|<span data-ttu-id="32b18-145">String</span><span class="sxs-lookup"><span data-stu-id="32b18-145">String</span></span>|<span data-ttu-id="32b18-146">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="32b18-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="32b18-147">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="32b18-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="32b18-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="32b18-148">deviceName</span></span>|<span data-ttu-id="32b18-149">String</span><span class="sxs-lookup"><span data-stu-id="32b18-149">String</span></span>|<span data-ttu-id="32b18-150">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="32b18-150">Host device name</span></span>|
|<span data-ttu-id="32b18-151">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="32b18-151">flaggedReasons</span></span>|<span data-ttu-id="32b18-152">Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="32b18-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="32b18-153">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="32b18-153">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="32b18-154">например</span><span class="sxs-lookup"><span data-stu-id="32b18-154">E.g.</span></span> <span data-ttu-id="32b18-155">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="32b18-155">app running on rooted device</span></span>|
|<span data-ttu-id="32b18-156">userId</span><span class="sxs-lookup"><span data-stu-id="32b18-156">userId</span></span>|<span data-ttu-id="32b18-157">String</span><span class="sxs-lookup"><span data-stu-id="32b18-157">String</span></span>|<span data-ttu-id="32b18-158">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="32b18-158">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="32b18-159">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="32b18-159">appIdentifier</span></span>|[<span data-ttu-id="32b18-160">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="32b18-160">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="32b18-161">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="32b18-161">The app package Identifier</span></span>|
|<span data-ttu-id="32b18-162">id</span><span class="sxs-lookup"><span data-stu-id="32b18-162">id</span></span>|<span data-ttu-id="32b18-163">String</span><span class="sxs-lookup"><span data-stu-id="32b18-163">String</span></span>|<span data-ttu-id="32b18-164">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="32b18-164">Key of the entity.</span></span>|
|<span data-ttu-id="32b18-165">version</span><span class="sxs-lookup"><span data-stu-id="32b18-165">version</span></span>|<span data-ttu-id="32b18-166">String</span><span class="sxs-lookup"><span data-stu-id="32b18-166">String</span></span>|<span data-ttu-id="32b18-167">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="32b18-167">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32b18-168">Связи</span><span class="sxs-lookup"><span data-stu-id="32b18-168">Relationships</span></span>
|<span data-ttu-id="32b18-169">Связь</span><span class="sxs-lookup"><span data-stu-id="32b18-169">Relationship</span></span>|<span data-ttu-id="32b18-170">Тип</span><span class="sxs-lookup"><span data-stu-id="32b18-170">Type</span></span>|<span data-ttu-id="32b18-171">Описание</span><span class="sxs-lookup"><span data-stu-id="32b18-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32b18-172">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="32b18-172">appliedPolicies</span></span>|<span data-ttu-id="32b18-173">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="32b18-173">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="32b18-174">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="32b18-174">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="32b18-175">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="32b18-175">intendedPolicies</span></span>|<span data-ttu-id="32b18-176">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="32b18-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="32b18-177">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="32b18-177">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="32b18-178">operations</span><span class="sxs-lookup"><span data-stu-id="32b18-178">operations</span></span>|<span data-ttu-id="32b18-179">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="32b18-179">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="32b18-180">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="32b18-180">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32b18-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32b18-181">JSON Representation</span></span>
<span data-ttu-id="32b18-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32b18-182">Here is a JSON representation of the resource.</span></span>
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

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->








