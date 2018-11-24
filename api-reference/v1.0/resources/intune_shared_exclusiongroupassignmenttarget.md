# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="392af-101">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="392af-101">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="392af-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="392af-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="392af-103">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="392af-103">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="392af-104">Наследуется от [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="392af-104">Inherits from [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="392af-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="392af-105">Properties</span></span>
|<span data-ttu-id="392af-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="392af-106">Property</span></span>|<span data-ttu-id="392af-107">Тип</span><span class="sxs-lookup"><span data-stu-id="392af-107">Type</span></span>|<span data-ttu-id="392af-108">Описание</span><span class="sxs-lookup"><span data-stu-id="392af-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="392af-109">groupId</span><span class="sxs-lookup"><span data-stu-id="392af-109">groupId</span></span>|<span data-ttu-id="392af-110">String</span><span class="sxs-lookup"><span data-stu-id="392af-110">String</span></span>|<span data-ttu-id="392af-111">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="392af-111">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="392af-112">Наследуется от [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="392af-112">Inherited from [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="392af-113">Связи</span><span class="sxs-lookup"><span data-stu-id="392af-113">Relationships</span></span>
<span data-ttu-id="392af-114">None</span><span class="sxs-lookup"><span data-stu-id="392af-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="392af-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="392af-115">JSON Representation</span></span>
<span data-ttu-id="392af-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="392af-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



