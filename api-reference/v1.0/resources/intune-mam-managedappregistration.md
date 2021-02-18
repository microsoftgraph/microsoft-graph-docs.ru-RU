---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8d2c9043e9283258b904cef1a61a3ce502f69601
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291897"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="0cfb2-104">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="0cfb2-104">managedAppRegistration resource type</span></span>

<span data-ttu-id="0cfb2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cfb2-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cfb2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cfb2-107">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="0cfb2-108">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="0cfb2-109">Методы</span><span class="sxs-lookup"><span data-stu-id="0cfb2-109">Methods</span></span>
|<span data-ttu-id="0cfb2-110">Метод</span><span class="sxs-lookup"><span data-stu-id="0cfb2-110">Method</span></span>|<span data-ttu-id="0cfb2-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0cfb2-111">Return Type</span></span>|<span data-ttu-id="0cfb2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0cfb2-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0cfb2-113">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="0cfb2-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="0cfb2-114">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="0cfb2-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="0cfb2-115">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0cfb2-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="0cfb2-116">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="0cfb2-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="0cfb2-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="0cfb2-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="0cfb2-118">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="0cfb2-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="0cfb2-119">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="0cfb2-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="0cfb2-120">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="0cfb2-120">String collection</span></span>|<span data-ttu-id="0cfb2-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0cfb2-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0cfb2-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cfb2-122">Properties</span></span>
|<span data-ttu-id="0cfb2-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cfb2-123">Property</span></span>|<span data-ttu-id="0cfb2-124">Тип</span><span class="sxs-lookup"><span data-stu-id="0cfb2-124">Type</span></span>|<span data-ttu-id="0cfb2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0cfb2-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cfb2-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0cfb2-126">createdDateTime</span></span>|<span data-ttu-id="0cfb2-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cfb2-127">DateTimeOffset</span></span>|<span data-ttu-id="0cfb2-128">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-128">Date and time of creation</span></span>|
|<span data-ttu-id="0cfb2-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0cfb2-129">lastSyncDateTime</span></span>|<span data-ttu-id="0cfb2-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cfb2-130">DateTimeOffset</span></span>|<span data-ttu-id="0cfb2-131">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="0cfb2-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="0cfb2-132">applicationVersion</span></span>|<span data-ttu-id="0cfb2-133">String</span><span class="sxs-lookup"><span data-stu-id="0cfb2-133">String</span></span>|<span data-ttu-id="0cfb2-134">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-134">App version</span></span>|
|<span data-ttu-id="0cfb2-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="0cfb2-135">managementSdkVersion</span></span>|<span data-ttu-id="0cfb2-136">String</span><span class="sxs-lookup"><span data-stu-id="0cfb2-136">String</span></span>|<span data-ttu-id="0cfb2-137">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-137">App management SDK version</span></span>|
|<span data-ttu-id="0cfb2-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="0cfb2-138">platformVersion</span></span>|<span data-ttu-id="0cfb2-139">String</span><span class="sxs-lookup"><span data-stu-id="0cfb2-139">String</span></span>|<span data-ttu-id="0cfb2-140">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-140">Operating System version</span></span>|
|<span data-ttu-id="0cfb2-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="0cfb2-141">deviceType</span></span>|<span data-ttu-id="0cfb2-142">String</span><span class="sxs-lookup"><span data-stu-id="0cfb2-142">String</span></span>|<span data-ttu-id="0cfb2-143">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-143">Host device type</span></span>|
|<span data-ttu-id="0cfb2-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="0cfb2-144">deviceTag</span></span>|<span data-ttu-id="0cfb2-145">String</span><span class="sxs-lookup"><span data-stu-id="0cfb2-145">String</span></span>|<span data-ttu-id="0cfb2-146">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="0cfb2-147">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="0cfb2-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="0cfb2-148">deviceName</span></span>|<span data-ttu-id="0cfb2-149">String</span><span class="sxs-lookup"><span data-stu-id="0cfb2-149">String</span></span>|<span data-ttu-id="0cfb2-150">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-150">Host device name</span></span>|
|<span data-ttu-id="0cfb2-151">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="0cfb2-151">flaggedReasons</span></span>|<span data-ttu-id="0cfb2-152">[Коллекция managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="0cfb2-152">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="0cfb2-153">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="0cfb2-153">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="0cfb2-154">например</span><span class="sxs-lookup"><span data-stu-id="0cfb2-154">E.g.</span></span> <span data-ttu-id="0cfb2-155">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-155">app running on rooted device</span></span>|
|<span data-ttu-id="0cfb2-156">userId</span><span class="sxs-lookup"><span data-stu-id="0cfb2-156">userId</span></span>|<span data-ttu-id="0cfb2-157">String</span><span class="sxs-lookup"><span data-stu-id="0cfb2-157">String</span></span>|<span data-ttu-id="0cfb2-158">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-158">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="0cfb2-159">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="0cfb2-159">appIdentifier</span></span>|[<span data-ttu-id="0cfb2-160">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="0cfb2-160">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="0cfb2-161">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-161">The app package Identifier</span></span>|
|<span data-ttu-id="0cfb2-162">id</span><span class="sxs-lookup"><span data-stu-id="0cfb2-162">id</span></span>|<span data-ttu-id="0cfb2-163">String</span><span class="sxs-lookup"><span data-stu-id="0cfb2-163">String</span></span>|<span data-ttu-id="0cfb2-164">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-164">Key of the entity.</span></span>|
|<span data-ttu-id="0cfb2-165">version</span><span class="sxs-lookup"><span data-stu-id="0cfb2-165">version</span></span>|<span data-ttu-id="0cfb2-166">String</span><span class="sxs-lookup"><span data-stu-id="0cfb2-166">String</span></span>|<span data-ttu-id="0cfb2-167">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-167">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cfb2-168">Связи</span><span class="sxs-lookup"><span data-stu-id="0cfb2-168">Relationships</span></span>
|<span data-ttu-id="0cfb2-169">Связь</span><span class="sxs-lookup"><span data-stu-id="0cfb2-169">Relationship</span></span>|<span data-ttu-id="0cfb2-170">Тип</span><span class="sxs-lookup"><span data-stu-id="0cfb2-170">Type</span></span>|<span data-ttu-id="0cfb2-171">Описание</span><span class="sxs-lookup"><span data-stu-id="0cfb2-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cfb2-172">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="0cfb2-172">appliedPolicies</span></span>|<span data-ttu-id="0cfb2-173">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0cfb2-173">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="0cfb2-174">Ноль или больше политик, уже примененных к зарегистрированному приложению при последней синхронизации со службой управления.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-174">Zero or more policys already applied on the registered app when it last synchronized with management service.</span></span>|
|<span data-ttu-id="0cfb2-175">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="0cfb2-175">intendedPolicies</span></span>|<span data-ttu-id="0cfb2-176">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0cfb2-176">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="0cfb2-177">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-177">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="0cfb2-178">operations</span><span class="sxs-lookup"><span data-stu-id="0cfb2-178">operations</span></span>|<span data-ttu-id="0cfb2-179">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="0cfb2-179">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="0cfb2-180">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-180">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cfb2-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cfb2-181">JSON Representation</span></span>
<span data-ttu-id="0cfb2-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cfb2-182">Here is a JSON representation of the resource.</span></span>
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
  ],
}
-->








