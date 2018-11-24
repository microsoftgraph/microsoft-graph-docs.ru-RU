# <a name="auditactor-resource-type"></a><span data-ttu-id="d6095-101">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="d6095-101">auditActor resource type</span></span>

> <span data-ttu-id="d6095-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d6095-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6095-103">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="d6095-103">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="d6095-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6095-104">Properties</span></span>
|<span data-ttu-id="d6095-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6095-105">Property</span></span>|<span data-ttu-id="d6095-106">Тип</span><span class="sxs-lookup"><span data-stu-id="d6095-106">Type</span></span>|<span data-ttu-id="d6095-107">Описание</span><span class="sxs-lookup"><span data-stu-id="d6095-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6095-108">type</span><span class="sxs-lookup"><span data-stu-id="d6095-108">type</span></span>|<span data-ttu-id="d6095-109">String</span><span class="sxs-lookup"><span data-stu-id="d6095-109">String</span></span>|<span data-ttu-id="d6095-110">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="d6095-110">Actor Type.</span></span>|
|<span data-ttu-id="d6095-111">userPermissions</span><span class="sxs-lookup"><span data-stu-id="d6095-111">userPermissions</span></span>|<span data-ttu-id="d6095-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6095-112">String collection</span></span>|<span data-ttu-id="d6095-113">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="d6095-113">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="d6095-114">applicationId</span><span class="sxs-lookup"><span data-stu-id="d6095-114">applicationId</span></span>|<span data-ttu-id="d6095-115">String</span><span class="sxs-lookup"><span data-stu-id="d6095-115">String</span></span>|<span data-ttu-id="d6095-116">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="d6095-116">AAD Application Id.</span></span>|
|<span data-ttu-id="d6095-117">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="d6095-117">applicationDisplayName</span></span>|<span data-ttu-id="d6095-118">String</span><span class="sxs-lookup"><span data-stu-id="d6095-118">String</span></span>|<span data-ttu-id="d6095-119">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="d6095-119">Name of the Application.</span></span>|
|<span data-ttu-id="d6095-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d6095-120">userPrincipalName</span></span>|<span data-ttu-id="d6095-121">String</span><span class="sxs-lookup"><span data-stu-id="d6095-121">String</span></span>|<span data-ttu-id="d6095-122">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="d6095-122">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="d6095-123">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="d6095-123">servicePrincipalName</span></span>|<span data-ttu-id="d6095-124">String</span><span class="sxs-lookup"><span data-stu-id="d6095-124">String</span></span>|<span data-ttu-id="d6095-125">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="d6095-125">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="d6095-126">ipAddress</span><span class="sxs-lookup"><span data-stu-id="d6095-126">ipAddress</span></span>|<span data-ttu-id="d6095-127">String</span><span class="sxs-lookup"><span data-stu-id="d6095-127">String</span></span>|<span data-ttu-id="d6095-128">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="d6095-128">IPAddress.</span></span>|
|<span data-ttu-id="d6095-129">userId</span><span class="sxs-lookup"><span data-stu-id="d6095-129">userId</span></span>|<span data-ttu-id="d6095-130">String</span><span class="sxs-lookup"><span data-stu-id="d6095-130">String</span></span>|<span data-ttu-id="d6095-131">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6095-131">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6095-132">Связи</span><span class="sxs-lookup"><span data-stu-id="d6095-132">Relationships</span></span>
<span data-ttu-id="d6095-133">None</span><span class="sxs-lookup"><span data-stu-id="d6095-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6095-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6095-134">JSON Representation</span></span>
<span data-ttu-id="d6095-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6095-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
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



