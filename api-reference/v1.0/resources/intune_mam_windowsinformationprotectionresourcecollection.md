# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="f063b-101">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="f063b-101">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="f063b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f063b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f063b-103">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="f063b-103">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="f063b-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="f063b-104">Properties</span></span>
|<span data-ttu-id="f063b-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="f063b-105">Property</span></span>|<span data-ttu-id="f063b-106">Тип</span><span class="sxs-lookup"><span data-stu-id="f063b-106">Type</span></span>|<span data-ttu-id="f063b-107">Описание</span><span class="sxs-lookup"><span data-stu-id="f063b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f063b-108">displayName</span><span class="sxs-lookup"><span data-stu-id="f063b-108">displayName</span></span>|<span data-ttu-id="f063b-109">Строка</span><span class="sxs-lookup"><span data-stu-id="f063b-109">String</span></span>|<span data-ttu-id="f063b-110">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="f063b-110">Display name</span></span>|
|<span data-ttu-id="f063b-111">resources</span><span class="sxs-lookup"><span data-stu-id="f063b-111">resources</span></span>|<span data-ttu-id="f063b-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f063b-112">String collection</span></span>|<span data-ttu-id="f063b-113">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="f063b-113">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="f063b-114">Связи</span><span class="sxs-lookup"><span data-stu-id="f063b-114">Relationships</span></span>
<span data-ttu-id="f063b-115">Нет</span><span class="sxs-lookup"><span data-stu-id="f063b-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f063b-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f063b-116">JSON Representation</span></span>
<span data-ttu-id="f063b-117">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f063b-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```



