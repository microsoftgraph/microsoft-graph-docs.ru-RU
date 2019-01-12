---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a954c3465ba4bb4d2f7372ee544a00fcd8c2af7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937091"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="2fa4c-103">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="2fa4c-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="2fa4c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fa4c-105">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-105">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="2fa4c-106">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="2fa4c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2fa4c-107">Methods</span></span>
|<span data-ttu-id="2fa4c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2fa4c-108">Method</span></span>|<span data-ttu-id="2fa4c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2fa4c-109">Return Type</span></span>|<span data-ttu-id="2fa4c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2fa4c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2fa4c-111">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="2fa4c-111">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="2fa4c-112">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="2fa4c-112">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="2fa4c-113">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="2fa4c-113">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="2fa4c-114">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="2fa4c-114">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="2fa4c-115">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="2fa4c-115">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="2fa4c-116">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="2fa4c-116">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="2fa4c-117">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="2fa4c-117">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="2fa4c-118">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="2fa4c-118">String collection</span></span>|<span data-ttu-id="2fa4c-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2fa4c-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2fa4c-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="2fa4c-120">Properties</span></span>
|<span data-ttu-id="2fa4c-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fa4c-121">Property</span></span>|<span data-ttu-id="2fa4c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="2fa4c-122">Type</span></span>|<span data-ttu-id="2fa4c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2fa4c-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fa4c-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2fa4c-124">createdDateTime</span></span>|<span data-ttu-id="2fa4c-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fa4c-125">DateTimeOffset</span></span>|<span data-ttu-id="2fa4c-126">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-126">Date and time of creation</span></span>|
|<span data-ttu-id="2fa4c-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2fa4c-127">lastSyncDateTime</span></span>|<span data-ttu-id="2fa4c-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fa4c-128">DateTimeOffset</span></span>|<span data-ttu-id="2fa4c-129">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-129">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="2fa4c-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="2fa4c-130">applicationVersion</span></span>|<span data-ttu-id="2fa4c-131">String</span><span class="sxs-lookup"><span data-stu-id="2fa4c-131">String</span></span>|<span data-ttu-id="2fa4c-132">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-132">App version</span></span>|
|<span data-ttu-id="2fa4c-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="2fa4c-133">managementSdkVersion</span></span>|<span data-ttu-id="2fa4c-134">String</span><span class="sxs-lookup"><span data-stu-id="2fa4c-134">String</span></span>|<span data-ttu-id="2fa4c-135">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-135">App management SDK version</span></span>|
|<span data-ttu-id="2fa4c-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="2fa4c-136">platformVersion</span></span>|<span data-ttu-id="2fa4c-137">String</span><span class="sxs-lookup"><span data-stu-id="2fa4c-137">String</span></span>|<span data-ttu-id="2fa4c-138">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-138">Operating System version</span></span>|
|<span data-ttu-id="2fa4c-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="2fa4c-139">deviceType</span></span>|<span data-ttu-id="2fa4c-140">String</span><span class="sxs-lookup"><span data-stu-id="2fa4c-140">String</span></span>|<span data-ttu-id="2fa4c-141">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-141">Host device type</span></span>|
|<span data-ttu-id="2fa4c-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="2fa4c-142">deviceTag</span></span>|<span data-ttu-id="2fa4c-143">String</span><span class="sxs-lookup"><span data-stu-id="2fa4c-143">String</span></span>|<span data-ttu-id="2fa4c-144">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="2fa4c-145">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-145">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="2fa4c-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="2fa4c-146">deviceName</span></span>|<span data-ttu-id="2fa4c-147">String</span><span class="sxs-lookup"><span data-stu-id="2fa4c-147">String</span></span>|<span data-ttu-id="2fa4c-148">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-148">Host device name</span></span>|
|<span data-ttu-id="2fa4c-149">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="2fa4c-149">flaggedReasons</span></span>|<span data-ttu-id="2fa4c-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="2fa4c-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="2fa4c-151">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="2fa4c-151">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="2fa4c-152">например</span><span class="sxs-lookup"><span data-stu-id="2fa4c-152">E.g.</span></span> <span data-ttu-id="2fa4c-153">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-153">app running on rooted device</span></span>|
|<span data-ttu-id="2fa4c-154">userId</span><span class="sxs-lookup"><span data-stu-id="2fa4c-154">userId</span></span>|<span data-ttu-id="2fa4c-155">String</span><span class="sxs-lookup"><span data-stu-id="2fa4c-155">String</span></span>|<span data-ttu-id="2fa4c-156">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-156">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="2fa4c-157">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="2fa4c-157">appIdentifier</span></span>|[<span data-ttu-id="2fa4c-158">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="2fa4c-158">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="2fa4c-159">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-159">The app package Identifier</span></span>|
|<span data-ttu-id="2fa4c-160">id</span><span class="sxs-lookup"><span data-stu-id="2fa4c-160">id</span></span>|<span data-ttu-id="2fa4c-161">Строка</span><span class="sxs-lookup"><span data-stu-id="2fa4c-161">String</span></span>|<span data-ttu-id="2fa4c-162">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-162">Key of the entity.</span></span>|
|<span data-ttu-id="2fa4c-163">version</span><span class="sxs-lookup"><span data-stu-id="2fa4c-163">version</span></span>|<span data-ttu-id="2fa4c-164">Строка</span><span class="sxs-lookup"><span data-stu-id="2fa4c-164">String</span></span>|<span data-ttu-id="2fa4c-165">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-165">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fa4c-166">Связи</span><span class="sxs-lookup"><span data-stu-id="2fa4c-166">Relationships</span></span>
|<span data-ttu-id="2fa4c-167">Связь</span><span class="sxs-lookup"><span data-stu-id="2fa4c-167">Relationship</span></span>|<span data-ttu-id="2fa4c-168">Тип</span><span class="sxs-lookup"><span data-stu-id="2fa4c-168">Type</span></span>|<span data-ttu-id="2fa4c-169">Описание</span><span class="sxs-lookup"><span data-stu-id="2fa4c-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fa4c-170">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="2fa4c-170">appliedPolicies</span></span>|<span data-ttu-id="2fa4c-171">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2fa4c-171">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="2fa4c-172">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-172">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="2fa4c-173">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="2fa4c-173">intendedPolicies</span></span>|<span data-ttu-id="2fa4c-174">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2fa4c-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="2fa4c-175">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-175">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="2fa4c-176">operations</span><span class="sxs-lookup"><span data-stu-id="2fa4c-176">operations</span></span>|<span data-ttu-id="2fa4c-177">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="2fa4c-177">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="2fa4c-178">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-178">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2fa4c-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2fa4c-179">JSON Representation</span></span>
<span data-ttu-id="2fa4c-180">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fa4c-180">Here is a JSON representation of the resource.</span></span>
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
