---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: be937879fa6e3d28d7e09538716f3562fc272f56
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367772"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="67034-104">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="67034-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="67034-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67034-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67034-106">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="67034-106">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="67034-107">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="67034-107">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="67034-108">Методы</span><span class="sxs-lookup"><span data-stu-id="67034-108">Methods</span></span>
|<span data-ttu-id="67034-109">Метод</span><span class="sxs-lookup"><span data-stu-id="67034-109">Method</span></span>|<span data-ttu-id="67034-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="67034-110">Return Type</span></span>|<span data-ttu-id="67034-111">Описание</span><span class="sxs-lookup"><span data-stu-id="67034-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="67034-112">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="67034-112">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="67034-113">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="67034-113">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="67034-114">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="67034-114">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="67034-115">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="67034-115">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="67034-116">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="67034-116">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="67034-117">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="67034-117">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="67034-118">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="67034-118">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="67034-119">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="67034-119">String collection</span></span>|<span data-ttu-id="67034-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="67034-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="67034-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="67034-121">Properties</span></span>
|<span data-ttu-id="67034-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="67034-122">Property</span></span>|<span data-ttu-id="67034-123">Тип</span><span class="sxs-lookup"><span data-stu-id="67034-123">Type</span></span>|<span data-ttu-id="67034-124">Описание</span><span class="sxs-lookup"><span data-stu-id="67034-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67034-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67034-125">createdDateTime</span></span>|<span data-ttu-id="67034-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67034-126">DateTimeOffset</span></span>|<span data-ttu-id="67034-127">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="67034-127">Date and time of creation</span></span>|
|<span data-ttu-id="67034-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="67034-128">lastSyncDateTime</span></span>|<span data-ttu-id="67034-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67034-129">DateTimeOffset</span></span>|<span data-ttu-id="67034-130">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="67034-130">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="67034-131">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="67034-131">applicationVersion</span></span>|<span data-ttu-id="67034-132">String</span><span class="sxs-lookup"><span data-stu-id="67034-132">String</span></span>|<span data-ttu-id="67034-133">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="67034-133">App version</span></span>|
|<span data-ttu-id="67034-134">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="67034-134">managementSdkVersion</span></span>|<span data-ttu-id="67034-135">String</span><span class="sxs-lookup"><span data-stu-id="67034-135">String</span></span>|<span data-ttu-id="67034-136">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="67034-136">App management SDK version</span></span>|
|<span data-ttu-id="67034-137">platformVersion</span><span class="sxs-lookup"><span data-stu-id="67034-137">platformVersion</span></span>|<span data-ttu-id="67034-138">String</span><span class="sxs-lookup"><span data-stu-id="67034-138">String</span></span>|<span data-ttu-id="67034-139">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="67034-139">Operating System version</span></span>|
|<span data-ttu-id="67034-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="67034-140">deviceType</span></span>|<span data-ttu-id="67034-141">String</span><span class="sxs-lookup"><span data-stu-id="67034-141">String</span></span>|<span data-ttu-id="67034-142">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="67034-142">Host device type</span></span>|
|<span data-ttu-id="67034-143">deviceTag</span><span class="sxs-lookup"><span data-stu-id="67034-143">deviceTag</span></span>|<span data-ttu-id="67034-144">String</span><span class="sxs-lookup"><span data-stu-id="67034-144">String</span></span>|<span data-ttu-id="67034-145">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="67034-145">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="67034-146">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="67034-146">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="67034-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="67034-147">deviceName</span></span>|<span data-ttu-id="67034-148">String</span><span class="sxs-lookup"><span data-stu-id="67034-148">String</span></span>|<span data-ttu-id="67034-149">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="67034-149">Host device name</span></span>|
|<span data-ttu-id="67034-150">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="67034-150">flaggedReasons</span></span>|<span data-ttu-id="67034-151">Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="67034-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="67034-152">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="67034-152">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="67034-153">например</span><span class="sxs-lookup"><span data-stu-id="67034-153">E.g.</span></span> <span data-ttu-id="67034-154">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="67034-154">app running on rooted device</span></span>|
|<span data-ttu-id="67034-155">userId</span><span class="sxs-lookup"><span data-stu-id="67034-155">userId</span></span>|<span data-ttu-id="67034-156">String</span><span class="sxs-lookup"><span data-stu-id="67034-156">String</span></span>|<span data-ttu-id="67034-157">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="67034-157">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="67034-158">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="67034-158">appIdentifier</span></span>|[<span data-ttu-id="67034-159">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="67034-159">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="67034-160">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="67034-160">The app package Identifier</span></span>|
|<span data-ttu-id="67034-161">id</span><span class="sxs-lookup"><span data-stu-id="67034-161">id</span></span>|<span data-ttu-id="67034-162">Строка</span><span class="sxs-lookup"><span data-stu-id="67034-162">String</span></span>|<span data-ttu-id="67034-163">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="67034-163">Key of the entity.</span></span>|
|<span data-ttu-id="67034-164">version</span><span class="sxs-lookup"><span data-stu-id="67034-164">version</span></span>|<span data-ttu-id="67034-165">Строка</span><span class="sxs-lookup"><span data-stu-id="67034-165">String</span></span>|<span data-ttu-id="67034-166">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="67034-166">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67034-167">Связи</span><span class="sxs-lookup"><span data-stu-id="67034-167">Relationships</span></span>
|<span data-ttu-id="67034-168">Связь</span><span class="sxs-lookup"><span data-stu-id="67034-168">Relationship</span></span>|<span data-ttu-id="67034-169">Тип</span><span class="sxs-lookup"><span data-stu-id="67034-169">Type</span></span>|<span data-ttu-id="67034-170">Описание</span><span class="sxs-lookup"><span data-stu-id="67034-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67034-171">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="67034-171">appliedPolicies</span></span>|<span data-ttu-id="67034-172">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="67034-172">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="67034-173">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="67034-173">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="67034-174">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="67034-174">intendedPolicies</span></span>|<span data-ttu-id="67034-175">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="67034-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="67034-176">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="67034-176">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="67034-177">operations</span><span class="sxs-lookup"><span data-stu-id="67034-177">operations</span></span>|<span data-ttu-id="67034-178">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="67034-178">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="67034-179">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="67034-179">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67034-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67034-180">JSON Representation</span></span>
<span data-ttu-id="67034-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67034-181">Here is a JSON representation of the resource.</span></span>
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



