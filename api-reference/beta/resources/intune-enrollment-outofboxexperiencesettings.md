---
title: Тип ресурса Outofboxexperiencesettings.
description: Настройка "нет на месте"
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 65ea22f4a0684fb77b267d7793082ae066af5bd8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528265"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="fa128-103">Тип ресурса Outofboxexperiencesettings.</span><span class="sxs-lookup"><span data-stu-id="fa128-103">outOfBoxExperienceSettings resource type</span></span>

<span data-ttu-id="fa128-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fa128-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa128-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa128-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa128-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa128-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa128-107">Настройка "нет на месте"</span><span class="sxs-lookup"><span data-stu-id="fa128-107">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="fa128-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa128-108">Properties</span></span>
|<span data-ttu-id="fa128-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa128-109">Property</span></span>|<span data-ttu-id="fa128-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fa128-110">Type</span></span>|<span data-ttu-id="fa128-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fa128-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa128-112">хидепривацисеттингс</span><span class="sxs-lookup"><span data-stu-id="fa128-112">hidePrivacySettings</span></span>|<span data-ttu-id="fa128-113">Логический</span><span class="sxs-lookup"><span data-stu-id="fa128-113">Boolean</span></span>|<span data-ttu-id="fa128-114">Отображение или скрытие параметров конфиденциальности для пользователя</span><span class="sxs-lookup"><span data-stu-id="fa128-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="fa128-115">хидиула</span><span class="sxs-lookup"><span data-stu-id="fa128-115">hideEULA</span></span>|<span data-ttu-id="fa128-116">Логический</span><span class="sxs-lookup"><span data-stu-id="fa128-116">Boolean</span></span>|<span data-ttu-id="fa128-117">Отображение или скрытие лицензионного соглашения для пользователя</span><span class="sxs-lookup"><span data-stu-id="fa128-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="fa128-118">userType</span><span class="sxs-lookup"><span data-stu-id="fa128-118">userType</span></span>|[<span data-ttu-id="fa128-119">виндовсусертипе</span><span class="sxs-lookup"><span data-stu-id="fa128-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="fa128-120">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa128-120">Type of user.</span></span> <span data-ttu-id="fa128-121">Возможные значения: `administrator`, `standard`.</span><span class="sxs-lookup"><span data-stu-id="fa128-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="fa128-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="fa128-122">deviceUsageType</span></span>|<span data-ttu-id="fa128-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).</span><span class="sxs-lookup"><span data-stu-id="fa128-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)</span></span>|<span data-ttu-id="fa128-124">Тип проверки подлинности присоединения AAD.</span><span class="sxs-lookup"><span data-stu-id="fa128-124">AAD join authentication type.</span></span> <span data-ttu-id="fa128-125">Возможные значения: `singleUser`, `shared`.</span><span class="sxs-lookup"><span data-stu-id="fa128-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="fa128-126">скипкэйбоардселектионпаже</span><span class="sxs-lookup"><span data-stu-id="fa128-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="fa128-127">Логический</span><span class="sxs-lookup"><span data-stu-id="fa128-127">Boolean</span></span>|<span data-ttu-id="fa128-128">Если задано, пропускать страницу "Выбор клавиатуры", если задан язык и регион</span><span class="sxs-lookup"><span data-stu-id="fa128-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="fa128-129">хидискапелинк</span><span class="sxs-lookup"><span data-stu-id="fa128-129">hideEscapeLink</span></span>|<span data-ttu-id="fa128-130">Логический</span><span class="sxs-lookup"><span data-stu-id="fa128-130">Boolean</span></span>|<span data-ttu-id="fa128-131">Если задано значение true, пользователь не сможет начать с другой учетной записи, при входе в компанию</span><span class="sxs-lookup"><span data-stu-id="fa128-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa128-132">Связи</span><span class="sxs-lookup"><span data-stu-id="fa128-132">Relationships</span></span>
<span data-ttu-id="fa128-133">Нет</span><span class="sxs-lookup"><span data-stu-id="fa128-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa128-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa128-134">JSON Representation</span></span>
<span data-ttu-id="fa128-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa128-135">Here is a JSON representation of the resource.</span></span>
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



