# <a name="mimecontent-resource-type"></a><span data-ttu-id="e8ff4-101">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="e8ff4-101">mimeContent resource type</span></span>

> <span data-ttu-id="e8ff4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e8ff4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8ff4-103">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="e8ff4-103">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="e8ff4-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8ff4-104">Properties</span></span>
|<span data-ttu-id="e8ff4-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8ff4-105">Property</span></span>|<span data-ttu-id="e8ff4-106">Тип</span><span class="sxs-lookup"><span data-stu-id="e8ff4-106">Type</span></span>|<span data-ttu-id="e8ff4-107">Описание</span><span class="sxs-lookup"><span data-stu-id="e8ff4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8ff4-108">type</span><span class="sxs-lookup"><span data-stu-id="e8ff4-108">type</span></span>|<span data-ttu-id="e8ff4-109">String</span><span class="sxs-lookup"><span data-stu-id="e8ff4-109">String</span></span>|<span data-ttu-id="e8ff4-110">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="e8ff4-110">Indicates the content mime type.</span></span>|
|<span data-ttu-id="e8ff4-111">value</span><span class="sxs-lookup"><span data-stu-id="e8ff4-111">value</span></span>|<span data-ttu-id="e8ff4-112">Двоичный</span><span class="sxs-lookup"><span data-stu-id="e8ff4-112">Binary</span></span>|<span data-ttu-id="e8ff4-113">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="e8ff4-113">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8ff4-114">Связи</span><span class="sxs-lookup"><span data-stu-id="e8ff4-114">Relationships</span></span>
<span data-ttu-id="e8ff4-115">Нет</span><span class="sxs-lookup"><span data-stu-id="e8ff4-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e8ff4-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8ff4-116">JSON Representation</span></span>
<span data-ttu-id="e8ff4-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8ff4-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



