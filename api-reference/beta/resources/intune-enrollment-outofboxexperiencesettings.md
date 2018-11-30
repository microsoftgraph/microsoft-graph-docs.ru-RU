---
title: Тип ресурса outOfBoxExperienceSettings
description: В соответствующем взаимодействия параметр
ms.openlocfilehash: 7d685c7e229828309e2ee759396215c3cd8dfac9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082200"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="64155-103">Тип ресурса outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="64155-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="64155-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64155-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64155-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64155-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64155-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="64155-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64155-107">В соответствующем взаимодействия параметр</span><span class="sxs-lookup"><span data-stu-id="64155-107">Out of box experience setting</span></span>
## <a name="properties"></a><span data-ttu-id="64155-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="64155-108">Properties</span></span>
|<span data-ttu-id="64155-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="64155-109">Property</span></span>|<span data-ttu-id="64155-110">Тип</span><span class="sxs-lookup"><span data-stu-id="64155-110">Type</span></span>|<span data-ttu-id="64155-111">Description</span><span class="sxs-lookup"><span data-stu-id="64155-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64155-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="64155-112">hidePrivacySettings</span></span>|<span data-ttu-id="64155-113">Логический</span><span class="sxs-lookup"><span data-stu-id="64155-113">Boolean</span></span>|<span data-ttu-id="64155-114">Показать или скрыть параметры конфиденциальности для пользователя</span><span class="sxs-lookup"><span data-stu-id="64155-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="64155-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="64155-115">hideEULA</span></span>|<span data-ttu-id="64155-116">Логический</span><span class="sxs-lookup"><span data-stu-id="64155-116">Boolean</span></span>|<span data-ttu-id="64155-117">Показать или скрыть лицензионное соглашение для пользователя</span><span class="sxs-lookup"><span data-stu-id="64155-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="64155-118">userType</span><span class="sxs-lookup"><span data-stu-id="64155-118">userType</span></span>|[<span data-ttu-id="64155-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="64155-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="64155-120">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="64155-120">Type of user.</span></span> <span data-ttu-id="64155-121">Возможные значения: `administrator`, `standard`.</span><span class="sxs-lookup"><span data-stu-id="64155-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="64155-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="64155-122">deviceUsageType</span></span>|<span data-ttu-id="64155-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).</span><span class="sxs-lookup"><span data-stu-id="64155-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)</span></span>|<span data-ttu-id="64155-124">Тип проверки подлинности соединения AAD.</span><span class="sxs-lookup"><span data-stu-id="64155-124">AAD join authentication type.</span></span> <span data-ttu-id="64155-125">Возможные значения: `singleUser`, `shared`.</span><span class="sxs-lookup"><span data-stu-id="64155-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="64155-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="64155-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="64155-127">Логический</span><span class="sxs-lookup"><span data-stu-id="64155-127">Boolean</span></span>|<span data-ttu-id="64155-128">Если набор, а затем пропустить раскладка клавиатуры страницы Если значение языка и региона</span><span class="sxs-lookup"><span data-stu-id="64155-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="64155-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="64155-129">hideEscapeLink</span></span>|<span data-ttu-id="64155-130">Логический</span><span class="sxs-lookup"><span data-stu-id="64155-130">Boolean</span></span>|<span data-ttu-id="64155-131">Если параметр имеет значение true, затем пользователь не может запуститься через с другой учетной записи для входа в компании</span><span class="sxs-lookup"><span data-stu-id="64155-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="64155-132">Связи</span><span class="sxs-lookup"><span data-stu-id="64155-132">Relationships</span></span>
<span data-ttu-id="64155-133">Нет</span><span class="sxs-lookup"><span data-stu-id="64155-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="64155-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64155-134">JSON Representation</span></span>
<span data-ttu-id="64155-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64155-135">Here is a JSON representation of the resource.</span></span>
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





