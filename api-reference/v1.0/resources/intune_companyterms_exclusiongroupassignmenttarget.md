# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="db52a-101">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="db52a-101">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="db52a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="db52a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db52a-103">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="db52a-103">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="db52a-104">Наследуется от [groupAssignmentTarget](../resources/intune_companyterms_groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="db52a-104">Inherits from [groupAssignmentTarget](../resources/intune_companyterms_groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="db52a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="db52a-105">Properties</span></span>
|<span data-ttu-id="db52a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="db52a-106">Property</span></span>|<span data-ttu-id="db52a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="db52a-107">Type</span></span>|<span data-ttu-id="db52a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="db52a-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db52a-109">groupId</span><span class="sxs-lookup"><span data-stu-id="db52a-109">groupId</span></span>|<span data-ttu-id="db52a-110">String</span><span class="sxs-lookup"><span data-stu-id="db52a-110">String</span></span>|<span data-ttu-id="db52a-111">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="db52a-111">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="db52a-112">Наследуется от [groupAssignmentTarget](../resources/intune_companyterms_groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="db52a-112">Inherited from [groupAssignmentTarget](../resources/intune_companyterms_groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="db52a-113">Связи</span><span class="sxs-lookup"><span data-stu-id="db52a-113">Relationships</span></span>
<span data-ttu-id="db52a-114">Нет</span><span class="sxs-lookup"><span data-stu-id="db52a-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="db52a-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db52a-115">JSON Representation</span></span>
<span data-ttu-id="db52a-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db52a-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



