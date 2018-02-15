# <a name="auditactor-resource-type"></a><span data-ttu-id="21aef-101">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="21aef-101">auditActor resource type</span></span>

> <span data-ttu-id="21aef-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="21aef-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21aef-103">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="21aef-103">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="21aef-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="21aef-104">Properties</span></span>
|<span data-ttu-id="21aef-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="21aef-105">Property</span></span>|<span data-ttu-id="21aef-106">Тип</span><span class="sxs-lookup"><span data-stu-id="21aef-106">Type</span></span>|<span data-ttu-id="21aef-107">Описание</span><span class="sxs-lookup"><span data-stu-id="21aef-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21aef-108">type</span><span class="sxs-lookup"><span data-stu-id="21aef-108">type</span></span>|<span data-ttu-id="21aef-109">String</span><span class="sxs-lookup"><span data-stu-id="21aef-109">String</span></span>|<span data-ttu-id="21aef-110">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="21aef-110">Actor Type.</span></span>|
|<span data-ttu-id="21aef-111">permissions</span><span class="sxs-lookup"><span data-stu-id="21aef-111">permissions</span></span>|<span data-ttu-id="21aef-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="21aef-112">String collection</span></span>|<span data-ttu-id="21aef-113">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="21aef-113">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="21aef-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="21aef-114">userPermissions</span></span>|<span data-ttu-id="21aef-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="21aef-115">String collection</span></span>|<span data-ttu-id="21aef-116">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="21aef-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="21aef-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="21aef-117">applicationId</span></span>|<span data-ttu-id="21aef-118">String</span><span class="sxs-lookup"><span data-stu-id="21aef-118">String</span></span>|<span data-ttu-id="21aef-119">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="21aef-119">AAD Application Id.</span></span>|
|<span data-ttu-id="21aef-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="21aef-120">applicationDisplayName</span></span>|<span data-ttu-id="21aef-121">String</span><span class="sxs-lookup"><span data-stu-id="21aef-121">String</span></span>|<span data-ttu-id="21aef-122">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="21aef-122">Name of the Application.</span></span>|
|<span data-ttu-id="21aef-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="21aef-123">userPrincipalName</span></span>|<span data-ttu-id="21aef-124">String</span><span class="sxs-lookup"><span data-stu-id="21aef-124">String</span></span>|<span data-ttu-id="21aef-125">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="21aef-125">User principal name (UPN)</span></span>|
|<span data-ttu-id="21aef-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="21aef-126">servicePrincipalName</span></span>|<span data-ttu-id="21aef-127">String</span><span class="sxs-lookup"><span data-stu-id="21aef-127">String</span></span>|<span data-ttu-id="21aef-128">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="21aef-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="21aef-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="21aef-129">ipAddress</span></span>|<span data-ttu-id="21aef-130">String</span><span class="sxs-lookup"><span data-stu-id="21aef-130">String</span></span>|<span data-ttu-id="21aef-131">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="21aef-131">IPAddress.</span></span>|
|<span data-ttu-id="21aef-132">userId</span><span class="sxs-lookup"><span data-stu-id="21aef-132">userID</span></span>|<span data-ttu-id="21aef-133">String</span><span class="sxs-lookup"><span data-stu-id="21aef-133">String</span></span>|<span data-ttu-id="21aef-134">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="21aef-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21aef-135">Связи</span><span class="sxs-lookup"><span data-stu-id="21aef-135">Relationships</span></span>
<span data-ttu-id="21aef-136">Нет</span><span class="sxs-lookup"><span data-stu-id="21aef-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21aef-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21aef-137">JSON Representation</span></span>
<span data-ttu-id="21aef-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21aef-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "permissions": [
    "String"
  ],
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```



