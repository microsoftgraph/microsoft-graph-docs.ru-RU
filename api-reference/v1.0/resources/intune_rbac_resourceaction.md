# <a name="resourceaction-resource-type"></a><span data-ttu-id="33195-101">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="33195-101">resourceAction resource type</span></span>

> <span data-ttu-id="33195-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="33195-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33195-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="33195-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="33195-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="33195-104">Properties</span></span>
|<span data-ttu-id="33195-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="33195-105">Property</span></span>|<span data-ttu-id="33195-106">Тип</span><span class="sxs-lookup"><span data-stu-id="33195-106">Type</span></span>|<span data-ttu-id="33195-107">Описание</span><span class="sxs-lookup"><span data-stu-id="33195-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33195-108">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="33195-108">allowedResourceActions</span></span>|<span data-ttu-id="33195-109">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="33195-109">String collection</span></span>|<span data-ttu-id="33195-110">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="33195-110">Allowed Actions</span></span>|
|<span data-ttu-id="33195-111">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="33195-111">notAllowedResourceActions</span></span>|<span data-ttu-id="33195-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="33195-112">String collection</span></span>|<span data-ttu-id="33195-113">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="33195-113">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="33195-114">Связи</span><span class="sxs-lookup"><span data-stu-id="33195-114">Relationships</span></span>
<span data-ttu-id="33195-115">Нет</span><span class="sxs-lookup"><span data-stu-id="33195-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="33195-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33195-116">JSON Representation</span></span>
<span data-ttu-id="33195-117">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33195-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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



