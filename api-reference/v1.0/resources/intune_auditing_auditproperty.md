# <a name="auditproperty-resource-type"></a><span data-ttu-id="02a0e-101">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="02a0e-101">auditProperty resource type</span></span>

> <span data-ttu-id="02a0e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="02a0e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02a0e-103">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="02a0e-103">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="02a0e-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="02a0e-104">Properties</span></span>
|<span data-ttu-id="02a0e-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="02a0e-105">Property</span></span>|<span data-ttu-id="02a0e-106">Тип</span><span class="sxs-lookup"><span data-stu-id="02a0e-106">Type</span></span>|<span data-ttu-id="02a0e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="02a0e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02a0e-108">displayName</span><span class="sxs-lookup"><span data-stu-id="02a0e-108">displayName</span></span>|<span data-ttu-id="02a0e-109">String</span><span class="sxs-lookup"><span data-stu-id="02a0e-109">String</span></span>|<span data-ttu-id="02a0e-110">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="02a0e-110">Display Name</span></span>|
|<span data-ttu-id="02a0e-111">oldValue</span><span class="sxs-lookup"><span data-stu-id="02a0e-111">oldValue</span></span>|<span data-ttu-id="02a0e-112">String</span><span class="sxs-lookup"><span data-stu-id="02a0e-112">String</span></span>|<span data-ttu-id="02a0e-113">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="02a0e-113">Old value.</span></span>|
|<span data-ttu-id="02a0e-114">newValue</span><span class="sxs-lookup"><span data-stu-id="02a0e-114">newValue</span></span>|<span data-ttu-id="02a0e-115">String</span><span class="sxs-lookup"><span data-stu-id="02a0e-115">String</span></span>|<span data-ttu-id="02a0e-116">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="02a0e-116">New value of  in </span></span>|

## <a name="relationships"></a><span data-ttu-id="02a0e-117">Связи</span><span class="sxs-lookup"><span data-stu-id="02a0e-117">Relationships</span></span>
<span data-ttu-id="02a0e-118">Нет</span><span class="sxs-lookup"><span data-stu-id="02a0e-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="02a0e-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02a0e-119">JSON Representation</span></span>
<span data-ttu-id="02a0e-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02a0e-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



