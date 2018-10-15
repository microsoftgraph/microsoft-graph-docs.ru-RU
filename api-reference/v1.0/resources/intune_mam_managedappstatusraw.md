# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="61097-101">Тип ресурса managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="61097-101">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="61097-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="61097-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61097-103">Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.</span><span class="sxs-lookup"><span data-stu-id="61097-103">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="61097-104">Наследуется от [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="61097-104">Inherits from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="61097-105">Методы</span><span class="sxs-lookup"><span data-stu-id="61097-105">Methods</span></span>
|<span data-ttu-id="61097-106">Метод</span><span class="sxs-lookup"><span data-stu-id="61097-106">Method</span></span>|<span data-ttu-id="61097-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="61097-107">Return Type</span></span>|<span data-ttu-id="61097-108">Описание</span><span class="sxs-lookup"><span data-stu-id="61097-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="61097-109">Перечисление managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="61097-109">List managedAppStatusRaws</span></span>](../api/intune_mam_managedappstatusraw_list.md)|<span data-ttu-id="61097-110">Коллекция [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="61097-110">[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) collection</span></span>|<span data-ttu-id="61097-111">Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="61097-111">List properties and relationships of the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="61097-112">Получение managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="61097-112">Get managedAppStatusRaw</span></span>](../api/intune_mam_managedappstatusraw_get.md)|[<span data-ttu-id="61097-113">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="61097-113">managedAppStatusRaw</span></span>](../resources/intune_mam_managedappstatusraw.md)|<span data-ttu-id="61097-114">Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="61097-114">Read properties and relationships of the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="61097-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="61097-115">Properties</span></span>
|<span data-ttu-id="61097-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="61097-116">Property</span></span>|<span data-ttu-id="61097-117">Тип</span><span class="sxs-lookup"><span data-stu-id="61097-117">Type</span></span>|<span data-ttu-id="61097-118">Описание</span><span class="sxs-lookup"><span data-stu-id="61097-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61097-119">displayName</span><span class="sxs-lookup"><span data-stu-id="61097-119">displayName</span></span>|<span data-ttu-id="61097-120">Строка</span><span class="sxs-lookup"><span data-stu-id="61097-120">String</span></span>|<span data-ttu-id="61097-121">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="61097-121">Friendly name of the status report.</span></span> <span data-ttu-id="61097-122">Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="61097-122">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="61097-123">id</span><span class="sxs-lookup"><span data-stu-id="61097-123">id</span></span>|<span data-ttu-id="61097-124">Строка</span><span class="sxs-lookup"><span data-stu-id="61097-124">String</span></span>|<span data-ttu-id="61097-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="61097-125">Key of the entity.</span></span> <span data-ttu-id="61097-126">Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="61097-126">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="61097-127">version</span><span class="sxs-lookup"><span data-stu-id="61097-127">version</span></span>|<span data-ttu-id="61097-128">Строка</span><span class="sxs-lookup"><span data-stu-id="61097-128">String</span></span>|<span data-ttu-id="61097-129">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="61097-129">Version of the entity.</span></span> <span data-ttu-id="61097-130">Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="61097-130">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="61097-131">content</span><span class="sxs-lookup"><span data-stu-id="61097-131">content</span></span>|[<span data-ttu-id="61097-132">Json</span><span class="sxs-lookup"><span data-stu-id="61097-132">Json</span></span>](../resources/json.md)|<span data-ttu-id="61097-133">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="61097-133">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61097-134">Связи</span><span class="sxs-lookup"><span data-stu-id="61097-134">Relationships</span></span>
<span data-ttu-id="61097-135">Нет</span><span class="sxs-lookup"><span data-stu-id="61097-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="61097-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61097-136">JSON Representation</span></span>
<span data-ttu-id="61097-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61097-137">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedAppStatus",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```








