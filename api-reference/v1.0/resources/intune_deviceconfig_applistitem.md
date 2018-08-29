# <a name="applistitem-resource-type"></a><span data-ttu-id="bf7b3-101">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="bf7b3-101">appListItem resource type</span></span>

> <span data-ttu-id="bf7b3-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bf7b3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf7b3-103">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="bf7b3-103">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="bf7b3-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf7b3-104">Properties</span></span>
|<span data-ttu-id="bf7b3-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf7b3-105">Property</span></span>|<span data-ttu-id="bf7b3-106">Тип</span><span class="sxs-lookup"><span data-stu-id="bf7b3-106">Type</span></span>|<span data-ttu-id="bf7b3-107">Описание</span><span class="sxs-lookup"><span data-stu-id="bf7b3-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf7b3-108">name</span><span class="sxs-lookup"><span data-stu-id="bf7b3-108">name</span></span>|<span data-ttu-id="bf7b3-109">String</span><span class="sxs-lookup"><span data-stu-id="bf7b3-109">String</span></span>|<span data-ttu-id="bf7b3-110">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="bf7b3-110">The application name</span></span>|
|<span data-ttu-id="bf7b3-111">publisher</span><span class="sxs-lookup"><span data-stu-id="bf7b3-111">publisher</span></span>|<span data-ttu-id="bf7b3-112">String</span><span class="sxs-lookup"><span data-stu-id="bf7b3-112">String</span></span>|<span data-ttu-id="bf7b3-113">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="bf7b3-113">The publisher of the application</span></span>|
|<span data-ttu-id="bf7b3-114">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="bf7b3-114">appStoreUrl</span></span>|<span data-ttu-id="bf7b3-115">String</span><span class="sxs-lookup"><span data-stu-id="bf7b3-115">String</span></span>|<span data-ttu-id="bf7b3-116">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="bf7b3-116">The Store URL of the application</span></span>|
|<span data-ttu-id="bf7b3-117">appId</span><span class="sxs-lookup"><span data-stu-id="bf7b3-117">appId</span></span>|<span data-ttu-id="bf7b3-118">String</span><span class="sxs-lookup"><span data-stu-id="bf7b3-118">String</span></span>|<span data-ttu-id="bf7b3-119">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="bf7b3-119">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf7b3-120">Связи</span><span class="sxs-lookup"><span data-stu-id="bf7b3-120">Relationships</span></span>
<span data-ttu-id="bf7b3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="bf7b3-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bf7b3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf7b3-122">JSON Representation</span></span>
<span data-ttu-id="bf7b3-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf7b3-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



