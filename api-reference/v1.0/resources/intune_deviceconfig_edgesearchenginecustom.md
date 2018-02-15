# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="4a1ad-101">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="4a1ad-101">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="4a1ad-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4a1ad-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a1ad-103">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="4a1ad-103">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="4a1ad-104">Наследуется от [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="4a1ad-104">Inherits from [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4a1ad-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a1ad-105">Properties</span></span>
|<span data-ttu-id="4a1ad-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a1ad-106">Property</span></span>|<span data-ttu-id="4a1ad-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4a1ad-107">Type</span></span>|<span data-ttu-id="4a1ad-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4a1ad-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a1ad-109">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="4a1ad-109">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="4a1ad-110">String</span><span class="sxs-lookup"><span data-stu-id="4a1ad-110">String</span></span>|<span data-ttu-id="4a1ad-111">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="4a1ad-111">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a1ad-112">Связи</span><span class="sxs-lookup"><span data-stu-id="4a1ad-112">Relationships</span></span>
<span data-ttu-id="4a1ad-113">Нет</span><span class="sxs-lookup"><span data-stu-id="4a1ad-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4a1ad-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a1ad-114">JSON Representation</span></span>
<span data-ttu-id="4a1ad-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a1ad-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```



