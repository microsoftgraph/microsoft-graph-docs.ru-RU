---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 69d532f7c8287b678c1f62f5b8b78c6e4a99d2ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944819"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="45216-103">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="45216-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="45216-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45216-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45216-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45216-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45216-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="45216-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45216-107">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="45216-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="45216-108">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="45216-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="45216-109">Методы</span><span class="sxs-lookup"><span data-stu-id="45216-109">Methods</span></span>
|<span data-ttu-id="45216-110">Метод</span><span class="sxs-lookup"><span data-stu-id="45216-110">Method</span></span>|<span data-ttu-id="45216-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="45216-111">Return Type</span></span>|<span data-ttu-id="45216-112">Описание</span><span class="sxs-lookup"><span data-stu-id="45216-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="45216-113">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="45216-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="45216-114">Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="45216-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="45216-115">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="45216-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="45216-116">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="45216-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="45216-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="45216-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="45216-118">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="45216-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="45216-119">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="45216-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="45216-120">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="45216-120">String collection</span></span>|<span data-ttu-id="45216-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="45216-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="45216-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="45216-122">Properties</span></span>
|<span data-ttu-id="45216-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="45216-123">Property</span></span>|<span data-ttu-id="45216-124">Тип</span><span class="sxs-lookup"><span data-stu-id="45216-124">Type</span></span>|<span data-ttu-id="45216-125">Описание</span><span class="sxs-lookup"><span data-stu-id="45216-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45216-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45216-126">createdDateTime</span></span>|<span data-ttu-id="45216-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45216-127">DateTimeOffset</span></span>|<span data-ttu-id="45216-128">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="45216-128">Date and time of creation</span></span>|
|<span data-ttu-id="45216-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="45216-129">lastSyncDateTime</span></span>|<span data-ttu-id="45216-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45216-130">DateTimeOffset</span></span>|<span data-ttu-id="45216-131">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="45216-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="45216-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="45216-132">applicationVersion</span></span>|<span data-ttu-id="45216-133">String</span><span class="sxs-lookup"><span data-stu-id="45216-133">String</span></span>|<span data-ttu-id="45216-134">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="45216-134">App version</span></span>|
|<span data-ttu-id="45216-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="45216-135">managementSdkVersion</span></span>|<span data-ttu-id="45216-136">String</span><span class="sxs-lookup"><span data-stu-id="45216-136">String</span></span>|<span data-ttu-id="45216-137">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="45216-137">App management SDK version</span></span>|
|<span data-ttu-id="45216-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="45216-138">platformVersion</span></span>|<span data-ttu-id="45216-139">String</span><span class="sxs-lookup"><span data-stu-id="45216-139">String</span></span>|<span data-ttu-id="45216-140">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="45216-140">Operating System version</span></span>|
|<span data-ttu-id="45216-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="45216-141">deviceType</span></span>|<span data-ttu-id="45216-142">String</span><span class="sxs-lookup"><span data-stu-id="45216-142">String</span></span>|<span data-ttu-id="45216-143">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="45216-143">Host device type</span></span>|
|<span data-ttu-id="45216-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="45216-144">deviceTag</span></span>|<span data-ttu-id="45216-145">String</span><span class="sxs-lookup"><span data-stu-id="45216-145">String</span></span>|<span data-ttu-id="45216-146">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="45216-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="45216-147">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="45216-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="45216-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="45216-148">deviceName</span></span>|<span data-ttu-id="45216-149">String</span><span class="sxs-lookup"><span data-stu-id="45216-149">String</span></span>|<span data-ttu-id="45216-150">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="45216-150">Host device name</span></span>|
|<span data-ttu-id="45216-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="45216-151">managedDeviceId</span></span>|<span data-ttu-id="45216-152">Строка</span><span class="sxs-lookup"><span data-stu-id="45216-152">String</span></span>|<span data-ttu-id="45216-153">Управляемые устройства идентификатор устройства узла.</span><span class="sxs-lookup"><span data-stu-id="45216-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="45216-154">Значение может быть пустой, даже в том случае, если управляемые устройства узла.</span><span class="sxs-lookup"><span data-stu-id="45216-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="45216-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="45216-155">azureADDeviceId</span></span>|<span data-ttu-id="45216-156">String</span><span class="sxs-lookup"><span data-stu-id="45216-156">String</span></span>|<span data-ttu-id="45216-157">Идентификатор Azure Active Directory устройства устройства узла.</span><span class="sxs-lookup"><span data-stu-id="45216-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="45216-158">Значение может быть пустым, даже в том случае, если устройство узла — это Azure Active Directory зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="45216-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="45216-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="45216-159">deviceModel</span></span>|<span data-ttu-id="45216-160">String</span><span class="sxs-lookup"><span data-stu-id="45216-160">String</span></span>|<span data-ttu-id="45216-161">Модель устройства для текущего Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="45216-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="45216-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="45216-162">deviceManufacturer</span></span>|<span data-ttu-id="45216-163">Строка</span><span class="sxs-lookup"><span data-stu-id="45216-163">String</span></span>|<span data-ttu-id="45216-164">Производитель устройства для текущего Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="45216-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="45216-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="45216-165">flaggedReasons</span></span>|<span data-ttu-id="45216-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="45216-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="45216-167">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="45216-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="45216-168">например</span><span class="sxs-lookup"><span data-stu-id="45216-168">E.g.</span></span> <span data-ttu-id="45216-169">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="45216-169">app running on rooted device</span></span>|
|<span data-ttu-id="45216-170">userId</span><span class="sxs-lookup"><span data-stu-id="45216-170">userId</span></span>|<span data-ttu-id="45216-171">String</span><span class="sxs-lookup"><span data-stu-id="45216-171">String</span></span>|<span data-ttu-id="45216-172">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="45216-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="45216-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="45216-173">appIdentifier</span></span>|[<span data-ttu-id="45216-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="45216-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="45216-175">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="45216-175">The app package Identifier</span></span>|
|<span data-ttu-id="45216-176">id</span><span class="sxs-lookup"><span data-stu-id="45216-176">id</span></span>|<span data-ttu-id="45216-177">Строка</span><span class="sxs-lookup"><span data-stu-id="45216-177">String</span></span>|<span data-ttu-id="45216-178">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="45216-178">Key of the entity.</span></span>|
|<span data-ttu-id="45216-179">version</span><span class="sxs-lookup"><span data-stu-id="45216-179">version</span></span>|<span data-ttu-id="45216-180">Строка</span><span class="sxs-lookup"><span data-stu-id="45216-180">String</span></span>|<span data-ttu-id="45216-181">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="45216-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45216-182">Связи</span><span class="sxs-lookup"><span data-stu-id="45216-182">Relationships</span></span>
|<span data-ttu-id="45216-183">Связь</span><span class="sxs-lookup"><span data-stu-id="45216-183">Relationship</span></span>|<span data-ttu-id="45216-184">Тип</span><span class="sxs-lookup"><span data-stu-id="45216-184">Type</span></span>|<span data-ttu-id="45216-185">Описание</span><span class="sxs-lookup"><span data-stu-id="45216-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45216-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="45216-186">appliedPolicies</span></span>|<span data-ttu-id="45216-187">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="45216-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="45216-188">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="45216-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="45216-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="45216-189">intendedPolicies</span></span>|<span data-ttu-id="45216-190">Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="45216-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="45216-191">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="45216-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="45216-192">operations</span><span class="sxs-lookup"><span data-stu-id="45216-192">operations</span></span>|<span data-ttu-id="45216-193">Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="45216-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="45216-194">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="45216-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45216-195">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45216-195">JSON Representation</span></span>
<span data-ttu-id="45216-196">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45216-196">Here is a JSON representation of the resource.</span></span>
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





