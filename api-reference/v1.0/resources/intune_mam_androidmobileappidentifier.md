# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="4b2b4-101">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="4b2b4-101">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="4b2b4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4b2b4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b2b4-103">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="4b2b4-103">The identifier for an Android app.</span></span>

<span data-ttu-id="4b2b4-104">Наследуется от [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="4b2b4-104">Inherits from [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4b2b4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b2b4-105">Properties</span></span>
|<span data-ttu-id="4b2b4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b2b4-106">Property</span></span>|<span data-ttu-id="4b2b4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4b2b4-107">Type</span></span>|<span data-ttu-id="4b2b4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4b2b4-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b2b4-109">packageId</span><span class="sxs-lookup"><span data-stu-id="4b2b4-109">packageId</span></span>|<span data-ttu-id="4b2b4-110">String</span><span class="sxs-lookup"><span data-stu-id="4b2b4-110">String</span></span>|<span data-ttu-id="4b2b4-111">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="4b2b4-111">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b2b4-112">Связи</span><span class="sxs-lookup"><span data-stu-id="4b2b4-112">Relationships</span></span>
<span data-ttu-id="4b2b4-113">Нет</span><span class="sxs-lookup"><span data-stu-id="4b2b4-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b2b4-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b2b4-114">JSON Representation</span></span>
<span data-ttu-id="4b2b4-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b2b4-115">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```








