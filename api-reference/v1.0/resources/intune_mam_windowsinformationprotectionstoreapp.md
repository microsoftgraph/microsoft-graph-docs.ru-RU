# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="54ba4-101">Тип ресурса windowsInformationProtectionStoreApp</span><span class="sxs-lookup"><span data-stu-id="54ba4-101">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="54ba4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="54ba4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54ba4-103">Защита данных приложений для Windows из Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="54ba4-103">Store App for Windows information protection</span></span>

<span data-ttu-id="54ba4-104">Наследуется от [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="54ba4-104">Inherits from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="54ba4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="54ba4-105">Properties</span></span>
|<span data-ttu-id="54ba4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="54ba4-106">Property</span></span>|<span data-ttu-id="54ba4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="54ba4-107">Type</span></span>|<span data-ttu-id="54ba4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="54ba4-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54ba4-109">displayName</span><span class="sxs-lookup"><span data-stu-id="54ba4-109">displayName</span></span>|<span data-ttu-id="54ba4-110">Строковый</span><span class="sxs-lookup"><span data-stu-id="54ba4-110">String</span></span>|<span data-ttu-id="54ba4-111">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="54ba4-111">App display name.</span></span> <span data-ttu-id="54ba4-112">Наследуется от [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="54ba4-112">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="54ba4-113">описание</span><span class="sxs-lookup"><span data-stu-id="54ba4-113">description</span></span>|<span data-ttu-id="54ba4-114">Строковый</span><span class="sxs-lookup"><span data-stu-id="54ba4-114">String</span></span>|<span data-ttu-id="54ba4-115">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="54ba4-115">The app's description.</span></span> <span data-ttu-id="54ba4-116">Наследуется от [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="54ba4-116">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="54ba4-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="54ba4-117">publisherName</span></span>|<span data-ttu-id="54ba4-118">Строковый</span><span class="sxs-lookup"><span data-stu-id="54ba4-118">String</span></span>|<span data-ttu-id="54ba4-119">Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="54ba4-119">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="54ba4-120">productName</span><span class="sxs-lookup"><span data-stu-id="54ba4-120">productName</span></span>|<span data-ttu-id="54ba4-121">Строковый</span><span class="sxs-lookup"><span data-stu-id="54ba4-121">String</span></span>|<span data-ttu-id="54ba4-122">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="54ba4-122">The product name.</span></span> <span data-ttu-id="54ba4-123">Наследуется от [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="54ba4-123">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="54ba4-124">отказано</span><span class="sxs-lookup"><span data-stu-id="54ba4-124">denied</span></span>|<span data-ttu-id="54ba4-125">Логический</span><span class="sxs-lookup"><span data-stu-id="54ba4-125">Boolean</span></span>|<span data-ttu-id="54ba4-126">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="54ba4-126">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="54ba4-127">Наследуется от [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="54ba4-127">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="54ba4-128">Связи</span><span class="sxs-lookup"><span data-stu-id="54ba4-128">Relationships</span></span>
<span data-ttu-id="54ba4-129">Нет</span><span class="sxs-lookup"><span data-stu-id="54ba4-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="54ba4-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54ba4-130">JSON Representation</span></span>
<span data-ttu-id="54ba4-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54ba4-131">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```








