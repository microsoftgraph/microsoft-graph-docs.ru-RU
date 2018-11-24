# <a name="managedappregistration-resource-type"></a><span data-ttu-id="ba5e8-101">Тип ресурса managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ba5e8-101">managedAppRegistration resource type</span></span>

> <span data-ttu-id="ba5e8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba5e8-103">ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-103">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="ba5e8-104">Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-104">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="ba5e8-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ba5e8-105">Methods</span></span>
|<span data-ttu-id="ba5e8-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ba5e8-106">Method</span></span>|<span data-ttu-id="ba5e8-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ba5e8-107">Return Type</span></span>|<span data-ttu-id="ba5e8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ba5e8-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ba5e8-109">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ba5e8-109">List managedAppRegistrations</span></span>](../api/intune_mam_managedappregistration_list.md)|<span data-ttu-id="ba5e8-110">Коллекция объектов [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="ba5e8-110">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="ba5e8-111">Список свойств и связей объектов [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ba5e8-111">List properties and relationships of the [managedAppRegistration](../resources/intune_mam_managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="ba5e8-112">Получение объекта managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ba5e8-112">Get managedAppRegistration</span></span>](../api/intune_mam_managedappregistration_get.md)|[<span data-ttu-id="ba5e8-113">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ba5e8-113">managedAppRegistration</span></span>](../resources/intune_mam_managedappregistration.md)|<span data-ttu-id="ba5e8-114">Чтение свойств и связей объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="ba5e8-114">Read properties and relationships of the [managedAppRegistration](../resources/intune_mam_managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="ba5e8-115">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ba5e8-115">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune_mam_managedappregistration_getuseridswithflaggedappregistration.md)|<span data-ttu-id="ba5e8-116">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="ba5e8-116">String collection</span></span>|<span data-ttu-id="ba5e8-117">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ba5e8-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ba5e8-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba5e8-118">Properties</span></span>
|<span data-ttu-id="ba5e8-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba5e8-119">Property</span></span>|<span data-ttu-id="ba5e8-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ba5e8-120">Type</span></span>|<span data-ttu-id="ba5e8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ba5e8-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba5e8-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba5e8-122">createdDateTime</span></span>|<span data-ttu-id="ba5e8-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba5e8-123">DateTimeOffset</span></span>|<span data-ttu-id="ba5e8-124">Дата и время создания.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-124">Date and time of creation</span></span>|
|<span data-ttu-id="ba5e8-125">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ba5e8-125">lastSyncDateTime</span></span>|<span data-ttu-id="ba5e8-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba5e8-126">DateTimeOffset</span></span>|<span data-ttu-id="ba5e8-127">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-127">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="ba5e8-128">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="ba5e8-128">applicationVersion</span></span>|<span data-ttu-id="ba5e8-129">String</span><span class="sxs-lookup"><span data-stu-id="ba5e8-129">String</span></span>|<span data-ttu-id="ba5e8-130">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-130">App version</span></span>|
|<span data-ttu-id="ba5e8-131">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="ba5e8-131">managementSdkVersion</span></span>|<span data-ttu-id="ba5e8-132">String</span><span class="sxs-lookup"><span data-stu-id="ba5e8-132">String</span></span>|<span data-ttu-id="ba5e8-133">Версия пакета SDK для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-133">App management SDK version</span></span>|
|<span data-ttu-id="ba5e8-134">platformVersion</span><span class="sxs-lookup"><span data-stu-id="ba5e8-134">platformVersion</span></span>|<span data-ttu-id="ba5e8-135">String</span><span class="sxs-lookup"><span data-stu-id="ba5e8-135">String</span></span>|<span data-ttu-id="ba5e8-136">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-136">Operating System version</span></span>|
|<span data-ttu-id="ba5e8-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="ba5e8-137">deviceType</span></span>|<span data-ttu-id="ba5e8-138">String</span><span class="sxs-lookup"><span data-stu-id="ba5e8-138">String</span></span>|<span data-ttu-id="ba5e8-139">Тип главного устройства.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-139">Host device type</span></span>|
|<span data-ttu-id="ba5e8-140">deviceTag</span><span class="sxs-lookup"><span data-stu-id="ba5e8-140">deviceTag</span></span>|<span data-ttu-id="ba5e8-141">String</span><span class="sxs-lookup"><span data-stu-id="ba5e8-141">String</span></span>|<span data-ttu-id="ba5e8-142">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-142">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="ba5e8-143">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-143">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="ba5e8-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="ba5e8-144">deviceName</span></span>|<span data-ttu-id="ba5e8-145">String</span><span class="sxs-lookup"><span data-stu-id="ba5e8-145">String</span></span>|<span data-ttu-id="ba5e8-146">Имя главного устройства.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-146">Host device name</span></span>|
|<span data-ttu-id="ba5e8-147">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="ba5e8-147">flaggedReasons</span></span>|<span data-ttu-id="ba5e8-148">[managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ba5e8-148">[managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="ba5e8-149">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="ba5e8-149">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="ba5e8-150">например</span><span class="sxs-lookup"><span data-stu-id="ba5e8-150">E.g.</span></span> <span data-ttu-id="ba5e8-151">приложения, запущенного на устройстве с административным доступом.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-151">app running on rooted device</span></span>|
|<span data-ttu-id="ba5e8-152">userId</span><span class="sxs-lookup"><span data-stu-id="ba5e8-152">userId</span></span>|<span data-ttu-id="ba5e8-153">String</span><span class="sxs-lookup"><span data-stu-id="ba5e8-153">String</span></span>|<span data-ttu-id="ba5e8-154">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-154">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="ba5e8-155">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="ba5e8-155">appIdentifier</span></span>|[<span data-ttu-id="ba5e8-156">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ba5e8-156">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="ba5e8-157">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-157">The app package Identifier</span></span>|
|<span data-ttu-id="ba5e8-158">id</span><span class="sxs-lookup"><span data-stu-id="ba5e8-158">id</span></span>|<span data-ttu-id="ba5e8-159">String</span><span class="sxs-lookup"><span data-stu-id="ba5e8-159">String</span></span>|<span data-ttu-id="ba5e8-160">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-160">Key of the entity.</span></span>|
|<span data-ttu-id="ba5e8-161">version</span><span class="sxs-lookup"><span data-stu-id="ba5e8-161">version</span></span>|<span data-ttu-id="ba5e8-162">String</span><span class="sxs-lookup"><span data-stu-id="ba5e8-162">String</span></span>|<span data-ttu-id="ba5e8-163">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-163">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba5e8-164">Связи</span><span class="sxs-lookup"><span data-stu-id="ba5e8-164">Relationships</span></span>
|<span data-ttu-id="ba5e8-165">Связь</span><span class="sxs-lookup"><span data-stu-id="ba5e8-165">Relationship</span></span>|<span data-ttu-id="ba5e8-166">Тип</span><span class="sxs-lookup"><span data-stu-id="ba5e8-166">Type</span></span>|<span data-ttu-id="ba5e8-167">Описание</span><span class="sxs-lookup"><span data-stu-id="ba5e8-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba5e8-168">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="ba5e8-168">appliedPolicies</span></span>|<span data-ttu-id="ba5e8-169">Коллекция объектов [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ba5e8-169">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="ba5e8-170">Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-170">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="ba5e8-171">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="ba5e8-171">intendedPolicies</span></span>|<span data-ttu-id="ba5e8-172">Коллекция объектов [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ba5e8-172">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="ba5e8-173">Нуль или более политик, которые на текущий момент администратор использует для приложения.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-173">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="ba5e8-174">operations</span><span class="sxs-lookup"><span data-stu-id="ba5e8-174">operations</span></span>|<span data-ttu-id="ba5e8-175">Коллекция объектов [managedAppOperation](../resources/intune_mam_managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="ba5e8-175">[managedAppOperation](../resources/intune_mam_managedappoperation.md) collection</span></span>|<span data-ttu-id="ba5e8-176">Нуль или более долговременных операций, запускаемых для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-176">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba5e8-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba5e8-177">JSON Representation</span></span>
<span data-ttu-id="ba5e8-178">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba5e8-178">Here is a JSON representation of the resource.</span></span>
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
     "Warning: /api-reference/v1.0/resources/intune_mam_managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->
