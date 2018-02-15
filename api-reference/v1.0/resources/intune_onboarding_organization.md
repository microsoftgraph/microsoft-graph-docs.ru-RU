# <a name="organization-resource-type"></a><span data-ttu-id="20b08-101">Тип ресурса organization</span><span class="sxs-lookup"><span data-stu-id="20b08-101">organization resource type</span></span>

> <span data-ttu-id="20b08-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="20b08-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20b08-103">Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="20b08-103">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="20b08-104">Методы</span><span class="sxs-lookup"><span data-stu-id="20b08-104">Methods</span></span>
|<span data-ttu-id="20b08-105">Метод</span><span class="sxs-lookup"><span data-stu-id="20b08-105">Method</span></span>|<span data-ttu-id="20b08-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="20b08-106">Return Type</span></span>|<span data-ttu-id="20b08-107">Описание</span><span class="sxs-lookup"><span data-stu-id="20b08-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="20b08-108">Список организаций</span><span class="sxs-lookup"><span data-stu-id="20b08-108">List organizations</span></span>](../api/intune_onboarding_organization_list.md)|<span data-ttu-id="20b08-109">Коллекция объектов [organization](../resources/intune_onboarding_organization.md)</span><span class="sxs-lookup"><span data-stu-id="20b08-109">[organization](../resources/intune_onboarding_organization.md) collection</span></span>|<span data-ttu-id="20b08-110">Список свойств и связей объектов [organization](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="20b08-110">List properties and relationships of the [organization](../resources/intune_onboarding_organization.md) objects.</span></span>|
|[<span data-ttu-id="20b08-111">Получение организации</span><span class="sxs-lookup"><span data-stu-id="20b08-111">Get organization</span></span>](../api/intune_onboarding_organization_get.md)|[<span data-ttu-id="20b08-112">organization</span><span class="sxs-lookup"><span data-stu-id="20b08-112">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="20b08-113">Чтение свойств и связей объекта [organization](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="20b08-113">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="20b08-114">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="20b08-114">Update organization</span></span>](../api/intune_onboarding_organization_update.md)|[<span data-ttu-id="20b08-115">organization</span><span class="sxs-lookup"><span data-stu-id="20b08-115">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="20b08-116">Обновление свойств объекта [organization](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="20b08-116">Update the properties of a [calendar](../resources/intune_onboarding_organization.md) object.</span></span>|
|[<span data-ttu-id="20b08-117">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="20b08-117">setMobileDeviceManagementAuthority action</span></span>](../api/intune_onboarding_organization_setmobiledevicemanagementauthority.md)|<span data-ttu-id="20b08-118">Int32</span><span class="sxs-lookup"><span data-stu-id="20b08-118">Int32</span></span>|<span data-ttu-id="20b08-119">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="20b08-119">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="20b08-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="20b08-120">Properties</span></span>
|<span data-ttu-id="20b08-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="20b08-121">Property</span></span>|<span data-ttu-id="20b08-122">Тип</span><span class="sxs-lookup"><span data-stu-id="20b08-122">Type</span></span>|<span data-ttu-id="20b08-123">Описание</span><span class="sxs-lookup"><span data-stu-id="20b08-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20b08-124">id</span><span class="sxs-lookup"><span data-stu-id="20b08-124">id</span></span>|<span data-ttu-id="20b08-125">String</span><span class="sxs-lookup"><span data-stu-id="20b08-125">String</span></span>|<span data-ttu-id="20b08-126">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="20b08-126">The resource GUID for the security object is not valid.</span></span>|
|<span data-ttu-id="20b08-127">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="20b08-127">mobileDeviceManagementAuthority</span></span>|<span data-ttu-id="20b08-128">String</span><span class="sxs-lookup"><span data-stu-id="20b08-128">String</span></span>|<span data-ttu-id="20b08-129">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="20b08-129">Mobile device management authority.</span></span> <span data-ttu-id="20b08-130">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="20b08-130">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20b08-131">Связи</span><span class="sxs-lookup"><span data-stu-id="20b08-131">Relationships</span></span>
<span data-ttu-id="20b08-132">Нет</span><span class="sxs-lookup"><span data-stu-id="20b08-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="20b08-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20b08-133">JSON Representation</span></span>
<span data-ttu-id="20b08-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20b08-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String"
}
```



