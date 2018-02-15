# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="63393-101">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="63393-101">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="63393-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="63393-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63393-103">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="63393-103">The identifier for an Android app.</span></span>

<span data-ttu-id="63393-104">Наследуется от [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="63393-104">Inherits from [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="63393-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="63393-105">Properties</span></span>
|<span data-ttu-id="63393-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="63393-106">Property</span></span>|<span data-ttu-id="63393-107">Тип</span><span class="sxs-lookup"><span data-stu-id="63393-107">Type</span></span>|<span data-ttu-id="63393-108">Описание</span><span class="sxs-lookup"><span data-stu-id="63393-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63393-109">packageId</span><span class="sxs-lookup"><span data-stu-id="63393-109">packageId</span></span>|<span data-ttu-id="63393-110">String</span><span class="sxs-lookup"><span data-stu-id="63393-110">String</span></span>|<span data-ttu-id="63393-111">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="63393-111">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63393-112">Связи</span><span class="sxs-lookup"><span data-stu-id="63393-112">Relationships</span></span>
<span data-ttu-id="63393-113">Нет</span><span class="sxs-lookup"><span data-stu-id="63393-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="63393-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63393-114">JSON Representation</span></span>
<span data-ttu-id="63393-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63393-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```



