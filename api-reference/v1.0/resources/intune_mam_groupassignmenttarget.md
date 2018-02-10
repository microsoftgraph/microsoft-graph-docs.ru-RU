# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="fa030-101">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fa030-101">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="fa030-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fa030-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa030-103">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="fa030-103">Represents an assignment to a group.</span></span>

<span data-ttu-id="fa030-104">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune_mam_deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="fa030-104">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune_mam_deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa030-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa030-105">Properties</span></span>
|<span data-ttu-id="fa030-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa030-106">Property</span></span>|<span data-ttu-id="fa030-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fa030-107">Type</span></span>|<span data-ttu-id="fa030-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fa030-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa030-109">groupId</span><span class="sxs-lookup"><span data-stu-id="fa030-109">groupId</span></span>|<span data-ttu-id="fa030-110">Строка</span><span class="sxs-lookup"><span data-stu-id="fa030-110">String</span></span>|<span data-ttu-id="fa030-111">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="fa030-111">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa030-112">Связи</span><span class="sxs-lookup"><span data-stu-id="fa030-112">Relationships</span></span>
<span data-ttu-id="fa030-113">Нет</span><span class="sxs-lookup"><span data-stu-id="fa030-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fa030-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa030-114">JSON Representation</span></span>
<span data-ttu-id="fa030-115">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa030-115">Here is a JSON representation of the resource.</span></span>
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



