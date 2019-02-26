---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc4754a190f19dab34ac417d2852ccc9e06ba9f4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252240"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="e6147-104">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e6147-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="e6147-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6147-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6147-106">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="e6147-106">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="e6147-107">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="e6147-107">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="e6147-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e6147-108">Methods</span></span>
|<span data-ttu-id="e6147-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e6147-109">Method</span></span>|<span data-ttu-id="e6147-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e6147-110">Return Type</span></span>|<span data-ttu-id="e6147-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e6147-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e6147-112">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e6147-112">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="e6147-113">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="e6147-113">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="e6147-114">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e6147-114">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="e6147-115">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e6147-115">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="e6147-116">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e6147-116">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="e6147-117">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e6147-117">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="e6147-118">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e6147-118">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="e6147-119">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e6147-119">String collection</span></span>|<span data-ttu-id="e6147-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e6147-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e6147-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6147-121">Properties</span></span>
|<span data-ttu-id="e6147-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6147-122">Property</span></span>|<span data-ttu-id="e6147-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e6147-123">Type</span></span>|<span data-ttu-id="e6147-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e6147-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6147-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6147-125">createdDateTime</span></span>|<span data-ttu-id="e6147-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6147-126">DateTimeOffset</span></span>|<span data-ttu-id="e6147-127">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="e6147-127">Date and time of creation</span></span>|
|<span data-ttu-id="e6147-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e6147-128">lastSyncDateTime</span></span>|<span data-ttu-id="e6147-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6147-129">DateTimeOffset</span></span>|<span data-ttu-id="e6147-130">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="e6147-130">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="e6147-131">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="e6147-131">applicationVersion</span></span>|<span data-ttu-id="e6147-132">String</span><span class="sxs-lookup"><span data-stu-id="e6147-132">String</span></span>|<span data-ttu-id="e6147-133">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="e6147-133">App version</span></span>|
|<span data-ttu-id="e6147-134">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="e6147-134">managementSdkVersion</span></span>|<span data-ttu-id="e6147-135">String</span><span class="sxs-lookup"><span data-stu-id="e6147-135">String</span></span>|<span data-ttu-id="e6147-136">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="e6147-136">App management SDK version</span></span>|
|<span data-ttu-id="e6147-137">platformVersion</span><span class="sxs-lookup"><span data-stu-id="e6147-137">platformVersion</span></span>|<span data-ttu-id="e6147-138">String</span><span class="sxs-lookup"><span data-stu-id="e6147-138">String</span></span>|<span data-ttu-id="e6147-139">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e6147-139">Operating System version</span></span>|
|<span data-ttu-id="e6147-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="e6147-140">deviceType</span></span>|<span data-ttu-id="e6147-141">String</span><span class="sxs-lookup"><span data-stu-id="e6147-141">String</span></span>|<span data-ttu-id="e6147-142">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="e6147-142">Host device type</span></span>|
|<span data-ttu-id="e6147-143">deviceTag</span><span class="sxs-lookup"><span data-stu-id="e6147-143">deviceTag</span></span>|<span data-ttu-id="e6147-144">String</span><span class="sxs-lookup"><span data-stu-id="e6147-144">String</span></span>|<span data-ttu-id="e6147-145">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="e6147-145">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="e6147-146">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="e6147-146">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="e6147-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="e6147-147">deviceName</span></span>|<span data-ttu-id="e6147-148">String</span><span class="sxs-lookup"><span data-stu-id="e6147-148">String</span></span>|<span data-ttu-id="e6147-149">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="e6147-149">Host device name</span></span>|
|<span data-ttu-id="e6147-150">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="e6147-150">flaggedReasons</span></span>|<span data-ttu-id="e6147-151">Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="e6147-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="e6147-152">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="e6147-152">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="e6147-153">например</span><span class="sxs-lookup"><span data-stu-id="e6147-153">E.g.</span></span> <span data-ttu-id="e6147-154">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="e6147-154">app running on rooted device</span></span>|
|<span data-ttu-id="e6147-155">userId</span><span class="sxs-lookup"><span data-stu-id="e6147-155">userId</span></span>|<span data-ttu-id="e6147-156">String</span><span class="sxs-lookup"><span data-stu-id="e6147-156">String</span></span>|<span data-ttu-id="e6147-157">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="e6147-157">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="e6147-158">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="e6147-158">appIdentifier</span></span>|[<span data-ttu-id="e6147-159">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e6147-159">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="e6147-160">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="e6147-160">The app package Identifier</span></span>|
|<span data-ttu-id="e6147-161">id</span><span class="sxs-lookup"><span data-stu-id="e6147-161">id</span></span>|<span data-ttu-id="e6147-162">String</span><span class="sxs-lookup"><span data-stu-id="e6147-162">String</span></span>|<span data-ttu-id="e6147-163">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e6147-163">Key of the entity.</span></span>|
|<span data-ttu-id="e6147-164">version</span><span class="sxs-lookup"><span data-stu-id="e6147-164">version</span></span>|<span data-ttu-id="e6147-165">Строка</span><span class="sxs-lookup"><span data-stu-id="e6147-165">String</span></span>|<span data-ttu-id="e6147-166">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="e6147-166">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6147-167">Связи</span><span class="sxs-lookup"><span data-stu-id="e6147-167">Relationships</span></span>
|<span data-ttu-id="e6147-168">Отношение</span><span class="sxs-lookup"><span data-stu-id="e6147-168">Relationship</span></span>|<span data-ttu-id="e6147-169">Тип</span><span class="sxs-lookup"><span data-stu-id="e6147-169">Type</span></span>|<span data-ttu-id="e6147-170">Описание</span><span class="sxs-lookup"><span data-stu-id="e6147-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6147-171">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="e6147-171">appliedPolicies</span></span>|<span data-ttu-id="e6147-172">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6147-172">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="e6147-173">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="e6147-173">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="e6147-174">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="e6147-174">intendedPolicies</span></span>|<span data-ttu-id="e6147-175">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6147-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="e6147-176">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="e6147-176">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="e6147-177">operations</span><span class="sxs-lookup"><span data-stu-id="e6147-177">operations</span></span>|<span data-ttu-id="e6147-178">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="e6147-178">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="e6147-179">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="e6147-179">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6147-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6147-180">JSON Representation</span></span>
<span data-ttu-id="e6147-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6147-181">Here is a JSON representation of the resource.</span></span>
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


