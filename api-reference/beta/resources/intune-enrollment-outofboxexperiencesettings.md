---
title: Тип ресурса Outofboxexperiencesettings.
description: Настройка "нет на месте"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a258adda7de3a44e33e980fd6e78f7065824ea91
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079908"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="43b81-103">Тип ресурса Outofboxexperiencesettings.</span><span class="sxs-lookup"><span data-stu-id="43b81-103">outOfBoxExperienceSettings resource type</span></span>

<span data-ttu-id="43b81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43b81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43b81-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43b81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43b81-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43b81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43b81-107">Настройка "нет на месте"</span><span class="sxs-lookup"><span data-stu-id="43b81-107">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="43b81-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="43b81-108">Properties</span></span>
|<span data-ttu-id="43b81-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="43b81-109">Property</span></span>|<span data-ttu-id="43b81-110">Тип</span><span class="sxs-lookup"><span data-stu-id="43b81-110">Type</span></span>|<span data-ttu-id="43b81-111">Описание</span><span class="sxs-lookup"><span data-stu-id="43b81-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43b81-112">хидепривацисеттингс</span><span class="sxs-lookup"><span data-stu-id="43b81-112">hidePrivacySettings</span></span>|<span data-ttu-id="43b81-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="43b81-113">Boolean</span></span>|<span data-ttu-id="43b81-114">Отображение или скрытие параметров конфиденциальности для пользователя</span><span class="sxs-lookup"><span data-stu-id="43b81-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="43b81-115">хидиула</span><span class="sxs-lookup"><span data-stu-id="43b81-115">hideEULA</span></span>|<span data-ttu-id="43b81-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="43b81-116">Boolean</span></span>|<span data-ttu-id="43b81-117">Отображение или скрытие лицензионного соглашения для пользователя</span><span class="sxs-lookup"><span data-stu-id="43b81-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="43b81-118">userType</span><span class="sxs-lookup"><span data-stu-id="43b81-118">userType</span></span>|[<span data-ttu-id="43b81-119">виндовсусертипе</span><span class="sxs-lookup"><span data-stu-id="43b81-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="43b81-120">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="43b81-120">Type of user.</span></span> <span data-ttu-id="43b81-121">Возможные значения: `administrator`, `standard`.</span><span class="sxs-lookup"><span data-stu-id="43b81-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="43b81-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="43b81-122">deviceUsageType</span></span>|<span data-ttu-id="43b81-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).</span><span class="sxs-lookup"><span data-stu-id="43b81-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)</span></span>|<span data-ttu-id="43b81-124">Тип проверки подлинности присоединения AAD.</span><span class="sxs-lookup"><span data-stu-id="43b81-124">AAD join authentication type.</span></span> <span data-ttu-id="43b81-125">Возможные значения: `singleUser`, `shared`.</span><span class="sxs-lookup"><span data-stu-id="43b81-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="43b81-126">скипкэйбоардселектионпаже</span><span class="sxs-lookup"><span data-stu-id="43b81-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="43b81-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="43b81-127">Boolean</span></span>|<span data-ttu-id="43b81-128">Если задано, пропускать страницу "Выбор клавиатуры", если задан язык и регион</span><span class="sxs-lookup"><span data-stu-id="43b81-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="43b81-129">хидискапелинк</span><span class="sxs-lookup"><span data-stu-id="43b81-129">hideEscapeLink</span></span>|<span data-ttu-id="43b81-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="43b81-130">Boolean</span></span>|<span data-ttu-id="43b81-131">Если задано значение true, пользователь не сможет начать с другой учетной записи, при входе в компанию</span><span class="sxs-lookup"><span data-stu-id="43b81-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="43b81-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="43b81-132">Relationships</span></span>
<span data-ttu-id="43b81-133">Нет</span><span class="sxs-lookup"><span data-stu-id="43b81-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43b81-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43b81-134">JSON Representation</span></span>
<span data-ttu-id="43b81-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43b81-135">Here is a JSON representation of the resource.</span></span>
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






