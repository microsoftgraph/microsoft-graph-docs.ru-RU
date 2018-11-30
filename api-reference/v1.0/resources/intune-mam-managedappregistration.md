---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.
ms.openlocfilehash: efccea80c953ee4eac07588a21944d10810f8532
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025150"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="249b8-103">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="249b8-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="249b8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="249b8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="249b8-105">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="249b8-105">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="249b8-106">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="249b8-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="249b8-107">Методы</span><span class="sxs-lookup"><span data-stu-id="249b8-107">Methods</span></span>
|<span data-ttu-id="249b8-108">Метод</span><span class="sxs-lookup"><span data-stu-id="249b8-108">Method</span></span>|<span data-ttu-id="249b8-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="249b8-109">Return Type</span></span>|<span data-ttu-id="249b8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="249b8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="249b8-111">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="249b8-111">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="249b8-112">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="249b8-112">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="249b8-113">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="249b8-113">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="249b8-114">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="249b8-114">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="249b8-115">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="249b8-115">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="249b8-116">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="249b8-116">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="249b8-117">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="249b8-117">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="249b8-118">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="249b8-118">String collection</span></span>|<span data-ttu-id="249b8-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="249b8-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="249b8-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="249b8-120">Properties</span></span>
|<span data-ttu-id="249b8-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="249b8-121">Property</span></span>|<span data-ttu-id="249b8-122">Тип</span><span class="sxs-lookup"><span data-stu-id="249b8-122">Type</span></span>|<span data-ttu-id="249b8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="249b8-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="249b8-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="249b8-124">createdDateTime</span></span>|<span data-ttu-id="249b8-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="249b8-125">DateTimeOffset</span></span>|<span data-ttu-id="249b8-126">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="249b8-126">Date and time of creation</span></span>|
|<span data-ttu-id="249b8-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="249b8-127">lastSyncDateTime</span></span>|<span data-ttu-id="249b8-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="249b8-128">DateTimeOffset</span></span>|<span data-ttu-id="249b8-129">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="249b8-129">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="249b8-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="249b8-130">applicationVersion</span></span>|<span data-ttu-id="249b8-131">String</span><span class="sxs-lookup"><span data-stu-id="249b8-131">String</span></span>|<span data-ttu-id="249b8-132">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="249b8-132">App version</span></span>|
|<span data-ttu-id="249b8-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="249b8-133">managementSdkVersion</span></span>|<span data-ttu-id="249b8-134">String</span><span class="sxs-lookup"><span data-stu-id="249b8-134">String</span></span>|<span data-ttu-id="249b8-135">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="249b8-135">App management SDK version</span></span>|
|<span data-ttu-id="249b8-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="249b8-136">platformVersion</span></span>|<span data-ttu-id="249b8-137">String</span><span class="sxs-lookup"><span data-stu-id="249b8-137">String</span></span>|<span data-ttu-id="249b8-138">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="249b8-138">Operating System version</span></span>|
|<span data-ttu-id="249b8-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="249b8-139">deviceType</span></span>|<span data-ttu-id="249b8-140">String</span><span class="sxs-lookup"><span data-stu-id="249b8-140">String</span></span>|<span data-ttu-id="249b8-141">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="249b8-141">Host device type</span></span>|
|<span data-ttu-id="249b8-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="249b8-142">deviceTag</span></span>|<span data-ttu-id="249b8-143">String</span><span class="sxs-lookup"><span data-stu-id="249b8-143">String</span></span>|<span data-ttu-id="249b8-144">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="249b8-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="249b8-145">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="249b8-145">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="249b8-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="249b8-146">deviceName</span></span>|<span data-ttu-id="249b8-147">String</span><span class="sxs-lookup"><span data-stu-id="249b8-147">String</span></span>|<span data-ttu-id="249b8-148">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="249b8-148">Host device name</span></span>|
|<span data-ttu-id="249b8-149">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="249b8-149">flaggedReasons</span></span>|<span data-ttu-id="249b8-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="249b8-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="249b8-151">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="249b8-151">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="249b8-152">например</span><span class="sxs-lookup"><span data-stu-id="249b8-152">E.g.</span></span> <span data-ttu-id="249b8-153">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="249b8-153">app running on rooted device</span></span>|
|<span data-ttu-id="249b8-154">userId</span><span class="sxs-lookup"><span data-stu-id="249b8-154">userId</span></span>|<span data-ttu-id="249b8-155">String</span><span class="sxs-lookup"><span data-stu-id="249b8-155">String</span></span>|<span data-ttu-id="249b8-156">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="249b8-156">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="249b8-157">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="249b8-157">appIdentifier</span></span>|[<span data-ttu-id="249b8-158">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="249b8-158">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="249b8-159">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="249b8-159">The app package Identifier</span></span>|
|<span data-ttu-id="249b8-160">id</span><span class="sxs-lookup"><span data-stu-id="249b8-160">id</span></span>|<span data-ttu-id="249b8-161">String</span><span class="sxs-lookup"><span data-stu-id="249b8-161">String</span></span>|<span data-ttu-id="249b8-162">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="249b8-162">Key of the entity.</span></span>|
|<span data-ttu-id="249b8-163">version</span><span class="sxs-lookup"><span data-stu-id="249b8-163">version</span></span>|<span data-ttu-id="249b8-164">String</span><span class="sxs-lookup"><span data-stu-id="249b8-164">String</span></span>|<span data-ttu-id="249b8-165">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="249b8-165">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="249b8-166">Связи</span><span class="sxs-lookup"><span data-stu-id="249b8-166">Relationships</span></span>
|<span data-ttu-id="249b8-167">Связь</span><span class="sxs-lookup"><span data-stu-id="249b8-167">Relationship</span></span>|<span data-ttu-id="249b8-168">Тип</span><span class="sxs-lookup"><span data-stu-id="249b8-168">Type</span></span>|<span data-ttu-id="249b8-169">Описание</span><span class="sxs-lookup"><span data-stu-id="249b8-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="249b8-170">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="249b8-170">appliedPolicies</span></span>|<span data-ttu-id="249b8-171">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="249b8-171">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="249b8-172">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="249b8-172">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="249b8-173">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="249b8-173">intendedPolicies</span></span>|<span data-ttu-id="249b8-174">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="249b8-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="249b8-175">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="249b8-175">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="249b8-176">operations</span><span class="sxs-lookup"><span data-stu-id="249b8-176">operations</span></span>|<span data-ttu-id="249b8-177">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="249b8-177">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="249b8-178">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="249b8-178">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="249b8-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="249b8-179">JSON Representation</span></span>
<span data-ttu-id="249b8-180">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="249b8-180">Here is a JSON representation of the resource.</span></span>
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
