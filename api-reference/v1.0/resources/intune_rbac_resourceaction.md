# <a name="resourceaction-resource-type"></a><span data-ttu-id="524ed-101">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="524ed-101">resourceAction resource type</span></span>

> <span data-ttu-id="524ed-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="524ed-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="524ed-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="524ed-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="524ed-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="524ed-104">Properties</span></span>
|<span data-ttu-id="524ed-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="524ed-105">Property</span></span>|<span data-ttu-id="524ed-106">Тип</span><span class="sxs-lookup"><span data-stu-id="524ed-106">Type</span></span>|<span data-ttu-id="524ed-107">Описание</span><span class="sxs-lookup"><span data-stu-id="524ed-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="524ed-108">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="524ed-108">allowedResourceActions</span></span>|<span data-ttu-id="524ed-109">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="524ed-109">String collection</span></span>|<span data-ttu-id="524ed-110">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="524ed-110">Allowed Actions</span></span>|
|<span data-ttu-id="524ed-111">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="524ed-111">notAllowedResourceActions</span></span>|<span data-ttu-id="524ed-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="524ed-112">String collection</span></span>|<span data-ttu-id="524ed-113">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="524ed-113">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="524ed-114">Связи</span><span class="sxs-lookup"><span data-stu-id="524ed-114">Relationships</span></span>
<span data-ttu-id="524ed-115">Нет</span><span class="sxs-lookup"><span data-stu-id="524ed-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="524ed-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="524ed-116">JSON Representation</span></span>
<span data-ttu-id="524ed-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="524ed-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```








