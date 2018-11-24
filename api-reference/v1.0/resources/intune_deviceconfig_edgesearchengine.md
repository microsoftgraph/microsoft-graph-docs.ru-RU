# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="2dfc4-101">Тип ресурса edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="2dfc4-101">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="2dfc4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2dfc4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2dfc4-103">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="2dfc4-103">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="2dfc4-104">Наследуется от [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="2dfc4-104">Inherits from [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2dfc4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2dfc4-105">Properties</span></span>
|<span data-ttu-id="2dfc4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2dfc4-106">Property</span></span>|<span data-ttu-id="2dfc4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2dfc4-107">Type</span></span>|<span data-ttu-id="2dfc4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2dfc4-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dfc4-109">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="2dfc4-109">edgeSearchEngineType</span></span>|[<span data-ttu-id="2dfc4-110">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="2dfc4-110">edgeSearchEngineType</span></span>](../resources/intune_deviceconfig_edgesearchenginetype.md)|<span data-ttu-id="2dfc4-111">Позволяет ИТ-администраторам предварительно задавать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="2dfc4-111">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="2dfc4-112">Возможные значения: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="2dfc4-112">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dfc4-113">Связи</span><span class="sxs-lookup"><span data-stu-id="2dfc4-113">Relationships</span></span>
<span data-ttu-id="2dfc4-114">Нет</span><span class="sxs-lookup"><span data-stu-id="2dfc4-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2dfc4-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2dfc4-115">JSON Representation</span></span>
<span data-ttu-id="2dfc4-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2dfc4-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```



