# <a name="auditresource-resource-type"></a><span data-ttu-id="60bfc-101">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="60bfc-101">auditResource resource type</span></span>

> <span data-ttu-id="60bfc-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="60bfc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60bfc-103">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="60bfc-103">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="60bfc-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="60bfc-104">Properties</span></span>
|<span data-ttu-id="60bfc-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="60bfc-105">Property</span></span>|<span data-ttu-id="60bfc-106">Тип</span><span class="sxs-lookup"><span data-stu-id="60bfc-106">Type</span></span>|<span data-ttu-id="60bfc-107">Описание</span><span class="sxs-lookup"><span data-stu-id="60bfc-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60bfc-108">displayName</span><span class="sxs-lookup"><span data-stu-id="60bfc-108">displayName</span></span>|<span data-ttu-id="60bfc-109">String</span><span class="sxs-lookup"><span data-stu-id="60bfc-109">String</span></span>|<span data-ttu-id="60bfc-110">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="60bfc-110">Display name.</span></span>|
|<span data-ttu-id="60bfc-111">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="60bfc-111">modifiedProperties</span></span>|<span data-ttu-id="60bfc-112">Коллекция [auditProperty](../resources/intune_auditing_auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="60bfc-112">[auditProperty](../resources/intune_auditing_auditproperty.md) collection</span></span>|<span data-ttu-id="60bfc-113">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="60bfc-113">List of modified properties.</span></span>|
|<span data-ttu-id="60bfc-114">type</span><span class="sxs-lookup"><span data-stu-id="60bfc-114">type</span></span>|<span data-ttu-id="60bfc-115">String</span><span class="sxs-lookup"><span data-stu-id="60bfc-115">String</span></span>|<span data-ttu-id="60bfc-116">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="60bfc-116">Audit resource's type.</span></span>|
|<span data-ttu-id="60bfc-117">resourceId</span><span class="sxs-lookup"><span data-stu-id="60bfc-117">resourceId</span></span>|<span data-ttu-id="60bfc-118">String</span><span class="sxs-lookup"><span data-stu-id="60bfc-118">String</span></span>|<span data-ttu-id="60bfc-119">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="60bfc-119">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60bfc-120">Связи</span><span class="sxs-lookup"><span data-stu-id="60bfc-120">Relationships</span></span>
<span data-ttu-id="60bfc-121">Нет</span><span class="sxs-lookup"><span data-stu-id="60bfc-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="60bfc-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60bfc-122">JSON Representation</span></span>
<span data-ttu-id="60bfc-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60bfc-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```



