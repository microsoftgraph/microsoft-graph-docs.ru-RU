# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="c0860-101">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c0860-101">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="c0860-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c0860-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0860-103">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="c0860-103">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="c0860-104">Наследуется от ресурса [groupAssignmentTarget](../resources/intune_onboarding_groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="c0860-104">Inherits from [groupAssignmentTarget](../resources/intune_onboarding_groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c0860-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0860-105">Properties</span></span>
|<span data-ttu-id="c0860-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0860-106">Property</span></span>|<span data-ttu-id="c0860-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c0860-107">Type</span></span>|<span data-ttu-id="c0860-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c0860-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0860-109">groupId</span><span class="sxs-lookup"><span data-stu-id="c0860-109">groupId</span></span>|<span data-ttu-id="c0860-110">Строка</span><span class="sxs-lookup"><span data-stu-id="c0860-110">String</span></span>|<span data-ttu-id="c0860-111">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="c0860-111">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="c0860-112">Наследуется от ресурса [groupAssignmentTarget](../resources/intune_onboarding_groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="c0860-112">Inherited from [groupAssignmentTarget](../resources/intune_onboarding_groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0860-113">Связи</span><span class="sxs-lookup"><span data-stu-id="c0860-113">Relationships</span></span>
<span data-ttu-id="c0860-114">Нет</span><span class="sxs-lookup"><span data-stu-id="c0860-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c0860-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0860-115">JSON Representation</span></span>
<span data-ttu-id="c0860-116">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0860-116">Here is a JSON representation of the resource.</span></span>
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



