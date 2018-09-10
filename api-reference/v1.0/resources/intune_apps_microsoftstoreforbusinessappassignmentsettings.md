# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="51958-101">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="51958-101">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="51958-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51958-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51958-103">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="51958-103">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="51958-104">Наследуется от [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="51958-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="51958-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="51958-105">Properties</span></span>
|<span data-ttu-id="51958-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="51958-106">Property</span></span>|<span data-ttu-id="51958-107">Тип</span><span class="sxs-lookup"><span data-stu-id="51958-107">Type</span></span>|<span data-ttu-id="51958-108">Описание</span><span class="sxs-lookup"><span data-stu-id="51958-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51958-109">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="51958-109">useDeviceContext</span></span>|<span data-ttu-id="51958-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="51958-110">Boolean</span></span>|<span data-ttu-id="51958-111">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="51958-111">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51958-112">Связи</span><span class="sxs-lookup"><span data-stu-id="51958-112">Relationships</span></span>
<span data-ttu-id="51958-113">Нет</span><span class="sxs-lookup"><span data-stu-id="51958-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51958-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51958-114">JSON Representation</span></span>
<span data-ttu-id="51958-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51958-115">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```








