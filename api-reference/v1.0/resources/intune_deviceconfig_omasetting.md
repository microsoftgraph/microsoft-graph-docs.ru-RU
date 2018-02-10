# <a name="omasetting-resource-type"></a><span data-ttu-id="9957a-101">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="9957a-101">omaSetting resource type</span></span>

> <span data-ttu-id="9957a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9957a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9957a-103">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="9957a-103">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="9957a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="9957a-104">Properties</span></span>
|<span data-ttu-id="9957a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="9957a-105">Property</span></span>|<span data-ttu-id="9957a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="9957a-106">Type</span></span>|<span data-ttu-id="9957a-107">Описание</span><span class="sxs-lookup"><span data-stu-id="9957a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9957a-108">displayName</span><span class="sxs-lookup"><span data-stu-id="9957a-108">displayName</span></span>|<span data-ttu-id="9957a-109">Строка</span><span class="sxs-lookup"><span data-stu-id="9957a-109">String</span></span>|<span data-ttu-id="9957a-110">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="9957a-110">Display Name</span></span>|
|<span data-ttu-id="9957a-111">description</span><span class="sxs-lookup"><span data-stu-id="9957a-111">description</span></span>|<span data-ttu-id="9957a-112">Строка</span><span class="sxs-lookup"><span data-stu-id="9957a-112">String</span></span>|<span data-ttu-id="9957a-113">Описание.</span><span class="sxs-lookup"><span data-stu-id="9957a-113">Description</span></span>|
|<span data-ttu-id="9957a-114">omaUri</span><span class="sxs-lookup"><span data-stu-id="9957a-114">omaUri</span></span>|<span data-ttu-id="9957a-115">Строка</span><span class="sxs-lookup"><span data-stu-id="9957a-115">String</span></span>|<span data-ttu-id="9957a-116">OMA.</span><span class="sxs-lookup"><span data-stu-id="9957a-116">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9957a-117">Связи</span><span class="sxs-lookup"><span data-stu-id="9957a-117">Relationships</span></span>
<span data-ttu-id="9957a-118">Нет</span><span class="sxs-lookup"><span data-stu-id="9957a-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9957a-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9957a-119">JSON Representation</span></span>
<span data-ttu-id="9957a-120">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9957a-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



