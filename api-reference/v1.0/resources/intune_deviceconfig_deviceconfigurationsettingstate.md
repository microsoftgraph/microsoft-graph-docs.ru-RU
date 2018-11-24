# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="fb9b7-101">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="fb9b7-101">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="fb9b7-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fb9b7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb9b7-103">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="fb9b7-103">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="fb9b7-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb9b7-104">Properties</span></span>
|<span data-ttu-id="fb9b7-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb9b7-105">Property</span></span>|<span data-ttu-id="fb9b7-106">Тип</span><span class="sxs-lookup"><span data-stu-id="fb9b7-106">Type</span></span>|<span data-ttu-id="fb9b7-107">Описание</span><span class="sxs-lookup"><span data-stu-id="fb9b7-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb9b7-108">setting</span><span class="sxs-lookup"><span data-stu-id="fb9b7-108">setting</span></span>|<span data-ttu-id="fb9b7-109">String</span><span class="sxs-lookup"><span data-stu-id="fb9b7-109">String</span></span>|<span data-ttu-id="fb9b7-110">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="fb9b7-110">The setting that is being reported</span></span>|
|<span data-ttu-id="fb9b7-111">settingName</span><span class="sxs-lookup"><span data-stu-id="fb9b7-111">settingName</span></span>|<span data-ttu-id="fb9b7-112">String</span><span class="sxs-lookup"><span data-stu-id="fb9b7-112">String</span></span>|<span data-ttu-id="fb9b7-113">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="fb9b7-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="fb9b7-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="fb9b7-114">instanceDisplayName</span></span>|<span data-ttu-id="fb9b7-115">String</span><span class="sxs-lookup"><span data-stu-id="fb9b7-115">String</span></span>|<span data-ttu-id="fb9b7-116">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="fb9b7-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="fb9b7-117">state</span><span class="sxs-lookup"><span data-stu-id="fb9b7-117">state</span></span>|[<span data-ttu-id="fb9b7-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="fb9b7-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="fb9b7-119">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="fb9b7-119">The compliance state of the setting.</span></span> <span data-ttu-id="fb9b7-120">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="fb9b7-120">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="fb9b7-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="fb9b7-121">errorCode</span></span>|<span data-ttu-id="fb9b7-122">Int64</span><span class="sxs-lookup"><span data-stu-id="fb9b7-122">Int64</span></span>|<span data-ttu-id="fb9b7-123">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="fb9b7-123">Error code for the setting</span></span>|
|<span data-ttu-id="fb9b7-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="fb9b7-124">errorDescription</span></span>|<span data-ttu-id="fb9b7-125">String</span><span class="sxs-lookup"><span data-stu-id="fb9b7-125">String</span></span>|<span data-ttu-id="fb9b7-126">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="fb9b7-126">Error description</span></span>|
|<span data-ttu-id="fb9b7-127">userId</span><span class="sxs-lookup"><span data-stu-id="fb9b7-127">userId</span></span>|<span data-ttu-id="fb9b7-128">String</span><span class="sxs-lookup"><span data-stu-id="fb9b7-128">String</span></span>|<span data-ttu-id="fb9b7-129">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="fb9b7-129">UserId</span></span>|
|<span data-ttu-id="fb9b7-130">userName</span><span class="sxs-lookup"><span data-stu-id="fb9b7-130">userName</span></span>|<span data-ttu-id="fb9b7-131">String</span><span class="sxs-lookup"><span data-stu-id="fb9b7-131">String</span></span>|<span data-ttu-id="fb9b7-132">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="fb9b7-132">UserName</span></span>|
|<span data-ttu-id="fb9b7-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="fb9b7-133">userEmail</span></span>|<span data-ttu-id="fb9b7-134">String</span><span class="sxs-lookup"><span data-stu-id="fb9b7-134">String</span></span>|<span data-ttu-id="fb9b7-135">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="fb9b7-135">UserEmail</span></span>|
|<span data-ttu-id="fb9b7-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fb9b7-136">userPrincipalName</span></span>|<span data-ttu-id="fb9b7-137">String</span><span class="sxs-lookup"><span data-stu-id="fb9b7-137">String</span></span>|<span data-ttu-id="fb9b7-138">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="fb9b7-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="fb9b7-139">sources</span><span class="sxs-lookup"><span data-stu-id="fb9b7-139">sources</span></span>|<span data-ttu-id="fb9b7-140">Коллекция [settingSource](../resources/intune_deviceconfig_settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="fb9b7-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="fb9b7-141">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="fb9b7-141">Contributing policies</span></span>|
|<span data-ttu-id="fb9b7-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="fb9b7-142">currentValue</span></span>|<span data-ttu-id="fb9b7-143">String</span><span class="sxs-lookup"><span data-stu-id="fb9b7-143">String</span></span>|<span data-ttu-id="fb9b7-144">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="fb9b7-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb9b7-145">Связи</span><span class="sxs-lookup"><span data-stu-id="fb9b7-145">Relationships</span></span>
<span data-ttu-id="fb9b7-146">None</span><span class="sxs-lookup"><span data-stu-id="fb9b7-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fb9b7-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb9b7-147">JSON Representation</span></span>
<span data-ttu-id="fb9b7-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb9b7-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```



