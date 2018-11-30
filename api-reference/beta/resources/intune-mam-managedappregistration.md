---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.
ms.openlocfilehash: bf05e7180f27be9c813f8fbb05346893fa6db172
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077783"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="8494c-103">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8494c-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="8494c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8494c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8494c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8494c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8494c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8494c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8494c-107">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="8494c-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="8494c-108">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="8494c-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="8494c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="8494c-109">Methods</span></span>
|<span data-ttu-id="8494c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="8494c-110">Method</span></span>|<span data-ttu-id="8494c-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8494c-111">Return Type</span></span>|<span data-ttu-id="8494c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8494c-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8494c-113">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8494c-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="8494c-114">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="8494c-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="8494c-115">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8494c-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="8494c-116">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8494c-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="8494c-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8494c-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="8494c-118">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8494c-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="8494c-119">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8494c-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="8494c-120">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="8494c-120">String collection</span></span>|<span data-ttu-id="8494c-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8494c-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8494c-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="8494c-122">Properties</span></span>
|<span data-ttu-id="8494c-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="8494c-123">Property</span></span>|<span data-ttu-id="8494c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="8494c-124">Type</span></span>|<span data-ttu-id="8494c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="8494c-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8494c-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8494c-126">createdDateTime</span></span>|<span data-ttu-id="8494c-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8494c-127">DateTimeOffset</span></span>|<span data-ttu-id="8494c-128">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="8494c-128">Date and time of creation</span></span>|
|<span data-ttu-id="8494c-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8494c-129">lastSyncDateTime</span></span>|<span data-ttu-id="8494c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8494c-130">DateTimeOffset</span></span>|<span data-ttu-id="8494c-131">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="8494c-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="8494c-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="8494c-132">applicationVersion</span></span>|<span data-ttu-id="8494c-133">String</span><span class="sxs-lookup"><span data-stu-id="8494c-133">String</span></span>|<span data-ttu-id="8494c-134">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="8494c-134">App version</span></span>|
|<span data-ttu-id="8494c-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="8494c-135">managementSdkVersion</span></span>|<span data-ttu-id="8494c-136">String</span><span class="sxs-lookup"><span data-stu-id="8494c-136">String</span></span>|<span data-ttu-id="8494c-137">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="8494c-137">App management SDK version</span></span>|
|<span data-ttu-id="8494c-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="8494c-138">platformVersion</span></span>|<span data-ttu-id="8494c-139">String</span><span class="sxs-lookup"><span data-stu-id="8494c-139">String</span></span>|<span data-ttu-id="8494c-140">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="8494c-140">Operating System version</span></span>|
|<span data-ttu-id="8494c-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="8494c-141">deviceType</span></span>|<span data-ttu-id="8494c-142">String</span><span class="sxs-lookup"><span data-stu-id="8494c-142">String</span></span>|<span data-ttu-id="8494c-143">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="8494c-143">Host device type</span></span>|
|<span data-ttu-id="8494c-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="8494c-144">deviceTag</span></span>|<span data-ttu-id="8494c-145">String</span><span class="sxs-lookup"><span data-stu-id="8494c-145">String</span></span>|<span data-ttu-id="8494c-146">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="8494c-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="8494c-147">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="8494c-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="8494c-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="8494c-148">deviceName</span></span>|<span data-ttu-id="8494c-149">String</span><span class="sxs-lookup"><span data-stu-id="8494c-149">String</span></span>|<span data-ttu-id="8494c-150">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="8494c-150">Host device name</span></span>|
|<span data-ttu-id="8494c-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="8494c-151">managedDeviceId</span></span>|<span data-ttu-id="8494c-152">String</span><span class="sxs-lookup"><span data-stu-id="8494c-152">String</span></span>|<span data-ttu-id="8494c-153">Управляемые устройства идентификатор устройства узла.</span><span class="sxs-lookup"><span data-stu-id="8494c-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="8494c-154">Значение может быть пустой, даже в том случае, если управляемые устройства узла.</span><span class="sxs-lookup"><span data-stu-id="8494c-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="8494c-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="8494c-155">azureADDeviceId</span></span>|<span data-ttu-id="8494c-156">String</span><span class="sxs-lookup"><span data-stu-id="8494c-156">String</span></span>|<span data-ttu-id="8494c-157">Идентификатор Azure Active Directory устройства устройства узла.</span><span class="sxs-lookup"><span data-stu-id="8494c-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="8494c-158">Значение может быть пустым, даже в том случае, если устройство узла — это Azure Active Directory зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="8494c-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="8494c-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="8494c-159">deviceModel</span></span>|<span data-ttu-id="8494c-160">String</span><span class="sxs-lookup"><span data-stu-id="8494c-160">String</span></span>|<span data-ttu-id="8494c-161">Модель устройства для текущего Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="8494c-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="8494c-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="8494c-162">deviceManufacturer</span></span>|<span data-ttu-id="8494c-163">String</span><span class="sxs-lookup"><span data-stu-id="8494c-163">String</span></span>|<span data-ttu-id="8494c-164">Производитель устройства для текущего Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="8494c-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="8494c-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="8494c-165">flaggedReasons</span></span>|<span data-ttu-id="8494c-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8494c-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="8494c-167">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="8494c-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="8494c-168">например</span><span class="sxs-lookup"><span data-stu-id="8494c-168">E.g.</span></span> <span data-ttu-id="8494c-169">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="8494c-169">app running on rooted device</span></span>|
|<span data-ttu-id="8494c-170">userId</span><span class="sxs-lookup"><span data-stu-id="8494c-170">userId</span></span>|<span data-ttu-id="8494c-171">String</span><span class="sxs-lookup"><span data-stu-id="8494c-171">String</span></span>|<span data-ttu-id="8494c-172">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="8494c-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="8494c-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="8494c-173">appIdentifier</span></span>|[<span data-ttu-id="8494c-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8494c-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="8494c-175">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="8494c-175">The app package Identifier</span></span>|
|<span data-ttu-id="8494c-176">id</span><span class="sxs-lookup"><span data-stu-id="8494c-176">id</span></span>|<span data-ttu-id="8494c-177">String</span><span class="sxs-lookup"><span data-stu-id="8494c-177">String</span></span>|<span data-ttu-id="8494c-178">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8494c-178">Key of the entity.</span></span>|
|<span data-ttu-id="8494c-179">version</span><span class="sxs-lookup"><span data-stu-id="8494c-179">version</span></span>|<span data-ttu-id="8494c-180">String</span><span class="sxs-lookup"><span data-stu-id="8494c-180">String</span></span>|<span data-ttu-id="8494c-181">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="8494c-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8494c-182">Связи</span><span class="sxs-lookup"><span data-stu-id="8494c-182">Relationships</span></span>
|<span data-ttu-id="8494c-183">Связь</span><span class="sxs-lookup"><span data-stu-id="8494c-183">Relationship</span></span>|<span data-ttu-id="8494c-184">Тип</span><span class="sxs-lookup"><span data-stu-id="8494c-184">Type</span></span>|<span data-ttu-id="8494c-185">Описание</span><span class="sxs-lookup"><span data-stu-id="8494c-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8494c-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="8494c-186">appliedPolicies</span></span>|<span data-ttu-id="8494c-187">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8494c-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="8494c-188">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="8494c-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="8494c-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="8494c-189">intendedPolicies</span></span>|<span data-ttu-id="8494c-190">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8494c-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="8494c-191">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="8494c-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="8494c-192">operations</span><span class="sxs-lookup"><span data-stu-id="8494c-192">operations</span></span>|<span data-ttu-id="8494c-193">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="8494c-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="8494c-194">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="8494c-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8494c-195">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8494c-195">JSON Representation</span></span>
<span data-ttu-id="8494c-196">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8494c-196">Here is a JSON representation of the resource.</span></span>
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





