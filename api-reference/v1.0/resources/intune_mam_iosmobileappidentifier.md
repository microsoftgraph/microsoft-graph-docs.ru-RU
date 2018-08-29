# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="58791-101">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="58791-101">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="58791-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="58791-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58791-103">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="58791-103">The identifier for an iOS app.</span></span>

<span data-ttu-id="58791-104">Наследуется от [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="58791-104">Inherits from [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="58791-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="58791-105">Properties</span></span>
|<span data-ttu-id="58791-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="58791-106">Property</span></span>|<span data-ttu-id="58791-107">Тип</span><span class="sxs-lookup"><span data-stu-id="58791-107">Type</span></span>|<span data-ttu-id="58791-108">Описание</span><span class="sxs-lookup"><span data-stu-id="58791-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58791-109">bundleId</span><span class="sxs-lookup"><span data-stu-id="58791-109">bundleId</span></span>|<span data-ttu-id="58791-110">String</span><span class="sxs-lookup"><span data-stu-id="58791-110">String</span></span>|<span data-ttu-id="58791-111">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="58791-111">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58791-112">Связи</span><span class="sxs-lookup"><span data-stu-id="58791-112">Relationships</span></span>
<span data-ttu-id="58791-113">Нет</span><span class="sxs-lookup"><span data-stu-id="58791-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="58791-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58791-114">JSON Representation</span></span>
<span data-ttu-id="58791-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58791-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileAppIdentifier",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```



