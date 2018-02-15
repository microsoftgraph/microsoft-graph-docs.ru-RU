# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="0433d-101">Тип ресурса deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="0433d-101">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="0433d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0433d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0433d-103">Состояние параметра конфигурации определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="0433d-103">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="0433d-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="0433d-104">Properties</span></span>
|<span data-ttu-id="0433d-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="0433d-105">Property</span></span>|<span data-ttu-id="0433d-106">Тип</span><span class="sxs-lookup"><span data-stu-id="0433d-106">Type</span></span>|<span data-ttu-id="0433d-107">Описание</span><span class="sxs-lookup"><span data-stu-id="0433d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0433d-108">setting</span><span class="sxs-lookup"><span data-stu-id="0433d-108">setting</span></span>|<span data-ttu-id="0433d-109">String</span><span class="sxs-lookup"><span data-stu-id="0433d-109">String</span></span>|<span data-ttu-id="0433d-110">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="0433d-110">The setting that is being reported</span></span>|
|<span data-ttu-id="0433d-111">settingName</span><span class="sxs-lookup"><span data-stu-id="0433d-111">settingName</span></span>|<span data-ttu-id="0433d-112">String</span><span class="sxs-lookup"><span data-stu-id="0433d-112">String</span></span>|<span data-ttu-id="0433d-113">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="0433d-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="0433d-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0433d-114">instanceDisplayName</span></span>|<span data-ttu-id="0433d-115">String</span><span class="sxs-lookup"><span data-stu-id="0433d-115">String</span></span>|<span data-ttu-id="0433d-116">Имя экземпляра параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="0433d-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="0433d-117">state</span><span class="sxs-lookup"><span data-stu-id="0433d-117">state</span></span>|<span data-ttu-id="0433d-118">String</span><span class="sxs-lookup"><span data-stu-id="0433d-118">String</span></span>|<span data-ttu-id="0433d-119">Состояние соответствия требованиям для параметра. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="0433d-119">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="0433d-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="0433d-120">errorCode</span></span>|<span data-ttu-id="0433d-121">Int64</span><span class="sxs-lookup"><span data-stu-id="0433d-121">Int64</span></span>|<span data-ttu-id="0433d-122">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="0433d-122">Error code for the setting</span></span>|
|<span data-ttu-id="0433d-123">errorDescription</span><span class="sxs-lookup"><span data-stu-id="0433d-123">error_description</span></span>|<span data-ttu-id="0433d-124">String</span><span class="sxs-lookup"><span data-stu-id="0433d-124">String</span></span>|<span data-ttu-id="0433d-125">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="0433d-125">Error description</span></span>|
|<span data-ttu-id="0433d-126">userId</span><span class="sxs-lookup"><span data-stu-id="0433d-126">userID</span></span>|<span data-ttu-id="0433d-127">String</span><span class="sxs-lookup"><span data-stu-id="0433d-127">String</span></span>|<span data-ttu-id="0433d-128">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="0433d-128">UserId</span></span>|
|<span data-ttu-id="0433d-129">userName</span><span class="sxs-lookup"><span data-stu-id="0433d-129">userName</span></span>|<span data-ttu-id="0433d-130">String</span><span class="sxs-lookup"><span data-stu-id="0433d-130">String</span></span>|<span data-ttu-id="0433d-131">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="0433d-131">userName</span></span>|
|<span data-ttu-id="0433d-132">userEmail</span><span class="sxs-lookup"><span data-stu-id="0433d-132">userEmail</span></span>|<span data-ttu-id="0433d-133">String</span><span class="sxs-lookup"><span data-stu-id="0433d-133">String</span></span>|<span data-ttu-id="0433d-134">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="0433d-134">UserEmail Element</span></span>|
|<span data-ttu-id="0433d-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0433d-135">userPrincipalName</span></span>|<span data-ttu-id="0433d-136">String</span><span class="sxs-lookup"><span data-stu-id="0433d-136">String</span></span>|<span data-ttu-id="0433d-137">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="0433d-137">userPrincipalName</span></span>|
|<span data-ttu-id="0433d-138">sources</span><span class="sxs-lookup"><span data-stu-id="0433d-138">Content sources</span></span>|<span data-ttu-id="0433d-139">Коллекция [settingSource](../resources/intune_deviceconfig_settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="0433d-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="0433d-140">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="0433d-140">Contributing policies</span></span>|
|<span data-ttu-id="0433d-141">currentValue</span><span class="sxs-lookup"><span data-stu-id="0433d-141">currentValue</span></span>|<span data-ttu-id="0433d-142">String</span><span class="sxs-lookup"><span data-stu-id="0433d-142">String</span></span>|<span data-ttu-id="0433d-143">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="0433d-143">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="0433d-144">Связи</span><span class="sxs-lookup"><span data-stu-id="0433d-144">Relationships</span></span>
<span data-ttu-id="0433d-145">Нет</span><span class="sxs-lookup"><span data-stu-id="0433d-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0433d-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0433d-146">JSON Representation</span></span>
<span data-ttu-id="0433d-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0433d-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



