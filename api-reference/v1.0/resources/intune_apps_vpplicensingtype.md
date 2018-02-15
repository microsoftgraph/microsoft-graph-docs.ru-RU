# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="95f77-101">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="95f77-101">vppLicensingType resource type</span></span>

> <span data-ttu-id="95f77-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="95f77-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95f77-103">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="95f77-103">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="95f77-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="95f77-104">Properties</span></span>
|<span data-ttu-id="95f77-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="95f77-105">Property</span></span>|<span data-ttu-id="95f77-106">Тип</span><span class="sxs-lookup"><span data-stu-id="95f77-106">Type</span></span>|<span data-ttu-id="95f77-107">Описание</span><span class="sxs-lookup"><span data-stu-id="95f77-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95f77-108">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="95f77-108">supportsUserLicensing</span></span>|<span data-ttu-id="95f77-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="95f77-109">Boolean</span></span>|<span data-ttu-id="95f77-110">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="95f77-110">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="95f77-111">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="95f77-111">supportsDeviceLicensing</span></span>|<span data-ttu-id="95f77-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="95f77-112">Boolean</span></span>|<span data-ttu-id="95f77-113">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="95f77-113">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95f77-114">Связи</span><span class="sxs-lookup"><span data-stu-id="95f77-114">Relationships</span></span>
<span data-ttu-id="95f77-115">Нет</span><span class="sxs-lookup"><span data-stu-id="95f77-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="95f77-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95f77-116">JSON Representation</span></span>
<span data-ttu-id="95f77-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95f77-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



