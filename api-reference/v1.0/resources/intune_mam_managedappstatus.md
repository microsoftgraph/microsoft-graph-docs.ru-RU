# <a name="managedappstatus-resource-type"></a><span data-ttu-id="c4069-101">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="c4069-101">managedAppStatus resource type</span></span>

> <span data-ttu-id="c4069-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c4069-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4069-103">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="c4069-103">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="c4069-104">Методы</span><span class="sxs-lookup"><span data-stu-id="c4069-104">Methods</span></span>
|<span data-ttu-id="c4069-105">Метод</span><span class="sxs-lookup"><span data-stu-id="c4069-105">Method</span></span>|<span data-ttu-id="c4069-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c4069-106">Return Type</span></span>|<span data-ttu-id="c4069-107">Описание</span><span class="sxs-lookup"><span data-stu-id="c4069-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c4069-108">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="c4069-108">List managedAppStatuses</span></span>](../api/intune_mam_managedappstatus_list.md)|<span data-ttu-id="c4069-109">Коллекция [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c4069-109">[managedAppStatus](../resources/intune_mam_managedappstatus.md) collection</span></span>|<span data-ttu-id="c4069-110">Список свойств и связей объектов [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c4069-110">List properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="c4069-111">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="c4069-111">Get managedAppStatus</span></span>](../api/intune_mam_managedappstatus_get.md)|[<span data-ttu-id="c4069-112">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="c4069-112">managedAppStatus</span></span>](../resources/intune_mam_managedappstatus.md)|<span data-ttu-id="c4069-113">Чтение свойств и связей объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c4069-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c4069-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4069-114">Properties</span></span>
|<span data-ttu-id="c4069-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4069-115">Property</span></span>|<span data-ttu-id="c4069-116">Тип</span><span class="sxs-lookup"><span data-stu-id="c4069-116">Type</span></span>|<span data-ttu-id="c4069-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c4069-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4069-118">displayName</span><span class="sxs-lookup"><span data-stu-id="c4069-118">displayName</span></span>|<span data-ttu-id="c4069-119">String</span><span class="sxs-lookup"><span data-stu-id="c4069-119">String</span></span>|<span data-ttu-id="c4069-120">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="c4069-120">Friendly name of the status report.</span></span>|
|<span data-ttu-id="c4069-121">id</span><span class="sxs-lookup"><span data-stu-id="c4069-121">id</span></span>|<span data-ttu-id="c4069-122">String</span><span class="sxs-lookup"><span data-stu-id="c4069-122">String</span></span>|<span data-ttu-id="c4069-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c4069-123">Key of the setting.</span></span>|
|<span data-ttu-id="c4069-124">version</span><span class="sxs-lookup"><span data-stu-id="c4069-124">version</span></span>|<span data-ttu-id="c4069-125">String</span><span class="sxs-lookup"><span data-stu-id="c4069-125">String</span></span>|<span data-ttu-id="c4069-126">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="c4069-126">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4069-127">Связи</span><span class="sxs-lookup"><span data-stu-id="c4069-127">Relationships</span></span>
<span data-ttu-id="c4069-128">Нет</span><span class="sxs-lookup"><span data-stu-id="c4069-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c4069-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4069-129">JSON Representation</span></span>
<span data-ttu-id="c4069-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4069-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



