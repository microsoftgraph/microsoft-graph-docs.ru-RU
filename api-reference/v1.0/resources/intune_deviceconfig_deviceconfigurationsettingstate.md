# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="51c2c-101">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="51c2c-101">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="51c2c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51c2c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51c2c-103">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="51c2c-103">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="51c2c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="51c2c-104">Properties</span></span>
|<span data-ttu-id="51c2c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="51c2c-105">Property</span></span>|<span data-ttu-id="51c2c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="51c2c-106">Type</span></span>|<span data-ttu-id="51c2c-107">Описание</span><span class="sxs-lookup"><span data-stu-id="51c2c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51c2c-108">Параметр</span><span class="sxs-lookup"><span data-stu-id="51c2c-108">setting</span></span>|<span data-ttu-id="51c2c-109">String (строка)</span><span class="sxs-lookup"><span data-stu-id="51c2c-109">String</span></span>|<span data-ttu-id="51c2c-110">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="51c2c-110">The setting that is being reported</span></span>|
|<span data-ttu-id="51c2c-111">settingName</span><span class="sxs-lookup"><span data-stu-id="51c2c-111">settingName</span></span>|<span data-ttu-id="51c2c-112">String (строка)</span><span class="sxs-lookup"><span data-stu-id="51c2c-112">String</span></span>|<span data-ttu-id="51c2c-113">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="51c2c-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="51c2c-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="51c2c-114">instanceDisplayName</span></span>|<span data-ttu-id="51c2c-115">String (строка)</span><span class="sxs-lookup"><span data-stu-id="51c2c-115">String</span></span>|<span data-ttu-id="51c2c-116">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="51c2c-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="51c2c-117">Состояние</span><span class="sxs-lookup"><span data-stu-id="51c2c-117">state</span></span>|[<span data-ttu-id="51c2c-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="51c2c-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="51c2c-p101">Состояние соответствия настроек требованиям. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="51c2c-p101">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="51c2c-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="51c2c-121">errorCode</span></span>|<span data-ttu-id="51c2c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="51c2c-122">Int64</span></span>|<span data-ttu-id="51c2c-123">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="51c2c-123">Error code for the setting</span></span>|
|<span data-ttu-id="51c2c-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="51c2c-124">errorDescription</span></span>|<span data-ttu-id="51c2c-125">String (строка)</span><span class="sxs-lookup"><span data-stu-id="51c2c-125">String</span></span>|<span data-ttu-id="51c2c-126">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="51c2c-126">Error description</span></span>|
|<span data-ttu-id="51c2c-127">userId</span><span class="sxs-lookup"><span data-stu-id="51c2c-127">userId</span></span>|<span data-ttu-id="51c2c-128">String (строка)</span><span class="sxs-lookup"><span data-stu-id="51c2c-128">String</span></span>|<span data-ttu-id="51c2c-129">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="51c2c-129">UserId</span></span>|
|<span data-ttu-id="51c2c-130">userName</span><span class="sxs-lookup"><span data-stu-id="51c2c-130">userName</span></span>|<span data-ttu-id="51c2c-131">String (строка)</span><span class="sxs-lookup"><span data-stu-id="51c2c-131">String</span></span>|<span data-ttu-id="51c2c-132">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="51c2c-132">UserName</span></span>|
|<span data-ttu-id="51c2c-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="51c2c-133">userEmail</span></span>|<span data-ttu-id="51c2c-134">String (строка)</span><span class="sxs-lookup"><span data-stu-id="51c2c-134">String</span></span>|<span data-ttu-id="51c2c-135">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="51c2c-135">UserEmail</span></span>|
|<span data-ttu-id="51c2c-136">Имя пользователя-участника</span><span class="sxs-lookup"><span data-stu-id="51c2c-136">userPrincipalName</span></span>|<span data-ttu-id="51c2c-137">String (строка)</span><span class="sxs-lookup"><span data-stu-id="51c2c-137">String</span></span>|<span data-ttu-id="51c2c-138">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="51c2c-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="51c2c-139">Источники</span><span class="sxs-lookup"><span data-stu-id="51c2c-139">sources</span></span>|<span data-ttu-id="51c2c-140">Коллекция [settingSource](../resources/intune_deviceconfig_settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="51c2c-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="51c2c-141">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="51c2c-141">Contributing policies</span></span>|
|<span data-ttu-id="51c2c-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="51c2c-142">currentValue</span></span>|<span data-ttu-id="51c2c-143">String (строка)</span><span class="sxs-lookup"><span data-stu-id="51c2c-143">String</span></span>|<span data-ttu-id="51c2c-144">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="51c2c-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="51c2c-145">Связи</span><span class="sxs-lookup"><span data-stu-id="51c2c-145">Relationships</span></span>
<span data-ttu-id="51c2c-146">Нет</span><span class="sxs-lookup"><span data-stu-id="51c2c-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51c2c-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51c2c-147">JSON Representation</span></span>
<span data-ttu-id="51c2c-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51c2c-148">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}-->
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








