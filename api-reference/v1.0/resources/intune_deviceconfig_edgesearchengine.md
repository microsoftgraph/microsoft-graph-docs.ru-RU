# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="850ad-101">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="850ad-101">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="850ad-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="850ad-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="850ad-103">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для MDM-управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="850ad-103">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="850ad-104">Наследуется от [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="850ad-104">Inherits from [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="850ad-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="850ad-105">Properties</span></span>
|<span data-ttu-id="850ad-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="850ad-106">Property</span></span>|<span data-ttu-id="850ad-107">Тип</span><span class="sxs-lookup"><span data-stu-id="850ad-107">Type</span></span>|<span data-ttu-id="850ad-108">Описание</span><span class="sxs-lookup"><span data-stu-id="850ad-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="850ad-109">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="850ad-109">edgeSearchEngineType</span></span>|[<span data-ttu-id="850ad-110">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="850ad-110">edgeSearchEngineType</span></span>](../resources/intune_deviceconfig_edgesearchenginetype.md)|<span data-ttu-id="850ad-p101">Позволяет ИТ-администраторам задать механизм поиска по умолчанию для устройств под управлением MDM. Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="850ad-p101">Allows IT admins to set a predefined default search engine for MDM-Controlled devices. The possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="850ad-113">Связи</span><span class="sxs-lookup"><span data-stu-id="850ad-113">Relationships</span></span>
<span data-ttu-id="850ad-114">Нет</span><span class="sxs-lookup"><span data-stu-id="850ad-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="850ad-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="850ad-115">JSON Representation</span></span>
<span data-ttu-id="850ad-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="850ad-116">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```








