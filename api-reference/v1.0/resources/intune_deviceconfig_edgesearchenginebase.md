# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="73cb3-101">Тип ресурса edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="73cb3-101">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="73cb3-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="73cb3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73cb3-103">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="73cb3-103">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="73cb3-104">Пользователи могут переопределять эту настройку и изменять поисковую систему по умолчанию, если не установлена политика AllowSearchEngineCustomization.</span><span class="sxs-lookup"><span data-stu-id="73cb3-104">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="73cb3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="73cb3-105">Properties</span></span>
|<span data-ttu-id="73cb3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="73cb3-106">Property</span></span>|<span data-ttu-id="73cb3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="73cb3-107">Type</span></span>|<span data-ttu-id="73cb3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="73cb3-108">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="73cb3-109">Связи</span><span class="sxs-lookup"><span data-stu-id="73cb3-109">Relationships</span></span>
<span data-ttu-id="73cb3-110">Нет</span><span class="sxs-lookup"><span data-stu-id="73cb3-110">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="73cb3-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73cb3-111">JSON Representation</span></span>
<span data-ttu-id="73cb3-112">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73cb3-112">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineBase"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineBase"
}
```








