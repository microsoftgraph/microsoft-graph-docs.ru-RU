---
title: Тип ресурса Outofboxexperiencesettings.
description: Настройка "нет на месте"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: df7137bfa4405e32887b1aa738d3b816ac3edf4a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728941"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="fcee7-103">Тип ресурса Outofboxexperiencesettings.</span><span class="sxs-lookup"><span data-stu-id="fcee7-103">outOfBoxExperienceSettings resource type</span></span>

<span data-ttu-id="fcee7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcee7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcee7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcee7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcee7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fcee7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcee7-107">Настройка "нет на месте"</span><span class="sxs-lookup"><span data-stu-id="fcee7-107">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="fcee7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcee7-108">Properties</span></span>
|<span data-ttu-id="fcee7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcee7-109">Property</span></span>|<span data-ttu-id="fcee7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fcee7-110">Type</span></span>|<span data-ttu-id="fcee7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fcee7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcee7-112">хидепривацисеттингс</span><span class="sxs-lookup"><span data-stu-id="fcee7-112">hidePrivacySettings</span></span>|<span data-ttu-id="fcee7-113">Логический</span><span class="sxs-lookup"><span data-stu-id="fcee7-113">Boolean</span></span>|<span data-ttu-id="fcee7-114">Отображение или скрытие параметров конфиденциальности для пользователя</span><span class="sxs-lookup"><span data-stu-id="fcee7-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="fcee7-115">хидиула</span><span class="sxs-lookup"><span data-stu-id="fcee7-115">hideEULA</span></span>|<span data-ttu-id="fcee7-116">Логический</span><span class="sxs-lookup"><span data-stu-id="fcee7-116">Boolean</span></span>|<span data-ttu-id="fcee7-117">Отображение или скрытие лицензионного соглашения для пользователя</span><span class="sxs-lookup"><span data-stu-id="fcee7-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="fcee7-118">userType</span><span class="sxs-lookup"><span data-stu-id="fcee7-118">userType</span></span>|[<span data-ttu-id="fcee7-119">виндовсусертипе</span><span class="sxs-lookup"><span data-stu-id="fcee7-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="fcee7-120">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="fcee7-120">Type of user.</span></span> <span data-ttu-id="fcee7-121">Возможные значения: `administrator`, `standard`.</span><span class="sxs-lookup"><span data-stu-id="fcee7-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="fcee7-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="fcee7-122">deviceUsageType</span></span>|<span data-ttu-id="fcee7-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).</span><span class="sxs-lookup"><span data-stu-id="fcee7-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)</span></span>|<span data-ttu-id="fcee7-124">Тип проверки подлинности присоединения AAD.</span><span class="sxs-lookup"><span data-stu-id="fcee7-124">AAD join authentication type.</span></span> <span data-ttu-id="fcee7-125">Возможные значения: `singleUser`, `shared`.</span><span class="sxs-lookup"><span data-stu-id="fcee7-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="fcee7-126">скипкэйбоардселектионпаже</span><span class="sxs-lookup"><span data-stu-id="fcee7-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="fcee7-127">Логический</span><span class="sxs-lookup"><span data-stu-id="fcee7-127">Boolean</span></span>|<span data-ttu-id="fcee7-128">Если задано, пропускать страницу "Выбор клавиатуры", если задан язык и регион</span><span class="sxs-lookup"><span data-stu-id="fcee7-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="fcee7-129">хидискапелинк</span><span class="sxs-lookup"><span data-stu-id="fcee7-129">hideEscapeLink</span></span>|<span data-ttu-id="fcee7-130">Логический</span><span class="sxs-lookup"><span data-stu-id="fcee7-130">Boolean</span></span>|<span data-ttu-id="fcee7-131">Если задано значение true, пользователь не сможет начать с другой учетной записи, при входе в компанию</span><span class="sxs-lookup"><span data-stu-id="fcee7-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="fcee7-132">Связи</span><span class="sxs-lookup"><span data-stu-id="fcee7-132">Relationships</span></span>
<span data-ttu-id="fcee7-133">Нет</span><span class="sxs-lookup"><span data-stu-id="fcee7-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fcee7-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcee7-134">JSON Representation</span></span>
<span data-ttu-id="fcee7-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcee7-135">Here is a JSON representation of the resource.</span></span>
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





