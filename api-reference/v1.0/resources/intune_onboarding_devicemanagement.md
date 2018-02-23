# <a name="devicemanagement-resource-type"></a><span data-ttu-id="f8555-101">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f8555-101">deviceManagement resource type</span></span>

> <span data-ttu-id="f8555-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f8555-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8555-103">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="f8555-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="f8555-104">Методы</span><span class="sxs-lookup"><span data-stu-id="f8555-104">Methods</span></span>
|<span data-ttu-id="f8555-105">Метод</span><span class="sxs-lookup"><span data-stu-id="f8555-105">Method</span></span>|<span data-ttu-id="f8555-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f8555-106">Return Type</span></span>|<span data-ttu-id="f8555-107">Описание</span><span class="sxs-lookup"><span data-stu-id="f8555-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f8555-108">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f8555-108">Get deviceManagement</span></span>](../api/intune_onboarding_devicemanagement_get.md)|[<span data-ttu-id="f8555-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f8555-109">deviceManagement</span></span>](../resources/intune_onboarding_devicemanagement.md)|<span data-ttu-id="f8555-110">Чтение свойств и связей объекта [deviceManagement](../resources/intune_onboarding_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="f8555-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_onboarding_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="f8555-111">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f8555-111">Update deviceManagement</span></span>](../api/intune_onboarding_devicemanagement_update.md)|[<span data-ttu-id="f8555-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f8555-112">deviceManagement</span></span>](../resources/intune_onboarding_devicemanagement.md)|<span data-ttu-id="f8555-113">Обновление свойств объекта [deviceManagement](../resources/intune_onboarding_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="f8555-113">Update the properties of a [calendar](../resources/intune_onboarding_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="f8555-114">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="f8555-114">verifyWindowsEnrollmentAutoDiscovery function</span></span>](../api/intune_onboarding_devicemanagement_verifywindowsenrollmentautodiscovery.md)|<span data-ttu-id="f8555-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8555-115">Boolean</span></span>|<span data-ttu-id="f8555-116">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f8555-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f8555-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8555-117">Properties</span></span>
|<span data-ttu-id="f8555-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8555-118">Property</span></span>|<span data-ttu-id="f8555-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f8555-119">Type</span></span>|<span data-ttu-id="f8555-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f8555-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8555-121">id</span><span class="sxs-lookup"><span data-stu-id="f8555-121">id</span></span>|<span data-ttu-id="f8555-122">String</span><span class="sxs-lookup"><span data-stu-id="f8555-122">String</span></span>|<span data-ttu-id="f8555-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f8555-123">Not yet documented</span></span>|
|<span data-ttu-id="f8555-124">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="f8555-124">intuneBrand</span></span>|[<span data-ttu-id="f8555-125">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="f8555-125">intuneBrand</span></span>](../resources/intune_onboarding_intunebrand.md)|<span data-ttu-id="f8555-126">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="f8555-126">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8555-127">Связи</span><span class="sxs-lookup"><span data-stu-id="f8555-127">Relationships</span></span>
|<span data-ttu-id="f8555-128">Связь</span><span class="sxs-lookup"><span data-stu-id="f8555-128">Relationship</span></span>|<span data-ttu-id="f8555-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f8555-129">Type</span></span>|<span data-ttu-id="f8555-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f8555-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8555-131">Объекты deviceCategory</span><span class="sxs-lookup"><span data-stu-id="f8555-131">deviceCategories</span></span>|<span data-ttu-id="f8555-132">Коллекция объектов [deviceCategory](../resources/intune_onboarding_devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="f8555-132">[deviceCategory](../resources/intune_onboarding_devicecategory.md) collection</span></span>|<span data-ttu-id="f8555-133">Список категорий устройств в клиенте.</span><span class="sxs-lookup"><span data-stu-id="f8555-133">The list of device categories with the tenant.</span></span>|
|<span data-ttu-id="f8555-134">Объекты exchangeConnector</span><span class="sxs-lookup"><span data-stu-id="f8555-134">exchangeConnectors</span></span>|<span data-ttu-id="f8555-135">Коллекция объектов [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)</span><span class="sxs-lookup"><span data-stu-id="f8555-135">[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) collection</span></span>|<span data-ttu-id="f8555-136">Список соединителей Exchange, настроенных с помощью клиента.</span><span class="sxs-lookup"><span data-stu-id="f8555-136">The list of Exchange Connectors configured by the tenant.</span></span>|
|<span data-ttu-id="f8555-137">Объекты deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8555-137">deviceEnrollmentConfigurations</span></span>|<span data-ttu-id="f8555-138">Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8555-138">[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="f8555-139">Список настроек регистрации устройств.</span><span class="sxs-lookup"><span data-stu-id="f8555-139">The list of device enrollment configurations</span></span>|
|<span data-ttu-id="f8555-140">conditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f8555-140">conditionalAccessSettings</span></span>|[<span data-ttu-id="f8555-141">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="f8555-141">onpremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="f8555-142">Параметры локального условного доступа в Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8555-142">The Exchange on premises conditional access settings.</span></span> <span data-ttu-id="f8555-143">Для локального условного доступа устройства должны быть зарегистрированы для доступа к почте и поддерживать его.</span><span class="sxs-lookup"><span data-stu-id="f8555-143">On premises conditional access will require devices to be both enrolled and compliant for mail access</span></span>|
|<span data-ttu-id="f8555-144">Объекты mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="f8555-144">mobileThreatDefenseConnectors</span></span>|<span data-ttu-id="f8555-145">Коллекция объектов [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)</span><span class="sxs-lookup"><span data-stu-id="f8555-145">[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) collection</span></span>|<span data-ttu-id="f8555-146">Список соединителей Mobile Threat Defense, настроенных с помощью клиента.</span><span class="sxs-lookup"><span data-stu-id="f8555-146">The list of Mobile threat Defense connectors configured by the tenant.</span></span>|
|<span data-ttu-id="f8555-147">Объекты deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="f8555-147">deviceManagementPartners</span></span>|<span data-ttu-id="f8555-148">Коллекция объектов [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="f8555-148">[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) collection</span></span>|<span data-ttu-id="f8555-149">Список партнеров по управлению устройствами, настроенных с помощью клиента.</span><span class="sxs-lookup"><span data-stu-id="f8555-149">The list of Device Management Partners configured by the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8555-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8555-150">JSON Representation</span></span>
<span data-ttu-id="f8555-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8555-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "displayName": "String",
    "contactITName": "String",
    "contactITPhoneNumber": "String",
    "contactITEmailAddress": "String",
    "contactITNotes": "String",
    "privacyUrl": "String",
    "onlineSupportSiteUrl": "String",
    "onlineSupportSiteName": "String",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1024,
      "g": 1024,
      "b": 1024
    },
    "showLogo": true,
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "String",
      "value": "binary"
    },
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "String",
      "value": "binary"
    },
    "showNameNextToLogo": true,
    "showDisplayNameNextToLogo": true
  }
}
```



