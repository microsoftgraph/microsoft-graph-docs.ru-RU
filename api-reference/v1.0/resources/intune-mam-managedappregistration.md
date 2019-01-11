---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7543f7cf591e1e89c05359634b7c4ec55a327b33
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825769"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="8ebc1-103">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8ebc1-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="8ebc1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ebc1-105">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-105">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="8ebc1-106">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="8ebc1-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8ebc1-107">Methods</span></span>
|<span data-ttu-id="8ebc1-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8ebc1-108">Method</span></span>|<span data-ttu-id="8ebc1-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8ebc1-109">Return Type</span></span>|<span data-ttu-id="8ebc1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8ebc1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ebc1-111">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8ebc1-111">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="8ebc1-112">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8ebc1-112">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="8ebc1-113">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8ebc1-113">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="8ebc1-114">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8ebc1-114">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="8ebc1-115">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8ebc1-115">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="8ebc1-116">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8ebc1-116">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="8ebc1-117">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8ebc1-117">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="8ebc1-118">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="8ebc1-118">String collection</span></span>|<span data-ttu-id="8ebc1-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8ebc1-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8ebc1-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ebc1-120">Properties</span></span>
|<span data-ttu-id="8ebc1-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ebc1-121">Property</span></span>|<span data-ttu-id="8ebc1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="8ebc1-122">Type</span></span>|<span data-ttu-id="8ebc1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8ebc1-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ebc1-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ebc1-124">createdDateTime</span></span>|<span data-ttu-id="8ebc1-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ebc1-125">DateTimeOffset</span></span>|<span data-ttu-id="8ebc1-126">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-126">Date and time of creation</span></span>|
|<span data-ttu-id="8ebc1-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8ebc1-127">lastSyncDateTime</span></span>|<span data-ttu-id="8ebc1-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ebc1-128">DateTimeOffset</span></span>|<span data-ttu-id="8ebc1-129">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-129">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="8ebc1-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="8ebc1-130">applicationVersion</span></span>|<span data-ttu-id="8ebc1-131">String</span><span class="sxs-lookup"><span data-stu-id="8ebc1-131">String</span></span>|<span data-ttu-id="8ebc1-132">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-132">App version</span></span>|
|<span data-ttu-id="8ebc1-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="8ebc1-133">managementSdkVersion</span></span>|<span data-ttu-id="8ebc1-134">String</span><span class="sxs-lookup"><span data-stu-id="8ebc1-134">String</span></span>|<span data-ttu-id="8ebc1-135">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-135">App management SDK version</span></span>|
|<span data-ttu-id="8ebc1-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="8ebc1-136">platformVersion</span></span>|<span data-ttu-id="8ebc1-137">String</span><span class="sxs-lookup"><span data-stu-id="8ebc1-137">String</span></span>|<span data-ttu-id="8ebc1-138">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-138">Operating System version</span></span>|
|<span data-ttu-id="8ebc1-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="8ebc1-139">deviceType</span></span>|<span data-ttu-id="8ebc1-140">String</span><span class="sxs-lookup"><span data-stu-id="8ebc1-140">String</span></span>|<span data-ttu-id="8ebc1-141">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-141">Host device type</span></span>|
|<span data-ttu-id="8ebc1-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="8ebc1-142">deviceTag</span></span>|<span data-ttu-id="8ebc1-143">String</span><span class="sxs-lookup"><span data-stu-id="8ebc1-143">String</span></span>|<span data-ttu-id="8ebc1-144">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="8ebc1-145">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-145">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="8ebc1-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="8ebc1-146">deviceName</span></span>|<span data-ttu-id="8ebc1-147">String</span><span class="sxs-lookup"><span data-stu-id="8ebc1-147">String</span></span>|<span data-ttu-id="8ebc1-148">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-148">Host device name</span></span>|
|<span data-ttu-id="8ebc1-149">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="8ebc1-149">flaggedReasons</span></span>|<span data-ttu-id="8ebc1-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8ebc1-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="8ebc1-151">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="8ebc1-151">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="8ebc1-152">например</span><span class="sxs-lookup"><span data-stu-id="8ebc1-152">E.g.</span></span> <span data-ttu-id="8ebc1-153">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-153">app running on rooted device</span></span>|
|<span data-ttu-id="8ebc1-154">userId</span><span class="sxs-lookup"><span data-stu-id="8ebc1-154">userId</span></span>|<span data-ttu-id="8ebc1-155">String</span><span class="sxs-lookup"><span data-stu-id="8ebc1-155">String</span></span>|<span data-ttu-id="8ebc1-156">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-156">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="8ebc1-157">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="8ebc1-157">appIdentifier</span></span>|[<span data-ttu-id="8ebc1-158">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8ebc1-158">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="8ebc1-159">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-159">The app package Identifier</span></span>|
|<span data-ttu-id="8ebc1-160">id</span><span class="sxs-lookup"><span data-stu-id="8ebc1-160">id</span></span>|<span data-ttu-id="8ebc1-161">Строка</span><span class="sxs-lookup"><span data-stu-id="8ebc1-161">String</span></span>|<span data-ttu-id="8ebc1-162">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-162">Key of the entity.</span></span>|
|<span data-ttu-id="8ebc1-163">version</span><span class="sxs-lookup"><span data-stu-id="8ebc1-163">version</span></span>|<span data-ttu-id="8ebc1-164">Строка</span><span class="sxs-lookup"><span data-stu-id="8ebc1-164">String</span></span>|<span data-ttu-id="8ebc1-165">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-165">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ebc1-166">Связи</span><span class="sxs-lookup"><span data-stu-id="8ebc1-166">Relationships</span></span>
|<span data-ttu-id="8ebc1-167">Связь</span><span class="sxs-lookup"><span data-stu-id="8ebc1-167">Relationship</span></span>|<span data-ttu-id="8ebc1-168">Тип</span><span class="sxs-lookup"><span data-stu-id="8ebc1-168">Type</span></span>|<span data-ttu-id="8ebc1-169">Описание</span><span class="sxs-lookup"><span data-stu-id="8ebc1-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ebc1-170">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="8ebc1-170">appliedPolicies</span></span>|<span data-ttu-id="8ebc1-171">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8ebc1-171">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="8ebc1-172">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-172">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="8ebc1-173">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="8ebc1-173">intendedPolicies</span></span>|<span data-ttu-id="8ebc1-174">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8ebc1-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="8ebc1-175">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-175">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="8ebc1-176">operations</span><span class="sxs-lookup"><span data-stu-id="8ebc1-176">operations</span></span>|<span data-ttu-id="8ebc1-177">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="8ebc1-177">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="8ebc1-178">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-178">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ebc1-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ebc1-179">JSON Representation</span></span>
<span data-ttu-id="8ebc1-180">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ebc1-180">Here is a JSON representation of the resource.</span></span>
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
