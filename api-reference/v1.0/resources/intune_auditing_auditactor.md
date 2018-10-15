# <a name="auditactor-resource-type"></a><span data-ttu-id="96c40-101">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="96c40-101">auditActor resource type</span></span>

> <span data-ttu-id="96c40-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="96c40-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96c40-103">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="96c40-103">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="96c40-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="96c40-104">Properties</span></span>
|<span data-ttu-id="96c40-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="96c40-105">Property</span></span>|<span data-ttu-id="96c40-106">Тип</span><span class="sxs-lookup"><span data-stu-id="96c40-106">Type</span></span>|<span data-ttu-id="96c40-107">Описание</span><span class="sxs-lookup"><span data-stu-id="96c40-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96c40-108">тип</span><span class="sxs-lookup"><span data-stu-id="96c40-108">type</span></span>|<span data-ttu-id="96c40-109">Строка</span><span class="sxs-lookup"><span data-stu-id="96c40-109">String</span></span>|<span data-ttu-id="96c40-110">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="96c40-110">Actor Type.</span></span>|
|<span data-ttu-id="96c40-111">userPermissions</span><span class="sxs-lookup"><span data-stu-id="96c40-111">userPermissions</span></span>|<span data-ttu-id="96c40-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="96c40-112">String collection</span></span>|<span data-ttu-id="96c40-113">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="96c40-113">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="96c40-114">applicationId</span><span class="sxs-lookup"><span data-stu-id="96c40-114">applicationId</span></span>|<span data-ttu-id="96c40-115">Строка</span><span class="sxs-lookup"><span data-stu-id="96c40-115">String</span></span>|<span data-ttu-id="96c40-116">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="96c40-116">AAD Application Id.</span></span>|
|<span data-ttu-id="96c40-117">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="96c40-117">applicationDisplayName</span></span>|<span data-ttu-id="96c40-118">Строка</span><span class="sxs-lookup"><span data-stu-id="96c40-118">String</span></span>|<span data-ttu-id="96c40-119">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="96c40-119">Name of the Application.</span></span>|
|<span data-ttu-id="96c40-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="96c40-120">userPrincipalName</span></span>|<span data-ttu-id="96c40-121">Строка</span><span class="sxs-lookup"><span data-stu-id="96c40-121">String</span></span>|<span data-ttu-id="96c40-122">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="96c40-122">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="96c40-123">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="96c40-123">servicePrincipalName</span></span>|<span data-ttu-id="96c40-124">Строка</span><span class="sxs-lookup"><span data-stu-id="96c40-124">String</span></span>|<span data-ttu-id="96c40-125">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="96c40-125">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="96c40-126">ipAddress</span><span class="sxs-lookup"><span data-stu-id="96c40-126">ipAddress</span></span>|<span data-ttu-id="96c40-127">Строка</span><span class="sxs-lookup"><span data-stu-id="96c40-127">String</span></span>|<span data-ttu-id="96c40-128">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="96c40-128">IPAddress.</span></span>|
|<span data-ttu-id="96c40-129">userId</span><span class="sxs-lookup"><span data-stu-id="96c40-129">userId</span></span>|<span data-ttu-id="96c40-130">Строка</span><span class="sxs-lookup"><span data-stu-id="96c40-130">String</span></span>|<span data-ttu-id="96c40-131">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="96c40-131">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96c40-132">Связи</span><span class="sxs-lookup"><span data-stu-id="96c40-132">Relationships</span></span>
<span data-ttu-id="96c40-133">Нет</span><span class="sxs-lookup"><span data-stu-id="96c40-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="96c40-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96c40-134">JSON Representation</span></span>
<span data-ttu-id="96c40-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96c40-135">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}-->
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








