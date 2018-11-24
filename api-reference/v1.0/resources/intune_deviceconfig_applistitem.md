# <a name="applistitem-resource-type"></a><span data-ttu-id="cd77f-101">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="cd77f-101">appListItem resource type</span></span>

> <span data-ttu-id="cd77f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cd77f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd77f-103">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="cd77f-103">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="cd77f-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd77f-104">Properties</span></span>
|<span data-ttu-id="cd77f-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd77f-105">Property</span></span>|<span data-ttu-id="cd77f-106">Тип</span><span class="sxs-lookup"><span data-stu-id="cd77f-106">Type</span></span>|<span data-ttu-id="cd77f-107">Описание</span><span class="sxs-lookup"><span data-stu-id="cd77f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd77f-108">name</span><span class="sxs-lookup"><span data-stu-id="cd77f-108">name</span></span>|<span data-ttu-id="cd77f-109">String</span><span class="sxs-lookup"><span data-stu-id="cd77f-109">String</span></span>|<span data-ttu-id="cd77f-110">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="cd77f-110">The application name</span></span>|
|<span data-ttu-id="cd77f-111">publisher</span><span class="sxs-lookup"><span data-stu-id="cd77f-111">publisher</span></span>|<span data-ttu-id="cd77f-112">String</span><span class="sxs-lookup"><span data-stu-id="cd77f-112">String</span></span>|<span data-ttu-id="cd77f-113">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="cd77f-113">The publisher of the application</span></span>|
|<span data-ttu-id="cd77f-114">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="cd77f-114">appStoreUrl</span></span>|<span data-ttu-id="cd77f-115">String</span><span class="sxs-lookup"><span data-stu-id="cd77f-115">String</span></span>|<span data-ttu-id="cd77f-116">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="cd77f-116">The Store URL of the application</span></span>|
|<span data-ttu-id="cd77f-117">appId</span><span class="sxs-lookup"><span data-stu-id="cd77f-117">appId</span></span>|<span data-ttu-id="cd77f-118">String</span><span class="sxs-lookup"><span data-stu-id="cd77f-118">String</span></span>|<span data-ttu-id="cd77f-119">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="cd77f-119">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd77f-120">Связи</span><span class="sxs-lookup"><span data-stu-id="cd77f-120">Relationships</span></span>
<span data-ttu-id="cd77f-121">Нет</span><span class="sxs-lookup"><span data-stu-id="cd77f-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cd77f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd77f-122">JSON Representation</span></span>
<span data-ttu-id="cd77f-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd77f-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



