---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 959bd294ab1752617cea6a6ea5bbe8f0a3802f0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869722"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="1f78e-103">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="1f78e-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="1f78e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1f78e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f78e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f78e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f78e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1f78e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f78e-107">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="1f78e-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="1f78e-108">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="1f78e-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="1f78e-109">Методы</span><span class="sxs-lookup"><span data-stu-id="1f78e-109">Methods</span></span>
|<span data-ttu-id="1f78e-110">Метод</span><span class="sxs-lookup"><span data-stu-id="1f78e-110">Method</span></span>|<span data-ttu-id="1f78e-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1f78e-111">Return Type</span></span>|<span data-ttu-id="1f78e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1f78e-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1f78e-113">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="1f78e-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="1f78e-114">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="1f78e-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="1f78e-115">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1f78e-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="1f78e-116">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="1f78e-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="1f78e-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="1f78e-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="1f78e-118">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1f78e-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="1f78e-119">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="1f78e-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="1f78e-120">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="1f78e-120">String collection</span></span>|<span data-ttu-id="1f78e-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1f78e-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1f78e-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f78e-122">Properties</span></span>
|<span data-ttu-id="1f78e-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f78e-123">Property</span></span>|<span data-ttu-id="1f78e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="1f78e-124">Type</span></span>|<span data-ttu-id="1f78e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1f78e-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f78e-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f78e-126">createdDateTime</span></span>|<span data-ttu-id="1f78e-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f78e-127">DateTimeOffset</span></span>|<span data-ttu-id="1f78e-128">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="1f78e-128">Date and time of creation</span></span>|
|<span data-ttu-id="1f78e-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1f78e-129">lastSyncDateTime</span></span>|<span data-ttu-id="1f78e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f78e-130">DateTimeOffset</span></span>|<span data-ttu-id="1f78e-131">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="1f78e-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="1f78e-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="1f78e-132">applicationVersion</span></span>|<span data-ttu-id="1f78e-133">String</span><span class="sxs-lookup"><span data-stu-id="1f78e-133">String</span></span>|<span data-ttu-id="1f78e-134">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="1f78e-134">App version</span></span>|
|<span data-ttu-id="1f78e-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="1f78e-135">managementSdkVersion</span></span>|<span data-ttu-id="1f78e-136">String</span><span class="sxs-lookup"><span data-stu-id="1f78e-136">String</span></span>|<span data-ttu-id="1f78e-137">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="1f78e-137">App management SDK version</span></span>|
|<span data-ttu-id="1f78e-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="1f78e-138">platformVersion</span></span>|<span data-ttu-id="1f78e-139">String</span><span class="sxs-lookup"><span data-stu-id="1f78e-139">String</span></span>|<span data-ttu-id="1f78e-140">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="1f78e-140">Operating System version</span></span>|
|<span data-ttu-id="1f78e-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="1f78e-141">deviceType</span></span>|<span data-ttu-id="1f78e-142">String</span><span class="sxs-lookup"><span data-stu-id="1f78e-142">String</span></span>|<span data-ttu-id="1f78e-143">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="1f78e-143">Host device type</span></span>|
|<span data-ttu-id="1f78e-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="1f78e-144">deviceTag</span></span>|<span data-ttu-id="1f78e-145">String</span><span class="sxs-lookup"><span data-stu-id="1f78e-145">String</span></span>|<span data-ttu-id="1f78e-146">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="1f78e-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="1f78e-147">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="1f78e-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="1f78e-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="1f78e-148">deviceName</span></span>|<span data-ttu-id="1f78e-149">String</span><span class="sxs-lookup"><span data-stu-id="1f78e-149">String</span></span>|<span data-ttu-id="1f78e-150">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="1f78e-150">Host device name</span></span>|
|<span data-ttu-id="1f78e-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="1f78e-151">managedDeviceId</span></span>|<span data-ttu-id="1f78e-152">Строка</span><span class="sxs-lookup"><span data-stu-id="1f78e-152">String</span></span>|<span data-ttu-id="1f78e-153">Управляемые устройства идентификатор устройства узла.</span><span class="sxs-lookup"><span data-stu-id="1f78e-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="1f78e-154">Значение может быть пустой, даже в том случае, если управляемые устройства узла.</span><span class="sxs-lookup"><span data-stu-id="1f78e-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="1f78e-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="1f78e-155">azureADDeviceId</span></span>|<span data-ttu-id="1f78e-156">String</span><span class="sxs-lookup"><span data-stu-id="1f78e-156">String</span></span>|<span data-ttu-id="1f78e-157">Идентификатор Azure Active Directory устройства устройства узла.</span><span class="sxs-lookup"><span data-stu-id="1f78e-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="1f78e-158">Значение может быть пустым, даже в том случае, если устройство узла — это Azure Active Directory зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="1f78e-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="1f78e-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="1f78e-159">deviceModel</span></span>|<span data-ttu-id="1f78e-160">String</span><span class="sxs-lookup"><span data-stu-id="1f78e-160">String</span></span>|<span data-ttu-id="1f78e-161">Модель устройства для текущего Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="1f78e-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="1f78e-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="1f78e-162">deviceManufacturer</span></span>|<span data-ttu-id="1f78e-163">Строка</span><span class="sxs-lookup"><span data-stu-id="1f78e-163">String</span></span>|<span data-ttu-id="1f78e-164">Производитель устройства для текущего Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="1f78e-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="1f78e-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="1f78e-165">flaggedReasons</span></span>|<span data-ttu-id="1f78e-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1f78e-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="1f78e-167">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="1f78e-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="1f78e-168">например</span><span class="sxs-lookup"><span data-stu-id="1f78e-168">E.g.</span></span> <span data-ttu-id="1f78e-169">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="1f78e-169">app running on rooted device</span></span>|
|<span data-ttu-id="1f78e-170">userId</span><span class="sxs-lookup"><span data-stu-id="1f78e-170">userId</span></span>|<span data-ttu-id="1f78e-171">String</span><span class="sxs-lookup"><span data-stu-id="1f78e-171">String</span></span>|<span data-ttu-id="1f78e-172">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="1f78e-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="1f78e-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="1f78e-173">appIdentifier</span></span>|[<span data-ttu-id="1f78e-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="1f78e-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="1f78e-175">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="1f78e-175">The app package Identifier</span></span>|
|<span data-ttu-id="1f78e-176">id</span><span class="sxs-lookup"><span data-stu-id="1f78e-176">id</span></span>|<span data-ttu-id="1f78e-177">Строка</span><span class="sxs-lookup"><span data-stu-id="1f78e-177">String</span></span>|<span data-ttu-id="1f78e-178">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1f78e-178">Key of the entity.</span></span>|
|<span data-ttu-id="1f78e-179">version</span><span class="sxs-lookup"><span data-stu-id="1f78e-179">version</span></span>|<span data-ttu-id="1f78e-180">Строка</span><span class="sxs-lookup"><span data-stu-id="1f78e-180">String</span></span>|<span data-ttu-id="1f78e-181">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="1f78e-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f78e-182">Связи</span><span class="sxs-lookup"><span data-stu-id="1f78e-182">Relationships</span></span>
|<span data-ttu-id="1f78e-183">Связь</span><span class="sxs-lookup"><span data-stu-id="1f78e-183">Relationship</span></span>|<span data-ttu-id="1f78e-184">Тип</span><span class="sxs-lookup"><span data-stu-id="1f78e-184">Type</span></span>|<span data-ttu-id="1f78e-185">Описание</span><span class="sxs-lookup"><span data-stu-id="1f78e-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f78e-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="1f78e-186">appliedPolicies</span></span>|<span data-ttu-id="1f78e-187">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1f78e-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="1f78e-188">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="1f78e-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="1f78e-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="1f78e-189">intendedPolicies</span></span>|<span data-ttu-id="1f78e-190">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1f78e-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="1f78e-191">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="1f78e-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="1f78e-192">operations</span><span class="sxs-lookup"><span data-stu-id="1f78e-192">operations</span></span>|<span data-ttu-id="1f78e-193">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="1f78e-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="1f78e-194">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="1f78e-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1f78e-195">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f78e-195">JSON Representation</span></span>
<span data-ttu-id="1f78e-196">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f78e-196">Here is a JSON representation of the resource.</span></span>
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





