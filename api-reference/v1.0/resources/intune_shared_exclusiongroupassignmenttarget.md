# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="e349e-101">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e349e-101">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="e349e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e349e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e349e-103">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="e349e-103">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="e349e-104">Наследуется от [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e349e-104">Inherits from [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e349e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e349e-105">Properties</span></span>
|<span data-ttu-id="e349e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e349e-106">Property</span></span>|<span data-ttu-id="e349e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e349e-107">Type</span></span>|<span data-ttu-id="e349e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e349e-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e349e-109">groupId</span><span class="sxs-lookup"><span data-stu-id="e349e-109">groupId</span></span>|<span data-ttu-id="e349e-110">Строка</span><span class="sxs-lookup"><span data-stu-id="e349e-110">String</span></span>|<span data-ttu-id="e349e-111">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="e349e-111">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="e349e-112">Наследуется от [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e349e-112">Inherited from [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e349e-113">Связи</span><span class="sxs-lookup"><span data-stu-id="e349e-113">Relationships</span></span>
<span data-ttu-id="e349e-114">Нет</span><span class="sxs-lookup"><span data-stu-id="e349e-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e349e-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e349e-115">JSON Representation</span></span>
<span data-ttu-id="e349e-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e349e-116">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```








