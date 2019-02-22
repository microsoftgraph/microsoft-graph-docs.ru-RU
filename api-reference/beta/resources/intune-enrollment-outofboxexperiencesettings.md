---
title: Тип ресурса Outofboxexperiencesettings.
description: Настройка "нет на месте"
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1148ba609a6533dcc6cedb9abd50e9191dceb5d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145530"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="60d54-103">Тип ресурса Outofboxexperiencesettings.</span><span class="sxs-lookup"><span data-stu-id="60d54-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="60d54-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60d54-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60d54-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60d54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60d54-106">Настройка "нет на месте"</span><span class="sxs-lookup"><span data-stu-id="60d54-106">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="60d54-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="60d54-107">Properties</span></span>
|<span data-ttu-id="60d54-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="60d54-108">Property</span></span>|<span data-ttu-id="60d54-109">Тип</span><span class="sxs-lookup"><span data-stu-id="60d54-109">Type</span></span>|<span data-ttu-id="60d54-110">Описание</span><span class="sxs-lookup"><span data-stu-id="60d54-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60d54-111">Хидепривацисеттингс</span><span class="sxs-lookup"><span data-stu-id="60d54-111">hidePrivacySettings</span></span>|<span data-ttu-id="60d54-112">Логический</span><span class="sxs-lookup"><span data-stu-id="60d54-112">Boolean</span></span>|<span data-ttu-id="60d54-113">Отображение или скрытие параметров конфиденциальности для пользователя</span><span class="sxs-lookup"><span data-stu-id="60d54-113">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="60d54-114">Хидиула</span><span class="sxs-lookup"><span data-stu-id="60d54-114">hideEULA</span></span>|<span data-ttu-id="60d54-115">Логический</span><span class="sxs-lookup"><span data-stu-id="60d54-115">Boolean</span></span>|<span data-ttu-id="60d54-116">Отображение или скрытие ЛИЦЕНЗИОНного соглашения для пользователя</span><span class="sxs-lookup"><span data-stu-id="60d54-116">Show or hide EULA to user</span></span>|
|<span data-ttu-id="60d54-117">userType</span><span class="sxs-lookup"><span data-stu-id="60d54-117">userType</span></span>|[<span data-ttu-id="60d54-118">Виндовсусертипе</span><span class="sxs-lookup"><span data-stu-id="60d54-118">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="60d54-119">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="60d54-119">Type of user.</span></span> <span data-ttu-id="60d54-120">Возможные значения: `administrator`, `standard`.</span><span class="sxs-lookup"><span data-stu-id="60d54-120">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="60d54-121">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="60d54-121">deviceUsageType</span></span>|<span data-ttu-id="60d54-122">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).</span><span class="sxs-lookup"><span data-stu-id="60d54-122">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)</span></span>|<span data-ttu-id="60d54-123">Тип проверки подлинности присоединения AAD.</span><span class="sxs-lookup"><span data-stu-id="60d54-123">AAD join authentication type.</span></span> <span data-ttu-id="60d54-124">Возможные значения: `singleUser`, `shared`.</span><span class="sxs-lookup"><span data-stu-id="60d54-124">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="60d54-125">Скипкэйбоардселектионпаже</span><span class="sxs-lookup"><span data-stu-id="60d54-125">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="60d54-126">Логический</span><span class="sxs-lookup"><span data-stu-id="60d54-126">Boolean</span></span>|<span data-ttu-id="60d54-127">Если задано, пропускать страницу "Выбор клавиатуры", если задан язык и регион</span><span class="sxs-lookup"><span data-stu-id="60d54-127">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="60d54-128">Хидискапелинк</span><span class="sxs-lookup"><span data-stu-id="60d54-128">hideEscapeLink</span></span>|<span data-ttu-id="60d54-129">Логический</span><span class="sxs-lookup"><span data-stu-id="60d54-129">Boolean</span></span>|<span data-ttu-id="60d54-130">Если задано значение true, пользователь не сможет начать с другой учетной записи, при входе в компанию</span><span class="sxs-lookup"><span data-stu-id="60d54-130">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="60d54-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="60d54-131">Relationships</span></span>
<span data-ttu-id="60d54-132">Нет</span><span class="sxs-lookup"><span data-stu-id="60d54-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60d54-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60d54-133">JSON Representation</span></span>
<span data-ttu-id="60d54-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60d54-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "hidePrivacySettings": true,
  "hideEULA": true,
  "userType": "String",
  "deviceUsageType": "String",
  "skipKeyboardSelectionPage": true,
  "hideEscapeLink": true
}
```




