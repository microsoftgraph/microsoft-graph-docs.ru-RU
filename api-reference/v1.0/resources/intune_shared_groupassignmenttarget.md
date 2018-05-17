# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="26884-101">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="26884-101">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="26884-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="26884-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26884-103">Представляет назначение группе.</span><span class="sxs-lookup"><span data-stu-id="26884-103">Represents an assignment to a group.</span></span>

<span data-ttu-id="26884-104">Наследуется от типа [deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="26884-104">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="26884-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="26884-105">Properties</span></span>
|<span data-ttu-id="26884-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="26884-106">Property</span></span>|<span data-ttu-id="26884-107">Тип</span><span class="sxs-lookup"><span data-stu-id="26884-107">Type</span></span>|<span data-ttu-id="26884-108">Описание</span><span class="sxs-lookup"><span data-stu-id="26884-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26884-109">groupId</span><span class="sxs-lookup"><span data-stu-id="26884-109">groupId</span></span>|<span data-ttu-id="26884-110">String</span><span class="sxs-lookup"><span data-stu-id="26884-110">String</span></span>|<span data-ttu-id="26884-111">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="26884-111">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26884-112">Связи</span><span class="sxs-lookup"><span data-stu-id="26884-112">Relationships</span></span>
<span data-ttu-id="26884-113">Нет</span><span class="sxs-lookup"><span data-stu-id="26884-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="26884-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26884-114">JSON Representation</span></span>
<span data-ttu-id="26884-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26884-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```



