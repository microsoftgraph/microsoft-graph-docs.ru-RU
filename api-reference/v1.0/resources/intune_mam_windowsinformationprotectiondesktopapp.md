# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="0c18b-101">Тип ресурса windowsInformationProtectionDesktopApp</span><span class="sxs-lookup"><span data-stu-id="0c18b-101">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="0c18b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0c18b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c18b-103">Защита данных классических приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="0c18b-103">Desktop App for Windows information protection</span></span>

<span data-ttu-id="0c18b-104">Наследуется от [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c18b-104">Inherits from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0c18b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c18b-105">Properties</span></span>
|<span data-ttu-id="0c18b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c18b-106">Property</span></span>|<span data-ttu-id="0c18b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0c18b-107">Type</span></span>|<span data-ttu-id="0c18b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0c18b-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c18b-109">displayName</span><span class="sxs-lookup"><span data-stu-id="0c18b-109">displayName</span></span>|<span data-ttu-id="0c18b-110">String</span><span class="sxs-lookup"><span data-stu-id="0c18b-110">String</span></span>|<span data-ttu-id="0c18b-111">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="0c18b-111">App display name.</span></span> <span data-ttu-id="0c18b-112">Наследуется от [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c18b-112">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="0c18b-113">description</span><span class="sxs-lookup"><span data-stu-id="0c18b-113">description</span></span>|<span data-ttu-id="0c18b-114">String</span><span class="sxs-lookup"><span data-stu-id="0c18b-114">String</span></span>|<span data-ttu-id="0c18b-115">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="0c18b-115">The app's description.</span></span> <span data-ttu-id="0c18b-116">Наследуется от [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c18b-116">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="0c18b-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="0c18b-117">publisherName</span></span>|<span data-ttu-id="0c18b-118">String</span><span class="sxs-lookup"><span data-stu-id="0c18b-118">String</span></span>|<span data-ttu-id="0c18b-119">Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c18b-119">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="0c18b-120">productName</span><span class="sxs-lookup"><span data-stu-id="0c18b-120">productName</span></span>|<span data-ttu-id="0c18b-121">String</span><span class="sxs-lookup"><span data-stu-id="0c18b-121">String</span></span>|<span data-ttu-id="0c18b-122">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="0c18b-122">The product name.</span></span> <span data-ttu-id="0c18b-123">Наследуется от [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c18b-123">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="0c18b-124">denied</span><span class="sxs-lookup"><span data-stu-id="0c18b-124">denied</span></span>|<span data-ttu-id="0c18b-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c18b-125">Boolean</span></span>|<span data-ttu-id="0c18b-126">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="0c18b-126">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="0c18b-127">Наследуется от [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="0c18b-127">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="0c18b-128">binaryName</span><span class="sxs-lookup"><span data-stu-id="0c18b-128">binaryName</span></span>|<span data-ttu-id="0c18b-129">String</span><span class="sxs-lookup"><span data-stu-id="0c18b-129">String</span></span>|<span data-ttu-id="0c18b-130">Двоичное имя.</span><span class="sxs-lookup"><span data-stu-id="0c18b-130">The binary name.</span></span>|
|<span data-ttu-id="0c18b-131">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="0c18b-131">binaryVersionLow</span></span>|<span data-ttu-id="0c18b-132">String</span><span class="sxs-lookup"><span data-stu-id="0c18b-132">String</span></span>|<span data-ttu-id="0c18b-133">Нижняя двоичная версия.</span><span class="sxs-lookup"><span data-stu-id="0c18b-133">The lower binary version.</span></span>|
|<span data-ttu-id="0c18b-134">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="0c18b-134">binaryVersionHigh</span></span>|<span data-ttu-id="0c18b-135">String</span><span class="sxs-lookup"><span data-stu-id="0c18b-135">String</span></span>|<span data-ttu-id="0c18b-136">Верхняя двоичная версия.</span><span class="sxs-lookup"><span data-stu-id="0c18b-136">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c18b-137">Связи</span><span class="sxs-lookup"><span data-stu-id="0c18b-137">Relationships</span></span>
<span data-ttu-id="0c18b-138">Нет</span><span class="sxs-lookup"><span data-stu-id="0c18b-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c18b-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c18b-139">JSON Representation</span></span>
<span data-ttu-id="0c18b-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c18b-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```



