---
title: Тип ресурса Outofboxexperiencesettings.
description: Настройка "нет на месте"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dc5b5e69fa0b7bdeb8f4db515ccd163fefc1b34a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256360"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="27a40-103">Тип ресурса Outofboxexperiencesettings.</span><span class="sxs-lookup"><span data-stu-id="27a40-103">outOfBoxExperienceSettings resource type</span></span>

<span data-ttu-id="27a40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27a40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27a40-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27a40-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27a40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27a40-107">Настройка "нет на месте"</span><span class="sxs-lookup"><span data-stu-id="27a40-107">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="27a40-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="27a40-108">Properties</span></span>
|<span data-ttu-id="27a40-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="27a40-109">Property</span></span>|<span data-ttu-id="27a40-110">Тип</span><span class="sxs-lookup"><span data-stu-id="27a40-110">Type</span></span>|<span data-ttu-id="27a40-111">Описание</span><span class="sxs-lookup"><span data-stu-id="27a40-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27a40-112">хидепривацисеттингс</span><span class="sxs-lookup"><span data-stu-id="27a40-112">hidePrivacySettings</span></span>|<span data-ttu-id="27a40-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="27a40-113">Boolean</span></span>|<span data-ttu-id="27a40-114">Отображение или скрытие параметров конфиденциальности для пользователя</span><span class="sxs-lookup"><span data-stu-id="27a40-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="27a40-115">хидиула</span><span class="sxs-lookup"><span data-stu-id="27a40-115">hideEULA</span></span>|<span data-ttu-id="27a40-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="27a40-116">Boolean</span></span>|<span data-ttu-id="27a40-117">Отображение или скрытие лицензионного соглашения для пользователя</span><span class="sxs-lookup"><span data-stu-id="27a40-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="27a40-118">userType</span><span class="sxs-lookup"><span data-stu-id="27a40-118">userType</span></span>|[<span data-ttu-id="27a40-119">виндовсусертипе</span><span class="sxs-lookup"><span data-stu-id="27a40-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="27a40-120">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="27a40-120">Type of user.</span></span> <span data-ttu-id="27a40-121">Возможные значения: `administrator`, `standard`.</span><span class="sxs-lookup"><span data-stu-id="27a40-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="27a40-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="27a40-122">deviceUsageType</span></span>|<span data-ttu-id="27a40-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).</span><span class="sxs-lookup"><span data-stu-id="27a40-123">[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)</span></span>|<span data-ttu-id="27a40-124">Тип проверки подлинности присоединения AAD.</span><span class="sxs-lookup"><span data-stu-id="27a40-124">AAD join authentication type.</span></span> <span data-ttu-id="27a40-125">Возможные значения: `singleUser`, `shared`.</span><span class="sxs-lookup"><span data-stu-id="27a40-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="27a40-126">скипкэйбоардселектионпаже</span><span class="sxs-lookup"><span data-stu-id="27a40-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="27a40-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="27a40-127">Boolean</span></span>|<span data-ttu-id="27a40-128">Если задано, пропускать страницу "Выбор клавиатуры", если задан язык и регион</span><span class="sxs-lookup"><span data-stu-id="27a40-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="27a40-129">хидискапелинк</span><span class="sxs-lookup"><span data-stu-id="27a40-129">hideEscapeLink</span></span>|<span data-ttu-id="27a40-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="27a40-130">Boolean</span></span>|<span data-ttu-id="27a40-131">Если задано значение true, пользователь не сможет начать с другой учетной записи, при входе в компанию</span><span class="sxs-lookup"><span data-stu-id="27a40-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="27a40-132">Связи</span><span class="sxs-lookup"><span data-stu-id="27a40-132">Relationships</span></span>
<span data-ttu-id="27a40-133">Нет</span><span class="sxs-lookup"><span data-stu-id="27a40-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27a40-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27a40-134">JSON Representation</span></span>
<span data-ttu-id="27a40-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27a40-135">Here is a JSON representation of the resource.</span></span>
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




