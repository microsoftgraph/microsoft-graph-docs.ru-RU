# <a name="resourceaction-resource-type"></a><span data-ttu-id="2f4c9-101">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="2f4c9-101">resourceAction resource type</span></span>

> <span data-ttu-id="2f4c9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f4c9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f4c9-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2f4c9-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2f4c9-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f4c9-104">Properties</span></span>
|<span data-ttu-id="2f4c9-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f4c9-105">Property</span></span>|<span data-ttu-id="2f4c9-106">Тип</span><span class="sxs-lookup"><span data-stu-id="2f4c9-106">Type</span></span>|<span data-ttu-id="2f4c9-107">Описание</span><span class="sxs-lookup"><span data-stu-id="2f4c9-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f4c9-108">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="2f4c9-108">allowedResourceActions</span></span>|<span data-ttu-id="2f4c9-109">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2f4c9-109">String collection</span></span>|<span data-ttu-id="2f4c9-110">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="2f4c9-110">Allowed Actions</span></span>|
|<span data-ttu-id="2f4c9-111">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="2f4c9-111">notAllowedResourceActions</span></span>|<span data-ttu-id="2f4c9-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2f4c9-112">String collection</span></span>|<span data-ttu-id="2f4c9-113">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="2f4c9-113">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f4c9-114">Связи</span><span class="sxs-lookup"><span data-stu-id="2f4c9-114">Relationships</span></span>
<span data-ttu-id="2f4c9-115">Нет</span><span class="sxs-lookup"><span data-stu-id="2f4c9-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2f4c9-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f4c9-116">JSON Representation</span></span>
<span data-ttu-id="2f4c9-117">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f4c9-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
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



