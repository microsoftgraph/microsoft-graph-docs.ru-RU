---
title: Тип ресурса outOfBoxExperienceSettings
description: В соответствующем взаимодействия параметр
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d2b48fef00c9c3a291a0a2fdfe680b9f4e21030
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404605"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="d71ef-103">Тип ресурса outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="d71ef-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="d71ef-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d71ef-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d71ef-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d71ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d71ef-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d71ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d71ef-107">В соответствующем взаимодействия параметр</span><span class="sxs-lookup"><span data-stu-id="d71ef-107">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="d71ef-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d71ef-108">Properties</span></span>
|<span data-ttu-id="d71ef-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d71ef-109">Property</span></span>|<span data-ttu-id="d71ef-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d71ef-110">Type</span></span>|<span data-ttu-id="d71ef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d71ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d71ef-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="d71ef-112">hidePrivacySettings</span></span>|<span data-ttu-id="d71ef-113">Логический</span><span class="sxs-lookup"><span data-stu-id="d71ef-113">Boolean</span></span>|<span data-ttu-id="d71ef-114">Показать или скрыть параметры конфиденциальности для пользователя</span><span class="sxs-lookup"><span data-stu-id="d71ef-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="d71ef-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="d71ef-115">hideEULA</span></span>|<span data-ttu-id="d71ef-116">Логический</span><span class="sxs-lookup"><span data-stu-id="d71ef-116">Boolean</span></span>|<span data-ttu-id="d71ef-117">Показать или скрыть лицензионное соглашение для пользователя</span><span class="sxs-lookup"><span data-stu-id="d71ef-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="d71ef-118">userType</span><span class="sxs-lookup"><span data-stu-id="d71ef-118">userType</span></span>|[<span data-ttu-id="d71ef-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="d71ef-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="d71ef-120">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="d71ef-120">Type of user.</span></span> <span data-ttu-id="d71ef-121">Возможные значения: `administrator`, `standard`.</span><span class="sxs-lookup"><span data-stu-id="d71ef-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="d71ef-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="d71ef-122">deviceUsageType</span></span>|<span data-ttu-id="d71ef-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).</span><span class="sxs-lookup"><span data-stu-id="d71ef-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)</span></span>|<span data-ttu-id="d71ef-124">Тип проверки подлинности соединения AAD.</span><span class="sxs-lookup"><span data-stu-id="d71ef-124">AAD join authentication type.</span></span> <span data-ttu-id="d71ef-125">Возможные значения: `singleUser`, `shared`.</span><span class="sxs-lookup"><span data-stu-id="d71ef-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="d71ef-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="d71ef-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="d71ef-127">Логический</span><span class="sxs-lookup"><span data-stu-id="d71ef-127">Boolean</span></span>|<span data-ttu-id="d71ef-128">Если набор, а затем пропустить раскладка клавиатуры страницы Если значение языка и региона</span><span class="sxs-lookup"><span data-stu-id="d71ef-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="d71ef-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="d71ef-129">hideEscapeLink</span></span>|<span data-ttu-id="d71ef-130">Логический</span><span class="sxs-lookup"><span data-stu-id="d71ef-130">Boolean</span></span>|<span data-ttu-id="d71ef-131">Если параметр имеет значение true, затем пользователь не может запуститься через с другой учетной записи для входа в компании</span><span class="sxs-lookup"><span data-stu-id="d71ef-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="d71ef-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="d71ef-132">Relationships</span></span>
<span data-ttu-id="d71ef-133">Нет</span><span class="sxs-lookup"><span data-stu-id="d71ef-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d71ef-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d71ef-134">JSON Representation</span></span>
<span data-ttu-id="d71ef-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d71ef-135">Here is a JSON representation of the resource.</span></span>
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




