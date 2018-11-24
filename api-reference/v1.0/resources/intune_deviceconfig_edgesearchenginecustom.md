# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="d3775-101">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="d3775-101">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="d3775-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d3775-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3775-103">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="d3775-103">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="d3775-104">Наследуется от [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="d3775-104">Inherits from [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d3775-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3775-105">Properties</span></span>
|<span data-ttu-id="d3775-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3775-106">Property</span></span>|<span data-ttu-id="d3775-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d3775-107">Type</span></span>|<span data-ttu-id="d3775-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d3775-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3775-109">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="d3775-109">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="d3775-110">String</span><span class="sxs-lookup"><span data-stu-id="d3775-110">String</span></span>|<span data-ttu-id="d3775-111">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="d3775-111">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3775-112">Связи</span><span class="sxs-lookup"><span data-stu-id="d3775-112">Relationships</span></span>
<span data-ttu-id="d3775-113">Нет</span><span class="sxs-lookup"><span data-stu-id="d3775-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d3775-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3775-114">JSON Representation</span></span>
<span data-ttu-id="d3775-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3775-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```



