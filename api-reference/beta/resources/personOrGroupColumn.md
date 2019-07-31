---
author: simonhult
description: Ресурс personOrGroupColumn в ресурсе columnDefinition указывает, что значения столбца представляют человека или группу, выбранные в каталоге.
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 24daf2ffd48e7647c898031aee634e8a84e05ee0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966155"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="5ba96-103">Тип ресурса personOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="5ba96-103">PersonOrGroupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ba96-104">Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="5ba96-104">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ba96-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5ba96-105">JSON representation</span></span>

<span data-ttu-id="5ba96-106">Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ba96-106">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="5ba96-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ba96-107">Properties</span></span>

| <span data-ttu-id="5ba96-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="5ba96-108">Property name</span></span>              | <span data-ttu-id="5ba96-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5ba96-109">Type</span></span>    | <span data-ttu-id="5ba96-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5ba96-110">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="5ba96-111">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="5ba96-111">**allowMultipleSelection**</span></span> | <span data-ttu-id="5ba96-112">boolean</span><span class="sxs-lookup"><span data-stu-id="5ba96-112">boolean</span></span> | <span data-ttu-id="5ba96-113">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="5ba96-113">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="5ba96-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="5ba96-114">**displayAs**</span></span>              | <span data-ttu-id="5ba96-115">string</span><span class="sxs-lookup"><span data-stu-id="5ba96-115">string</span></span>  | <span data-ttu-id="5ba96-116">Указывает способ отображения сведений о выбранном человеке или группе.</span><span class="sxs-lookup"><span data-stu-id="5ba96-116">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="5ba96-117">См. ниже.</span><span class="sxs-lookup"><span data-stu-id="5ba96-117">See below.</span></span>
| <span data-ttu-id="5ba96-118">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="5ba96-118">**chooseFromType**</span></span>         | <span data-ttu-id="5ba96-119">string</span><span class="sxs-lookup"><span data-stu-id="5ba96-119">string</span></span>  | <span data-ttu-id="5ba96-120">Указывает, что можно выбирать: только людей либо людей и группы.</span><span class="sxs-lookup"><span data-stu-id="5ba96-120">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="5ba96-121">Должно иметь тип `peopleAndGroups` или `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="5ba96-121">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="5ba96-122">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="5ba96-122">DisplayAs values</span></span>

| <span data-ttu-id="5ba96-123">Значение DisplayAs</span><span class="sxs-lookup"><span data-stu-id="5ba96-123">DisplayAs value</span></span>               | <span data-ttu-id="5ba96-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5ba96-124">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="5ba96-125">**account**</span><span class="sxs-lookup"><span data-stu-id="5ba96-125">**account**</span></span>                   | <span data-ttu-id="5ba96-126">Необработанная закодированная строка утверждения SharePoint для человека или группы (например,</span><span class="sxs-lookup"><span data-stu-id="5ba96-126">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="5ba96-127">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="5ba96-127">i:0#.f</span></span>|<span data-ttu-id="5ba96-128">membership</span><span class="sxs-lookup"><span data-stu-id="5ba96-128">membership</span></span>|<span data-ttu-id="5ba96-129">olga@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="5ba96-129">jane@contoso.com).</span></span>
| <span data-ttu-id="5ba96-130">**department**</span><span class="sxs-lookup"><span data-stu-id="5ba96-130">**department**</span></span>                | <span data-ttu-id="5ba96-131">Отдел человека или группы.</span><span class="sxs-lookup"><span data-stu-id="5ba96-131">The person or group's department.</span></span>
| <span data-ttu-id="5ba96-132">**firstName**</span><span class="sxs-lookup"><span data-stu-id="5ba96-132">**firstName**</span></span>                 | <span data-ttu-id="5ba96-133">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="5ba96-133">The person's first name.</span></span>
| <span data-ttu-id="5ba96-134">**id**</span><span class="sxs-lookup"><span data-stu-id="5ba96-134">**id**</span></span>                        | <span data-ttu-id="5ba96-135">Идентификатор человека или группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="5ba96-135">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="5ba96-136">**lastName**</span><span class="sxs-lookup"><span data-stu-id="5ba96-136">**lastName**</span></span>                  | <span data-ttu-id="5ba96-137">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="5ba96-137">The person's last name.</span></span>
| <span data-ttu-id="5ba96-138">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="5ba96-138">**mobilePhone**</span></span>               | <span data-ttu-id="5ba96-139">Номер мобильного телефона человека.</span><span class="sxs-lookup"><span data-stu-id="5ba96-139">The person's mobile phone number.</span></span>
| <span data-ttu-id="5ba96-140">**name**</span><span class="sxs-lookup"><span data-stu-id="5ba96-140">**name**</span></span>                      | <span data-ttu-id="5ba96-141">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="5ba96-141">The person's name.</span></span>
| <span data-ttu-id="5ba96-142">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="5ba96-142">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="5ba96-143">Имя человека, а также его изображение и дополнительные сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="5ba96-143">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="5ba96-144">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="5ba96-144">**nameWithPresence**</span></span>          | <span data-ttu-id="5ba96-145">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5ba96-145">Default.</span></span> <span data-ttu-id="5ba96-146">Имя человека со значком индикатора присутствия (доступен, занят и т. д.)</span><span class="sxs-lookup"><span data-stu-id="5ba96-146">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="5ba96-147">**office**</span><span class="sxs-lookup"><span data-stu-id="5ba96-147">**office**</span></span>                    | <span data-ttu-id="5ba96-148">Номер офиса человека.</span><span class="sxs-lookup"><span data-stu-id="5ba96-148">The person's office number.</span></span>
| <span data-ttu-id="5ba96-149">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="5ba96-149">**pictureOnly36x36**</span></span>          | <span data-ttu-id="5ba96-150">Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.</span><span class="sxs-lookup"><span data-stu-id="5ba96-150">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="5ba96-151">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="5ba96-151">**pictureOnly48x48**</span></span>          | <span data-ttu-id="5ba96-152">Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="5ba96-152">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="5ba96-153">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="5ba96-153">**pictureOnly72x72**</span></span>          | <span data-ttu-id="5ba96-154">Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.</span><span class="sxs-lookup"><span data-stu-id="5ba96-154">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="5ba96-155">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="5ba96-155">**sipAddress**</span></span>                | <span data-ttu-id="5ba96-156">SIP-адрес человека.</span><span class="sxs-lookup"><span data-stu-id="5ba96-156">The person's sip address.</span></span>
| <span data-ttu-id="5ba96-157">**title**</span><span class="sxs-lookup"><span data-stu-id="5ba96-157">**title**</span></span>                     | <span data-ttu-id="5ba96-158">Должность человека в организации.</span><span class="sxs-lookup"><span data-stu-id="5ba96-158">The person's title in the organization.</span></span>
| <span data-ttu-id="5ba96-159">**userName**</span><span class="sxs-lookup"><span data-stu-id="5ba96-159">**userName**</span></span>                  | <span data-ttu-id="5ba96-160">Имя пользователя человека или группы.</span><span class="sxs-lookup"><span data-stu-id="5ba96-160">The person or group's user name.</span></span>
| <span data-ttu-id="5ba96-161">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="5ba96-161">**workEmail**</span></span>                 | <span data-ttu-id="5ba96-162">Электронный адрес человека или группы.</span><span class="sxs-lookup"><span data-stu-id="5ba96-162">The person or group's email address.</span></span>
| <span data-ttu-id="5ba96-163">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="5ba96-163">**workPhone**</span></span>                 | <span data-ttu-id="5ba96-164">Номер рабочего телефона человека.</span><span class="sxs-lookup"><span data-stu-id="5ba96-164">The person's work phone number.</span></span>

<span data-ttu-id="5ba96-165">Примечание. Система может возвращать дополнительные типы DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="5ba96-165">Note: Additional DisplayAs types may be returned.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn",
  "suppressions": []
}
-->
