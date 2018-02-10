# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="ee126-101">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ee126-101">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="ee126-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ee126-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee126-103">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="ee126-103">Represents an assignment to a group.</span></span>

<span data-ttu-id="ee126-104">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune_companyterms_deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="ee126-104">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune_companyterms_deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ee126-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee126-105">Properties</span></span>
|<span data-ttu-id="ee126-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee126-106">Property</span></span>|<span data-ttu-id="ee126-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ee126-107">Type</span></span>|<span data-ttu-id="ee126-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ee126-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee126-109">groupId</span><span class="sxs-lookup"><span data-stu-id="ee126-109">groupId</span></span>|<span data-ttu-id="ee126-110">Строка</span><span class="sxs-lookup"><span data-stu-id="ee126-110">String</span></span>|<span data-ttu-id="ee126-111">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="ee126-111">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee126-112">Связи</span><span class="sxs-lookup"><span data-stu-id="ee126-112">Relationships</span></span>
<span data-ttu-id="ee126-113">Нет</span><span class="sxs-lookup"><span data-stu-id="ee126-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ee126-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee126-114">JSON Representation</span></span>
<span data-ttu-id="ee126-115">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee126-115">Here is a JSON representation of the resource.</span></span>
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



