---
title: Тип ресурса outOfBoxExperienceSettings
description: В соответствующем взаимодействия параметр
author: tfitzmac
ms.openlocfilehash: 545fbe5c27063397a4d08c40729227804ebfc56d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308409"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="67211-103">Тип ресурса outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="67211-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="67211-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="67211-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67211-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67211-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67211-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="67211-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67211-107">В соответствующем взаимодействия параметр</span><span class="sxs-lookup"><span data-stu-id="67211-107">Out of box experience setting</span></span>
## <a name="properties"></a><span data-ttu-id="67211-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="67211-108">Properties</span></span>
|<span data-ttu-id="67211-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="67211-109">Property</span></span>|<span data-ttu-id="67211-110">Тип</span><span class="sxs-lookup"><span data-stu-id="67211-110">Type</span></span>|<span data-ttu-id="67211-111">Описание</span><span class="sxs-lookup"><span data-stu-id="67211-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67211-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="67211-112">hidePrivacySettings</span></span>|<span data-ttu-id="67211-113">Boolean.</span><span class="sxs-lookup"><span data-stu-id="67211-113">Boolean</span></span>|<span data-ttu-id="67211-114">Показать или скрыть параметры конфиденциальности для пользователя</span><span class="sxs-lookup"><span data-stu-id="67211-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="67211-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="67211-115">hideEULA</span></span>|<span data-ttu-id="67211-116">Boolean.</span><span class="sxs-lookup"><span data-stu-id="67211-116">Boolean</span></span>|<span data-ttu-id="67211-117">Показать или скрыть лицензионное соглашение для пользователя</span><span class="sxs-lookup"><span data-stu-id="67211-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="67211-118">userType</span><span class="sxs-lookup"><span data-stu-id="67211-118">userType</span></span>|[<span data-ttu-id="67211-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="67211-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="67211-120">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="67211-120">Type of user.</span></span> <span data-ttu-id="67211-121">Возможные значения: `administrator`, `standard`.</span><span class="sxs-lookup"><span data-stu-id="67211-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="67211-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="67211-122">deviceUsageType</span></span>|<span data-ttu-id="67211-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).</span><span class="sxs-lookup"><span data-stu-id="67211-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)</span></span>|<span data-ttu-id="67211-124">Тип проверки подлинности соединения AAD.</span><span class="sxs-lookup"><span data-stu-id="67211-124">AAD join authentication type.</span></span> <span data-ttu-id="67211-125">Возможные значения: `singleUser`, `shared`.</span><span class="sxs-lookup"><span data-stu-id="67211-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="67211-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="67211-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="67211-127">Boolean.</span><span class="sxs-lookup"><span data-stu-id="67211-127">Boolean</span></span>|<span data-ttu-id="67211-128">Если набор, а затем пропустить раскладка клавиатуры страницы Если значение языка и региона</span><span class="sxs-lookup"><span data-stu-id="67211-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="67211-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="67211-129">hideEscapeLink</span></span>|<span data-ttu-id="67211-130">Boolean.</span><span class="sxs-lookup"><span data-stu-id="67211-130">Boolean</span></span>|<span data-ttu-id="67211-131">Если параметр имеет значение true, затем пользователь не может запуститься через с другой учетной записи для входа в компании</span><span class="sxs-lookup"><span data-stu-id="67211-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="67211-132">Связи</span><span class="sxs-lookup"><span data-stu-id="67211-132">Relationships</span></span>
<span data-ttu-id="67211-133">Нет</span><span class="sxs-lookup"><span data-stu-id="67211-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="67211-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67211-134">JSON Representation</span></span>
<span data-ttu-id="67211-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67211-135">Here is a JSON representation of the resource.</span></span>
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





