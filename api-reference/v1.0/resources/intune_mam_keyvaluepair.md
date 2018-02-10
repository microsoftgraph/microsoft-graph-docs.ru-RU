# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="7b372-101">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="7b372-101">keyValuePair resource type</span></span>

> <span data-ttu-id="7b372-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7b372-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b372-103">Пара "ключ-значение" для хранения пользовательских настроек</span><span class="sxs-lookup"><span data-stu-id="7b372-103">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="7b372-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b372-104">Properties</span></span>
|<span data-ttu-id="7b372-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b372-105">Property</span></span>|<span data-ttu-id="7b372-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7b372-106">Type</span></span>|<span data-ttu-id="7b372-107">Описание</span><span class="sxs-lookup"><span data-stu-id="7b372-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b372-108">name</span><span class="sxs-lookup"><span data-stu-id="7b372-108">name</span></span>|<span data-ttu-id="7b372-109">Строка</span><span class="sxs-lookup"><span data-stu-id="7b372-109">String</span></span>|<span data-ttu-id="7b372-110">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="7b372-110">Name for this key-value pair</span></span>|
|<span data-ttu-id="7b372-111">value</span><span class="sxs-lookup"><span data-stu-id="7b372-111">value</span></span>|<span data-ttu-id="7b372-112">Строка</span><span class="sxs-lookup"><span data-stu-id="7b372-112">String</span></span>|<span data-ttu-id="7b372-113">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="7b372-113">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b372-114">Связи</span><span class="sxs-lookup"><span data-stu-id="7b372-114">Relationships</span></span>
<span data-ttu-id="7b372-115">Нет</span><span class="sxs-lookup"><span data-stu-id="7b372-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7b372-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b372-116">JSON Representation</span></span>
<span data-ttu-id="7b372-117">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b372-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



