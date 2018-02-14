# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="40c6b-101">Тип ресурса deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="40c6b-101">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="40c6b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="40c6b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40c6b-103">Состояние параметров политики соответствия требованиям для определенного устройства.</span><span class="sxs-lookup"><span data-stu-id="40c6b-103">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="40c6b-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="40c6b-104">Properties</span></span>
|<span data-ttu-id="40c6b-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="40c6b-105">Property</span></span>|<span data-ttu-id="40c6b-106">Тип</span><span class="sxs-lookup"><span data-stu-id="40c6b-106">Type</span></span>|<span data-ttu-id="40c6b-107">Описание</span><span class="sxs-lookup"><span data-stu-id="40c6b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40c6b-108">setting</span><span class="sxs-lookup"><span data-stu-id="40c6b-108">setting</span></span>|<span data-ttu-id="40c6b-109">String</span><span class="sxs-lookup"><span data-stu-id="40c6b-109">String</span></span>|<span data-ttu-id="40c6b-110">Параметр для отчета</span><span class="sxs-lookup"><span data-stu-id="40c6b-110">The setting that is being reported</span></span>|
|<span data-ttu-id="40c6b-111">settingName</span><span class="sxs-lookup"><span data-stu-id="40c6b-111">settingName</span></span>|<span data-ttu-id="40c6b-112">String</span><span class="sxs-lookup"><span data-stu-id="40c6b-112">String</span></span>|<span data-ttu-id="40c6b-113">Локализованное или понятное имя параметра для отчета</span><span class="sxs-lookup"><span data-stu-id="40c6b-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="40c6b-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="40c6b-114">instanceDisplayName</span></span>|<span data-ttu-id="40c6b-115">String</span><span class="sxs-lookup"><span data-stu-id="40c6b-115">String</span></span>|<span data-ttu-id="40c6b-116">Имя экземпляра параметра для отчета.</span><span class="sxs-lookup"><span data-stu-id="40c6b-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="40c6b-117">state</span><span class="sxs-lookup"><span data-stu-id="40c6b-117">state</span></span>|<span data-ttu-id="40c6b-118">String</span><span class="sxs-lookup"><span data-stu-id="40c6b-118">String</span></span>|<span data-ttu-id="40c6b-119">Состояние соответствия требованиям для параметра. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="40c6b-119">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="40c6b-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="40c6b-120">errorCode</span></span>|<span data-ttu-id="40c6b-121">Int64</span><span class="sxs-lookup"><span data-stu-id="40c6b-121">Int64</span></span>|<span data-ttu-id="40c6b-122">Код ошибки для параметра</span><span class="sxs-lookup"><span data-stu-id="40c6b-122">Error code for the setting</span></span>|
|<span data-ttu-id="40c6b-123">errorDescription</span><span class="sxs-lookup"><span data-stu-id="40c6b-123">error_description</span></span>|<span data-ttu-id="40c6b-124">String</span><span class="sxs-lookup"><span data-stu-id="40c6b-124">String</span></span>|<span data-ttu-id="40c6b-125">Описание ошибки</span><span class="sxs-lookup"><span data-stu-id="40c6b-125">Error description</span></span>|
|<span data-ttu-id="40c6b-126">userId</span><span class="sxs-lookup"><span data-stu-id="40c6b-126">userID</span></span>|<span data-ttu-id="40c6b-127">String</span><span class="sxs-lookup"><span data-stu-id="40c6b-127">String</span></span>|<span data-ttu-id="40c6b-128">ИД пользователя</span><span class="sxs-lookup"><span data-stu-id="40c6b-128">UserId</span></span>|
|<span data-ttu-id="40c6b-129">userName</span><span class="sxs-lookup"><span data-stu-id="40c6b-129">userName</span></span>|<span data-ttu-id="40c6b-130">String</span><span class="sxs-lookup"><span data-stu-id="40c6b-130">String</span></span>|<span data-ttu-id="40c6b-131">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="40c6b-131">userName</span></span>|
|<span data-ttu-id="40c6b-132">userEmail</span><span class="sxs-lookup"><span data-stu-id="40c6b-132">userEmail</span></span>|<span data-ttu-id="40c6b-133">String</span><span class="sxs-lookup"><span data-stu-id="40c6b-133">String</span></span>|<span data-ttu-id="40c6b-134">Электронный адрес пользователя</span><span class="sxs-lookup"><span data-stu-id="40c6b-134">UserEmail Element</span></span>|
|<span data-ttu-id="40c6b-135">userPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="40c6b-135">userPrincipalName</span></span>|<span data-ttu-id="40c6b-136">String</span><span class="sxs-lookup"><span data-stu-id="40c6b-136">String</span></span>|<span data-ttu-id="40c6b-137">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="40c6b-137">userPrincipalName</span></span>|
|<span data-ttu-id="40c6b-138">sources</span><span class="sxs-lookup"><span data-stu-id="40c6b-138">Content sources</span></span>|<span data-ttu-id="40c6b-139">Коллекция [settingSource](../resources/intune_deviceconfig_settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="40c6b-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="40c6b-140">Соответствующие политики</span><span class="sxs-lookup"><span data-stu-id="40c6b-140">Contributing policies</span></span>|
|<span data-ttu-id="40c6b-141">currentValue</span><span class="sxs-lookup"><span data-stu-id="40c6b-141">currentValue</span></span>|<span data-ttu-id="40c6b-142">String</span><span class="sxs-lookup"><span data-stu-id="40c6b-142">String</span></span>|<span data-ttu-id="40c6b-143">Текущее значение параметра на устройстве</span><span class="sxs-lookup"><span data-stu-id="40c6b-143">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="40c6b-144">Связи</span><span class="sxs-lookup"><span data-stu-id="40c6b-144">Relationships</span></span>
<span data-ttu-id="40c6b-145">Нет</span><span class="sxs-lookup"><span data-stu-id="40c6b-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="40c6b-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40c6b-146">JSON Representation</span></span>
<span data-ttu-id="40c6b-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40c6b-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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



