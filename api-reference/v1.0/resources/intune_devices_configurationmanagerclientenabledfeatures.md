# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="afaab-101">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="afaab-101">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="afaab-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="afaab-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afaab-103">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="afaab-103">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="afaab-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="afaab-104">Properties</span></span>
|<span data-ttu-id="afaab-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="afaab-105">Property</span></span>|<span data-ttu-id="afaab-106">Тип</span><span class="sxs-lookup"><span data-stu-id="afaab-106">Type</span></span>|<span data-ttu-id="afaab-107">Описание</span><span class="sxs-lookup"><span data-stu-id="afaab-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afaab-108">inventory</span><span class="sxs-lookup"><span data-stu-id="afaab-108">inventory</span></span>|<span data-ttu-id="afaab-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="afaab-109">Boolean</span></span>|<span data-ttu-id="afaab-110">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="afaab-110">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="afaab-111">modernApps</span><span class="sxs-lookup"><span data-stu-id="afaab-111">modernApps</span></span>|<span data-ttu-id="afaab-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="afaab-112">Boolean</span></span>|<span data-ttu-id="afaab-113">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="afaab-113">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="afaab-114">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="afaab-114">resourceAccess</span></span>|<span data-ttu-id="afaab-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="afaab-115">Boolean</span></span>|<span data-ttu-id="afaab-116">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="afaab-116">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="afaab-117">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="afaab-117">deviceConfiguration</span></span>|<span data-ttu-id="afaab-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="afaab-118">Boolean</span></span>|<span data-ttu-id="afaab-119">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="afaab-119">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="afaab-120">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="afaab-120">compliancePolicy</span></span>|<span data-ttu-id="afaab-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="afaab-121">Boolean</span></span>|<span data-ttu-id="afaab-122">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="afaab-122">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="afaab-123">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="afaab-123">windowsUpdateForBusiness</span></span>|<span data-ttu-id="afaab-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="afaab-124">Boolean</span></span>|<span data-ttu-id="afaab-125">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="afaab-125">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="afaab-126">Связи</span><span class="sxs-lookup"><span data-stu-id="afaab-126">Relationships</span></span>
<span data-ttu-id="afaab-127">Нет</span><span class="sxs-lookup"><span data-stu-id="afaab-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="afaab-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="afaab-128">JSON Representation</span></span>
<span data-ttu-id="afaab-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="afaab-129">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```



