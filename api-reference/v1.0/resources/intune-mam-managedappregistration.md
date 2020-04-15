---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a1919cfa3bd7022eda2413a251735b310829afae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43354319"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="f183e-104">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="f183e-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="f183e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f183e-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f183e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f183e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f183e-107">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="f183e-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="f183e-108">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="f183e-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="f183e-109">Методы</span><span class="sxs-lookup"><span data-stu-id="f183e-109">Methods</span></span>
|<span data-ttu-id="f183e-110">Метод</span><span class="sxs-lookup"><span data-stu-id="f183e-110">Method</span></span>|<span data-ttu-id="f183e-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f183e-111">Return Type</span></span>|<span data-ttu-id="f183e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f183e-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f183e-113">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="f183e-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="f183e-114">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="f183e-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="f183e-115">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f183e-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="f183e-116">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="f183e-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="f183e-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="f183e-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="f183e-118">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f183e-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="f183e-119">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="f183e-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="f183e-120">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="f183e-120">String collection</span></span>|<span data-ttu-id="f183e-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f183e-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f183e-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="f183e-122">Properties</span></span>
|<span data-ttu-id="f183e-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="f183e-123">Property</span></span>|<span data-ttu-id="f183e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="f183e-124">Type</span></span>|<span data-ttu-id="f183e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f183e-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f183e-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f183e-126">createdDateTime</span></span>|<span data-ttu-id="f183e-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f183e-127">DateTimeOffset</span></span>|<span data-ttu-id="f183e-128">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="f183e-128">Date and time of creation</span></span>|
|<span data-ttu-id="f183e-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f183e-129">lastSyncDateTime</span></span>|<span data-ttu-id="f183e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f183e-130">DateTimeOffset</span></span>|<span data-ttu-id="f183e-131">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="f183e-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="f183e-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="f183e-132">applicationVersion</span></span>|<span data-ttu-id="f183e-133">String</span><span class="sxs-lookup"><span data-stu-id="f183e-133">String</span></span>|<span data-ttu-id="f183e-134">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="f183e-134">App version</span></span>|
|<span data-ttu-id="f183e-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="f183e-135">managementSdkVersion</span></span>|<span data-ttu-id="f183e-136">String</span><span class="sxs-lookup"><span data-stu-id="f183e-136">String</span></span>|<span data-ttu-id="f183e-137">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="f183e-137">App management SDK version</span></span>|
|<span data-ttu-id="f183e-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="f183e-138">platformVersion</span></span>|<span data-ttu-id="f183e-139">String</span><span class="sxs-lookup"><span data-stu-id="f183e-139">String</span></span>|<span data-ttu-id="f183e-140">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="f183e-140">Operating System version</span></span>|
|<span data-ttu-id="f183e-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="f183e-141">deviceType</span></span>|<span data-ttu-id="f183e-142">String</span><span class="sxs-lookup"><span data-stu-id="f183e-142">String</span></span>|<span data-ttu-id="f183e-143">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="f183e-143">Host device type</span></span>|
|<span data-ttu-id="f183e-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="f183e-144">deviceTag</span></span>|<span data-ttu-id="f183e-145">String</span><span class="sxs-lookup"><span data-stu-id="f183e-145">String</span></span>|<span data-ttu-id="f183e-146">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="f183e-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="f183e-147">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="f183e-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="f183e-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="f183e-148">deviceName</span></span>|<span data-ttu-id="f183e-149">String</span><span class="sxs-lookup"><span data-stu-id="f183e-149">String</span></span>|<span data-ttu-id="f183e-150">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="f183e-150">Host device name</span></span>|
|<span data-ttu-id="f183e-151">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="f183e-151">flaggedReasons</span></span>|<span data-ttu-id="f183e-152">Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="f183e-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="f183e-153">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="f183e-153">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="f183e-154">например</span><span class="sxs-lookup"><span data-stu-id="f183e-154">E.g.</span></span> <span data-ttu-id="f183e-155">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="f183e-155">app running on rooted device</span></span>|
|<span data-ttu-id="f183e-156">userId</span><span class="sxs-lookup"><span data-stu-id="f183e-156">userId</span></span>|<span data-ttu-id="f183e-157">String</span><span class="sxs-lookup"><span data-stu-id="f183e-157">String</span></span>|<span data-ttu-id="f183e-158">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="f183e-158">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="f183e-159">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="f183e-159">appIdentifier</span></span>|[<span data-ttu-id="f183e-160">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f183e-160">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="f183e-161">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="f183e-161">The app package Identifier</span></span>|
|<span data-ttu-id="f183e-162">id</span><span class="sxs-lookup"><span data-stu-id="f183e-162">id</span></span>|<span data-ttu-id="f183e-163">Строка</span><span class="sxs-lookup"><span data-stu-id="f183e-163">String</span></span>|<span data-ttu-id="f183e-164">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f183e-164">Key of the entity.</span></span>|
|<span data-ttu-id="f183e-165">version</span><span class="sxs-lookup"><span data-stu-id="f183e-165">version</span></span>|<span data-ttu-id="f183e-166">Строка</span><span class="sxs-lookup"><span data-stu-id="f183e-166">String</span></span>|<span data-ttu-id="f183e-167">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="f183e-167">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f183e-168">Отношения</span><span class="sxs-lookup"><span data-stu-id="f183e-168">Relationships</span></span>
|<span data-ttu-id="f183e-169">Связь</span><span class="sxs-lookup"><span data-stu-id="f183e-169">Relationship</span></span>|<span data-ttu-id="f183e-170">Тип</span><span class="sxs-lookup"><span data-stu-id="f183e-170">Type</span></span>|<span data-ttu-id="f183e-171">Описание</span><span class="sxs-lookup"><span data-stu-id="f183e-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f183e-172">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="f183e-172">appliedPolicies</span></span>|<span data-ttu-id="f183e-173">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f183e-173">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="f183e-174">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="f183e-174">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="f183e-175">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="f183e-175">intendedPolicies</span></span>|<span data-ttu-id="f183e-176">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f183e-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="f183e-177">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="f183e-177">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="f183e-178">operations</span><span class="sxs-lookup"><span data-stu-id="f183e-178">operations</span></span>|<span data-ttu-id="f183e-179">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="f183e-179">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="f183e-180">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="f183e-180">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f183e-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f183e-181">JSON Representation</span></span>
<span data-ttu-id="f183e-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f183e-182">Here is a JSON representation of the resource.</span></span>
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






