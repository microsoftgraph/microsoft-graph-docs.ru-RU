# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="d9ed2-101">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d9ed2-101">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="d9ed2-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d9ed2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9ed2-103">Представляет назначение группе.</span><span class="sxs-lookup"><span data-stu-id="d9ed2-103">Represents an assignment to a group.</span></span>

<span data-ttu-id="d9ed2-104">Наследуется от типа [deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d9ed2-104">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d9ed2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9ed2-105">Properties</span></span>
|<span data-ttu-id="d9ed2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9ed2-106">Property</span></span>|<span data-ttu-id="d9ed2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d9ed2-107">Type</span></span>|<span data-ttu-id="d9ed2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d9ed2-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9ed2-109">groupId</span><span class="sxs-lookup"><span data-stu-id="d9ed2-109">groupId</span></span>|<span data-ttu-id="d9ed2-110">String</span><span class="sxs-lookup"><span data-stu-id="d9ed2-110">String</span></span>|<span data-ttu-id="d9ed2-111">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="d9ed2-111">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9ed2-112">Связи</span><span class="sxs-lookup"><span data-stu-id="d9ed2-112">Relationships</span></span>
<span data-ttu-id="d9ed2-113">None</span><span class="sxs-lookup"><span data-stu-id="d9ed2-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d9ed2-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9ed2-114">JSON Representation</span></span>
<span data-ttu-id="d9ed2-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9ed2-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```



