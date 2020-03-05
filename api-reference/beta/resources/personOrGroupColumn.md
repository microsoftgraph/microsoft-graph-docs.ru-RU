---
author: simonhult
description: Ресурс personOrGroupColumn в ресурсе columnDefinition указывает, что значения столбца представляют человека или группу, выбранные в каталоге.
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 9b7901b52bcd877df16f5507c450425484ada703
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521934"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="01470-103">Тип ресурса personOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="01470-103">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="01470-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="01470-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01470-105">Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="01470-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="01470-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="01470-106">JSON representation</span></span>

<span data-ttu-id="01470-107">Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01470-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="01470-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="01470-108">Properties</span></span>

| <span data-ttu-id="01470-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="01470-109">Property name</span></span>              | <span data-ttu-id="01470-110">Тип</span><span class="sxs-lookup"><span data-stu-id="01470-110">Type</span></span>    | <span data-ttu-id="01470-111">Описание</span><span class="sxs-lookup"><span data-stu-id="01470-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="01470-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="01470-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="01470-113">boolean</span><span class="sxs-lookup"><span data-stu-id="01470-113">boolean</span></span> | <span data-ttu-id="01470-114">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="01470-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="01470-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="01470-115">**displayAs**</span></span>              | <span data-ttu-id="01470-116">строка</span><span class="sxs-lookup"><span data-stu-id="01470-116">string</span></span>  | <span data-ttu-id="01470-117">Указывает способ отображения сведений о выбранном человеке или группе.</span><span class="sxs-lookup"><span data-stu-id="01470-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="01470-118">См. ниже.</span><span class="sxs-lookup"><span data-stu-id="01470-118">See below.</span></span>
| <span data-ttu-id="01470-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="01470-119">**chooseFromType**</span></span>         | <span data-ttu-id="01470-120">string</span><span class="sxs-lookup"><span data-stu-id="01470-120">string</span></span>  | <span data-ttu-id="01470-121">Указывает, что можно выбирать: только людей либо людей и группы.</span><span class="sxs-lookup"><span data-stu-id="01470-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="01470-122">Должно иметь тип `peopleAndGroups` или `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="01470-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="01470-123">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="01470-123">DisplayAs values</span></span>

| <span data-ttu-id="01470-124">Значение DisplayAs</span><span class="sxs-lookup"><span data-stu-id="01470-124">DisplayAs value</span></span>               | <span data-ttu-id="01470-125">Описание</span><span class="sxs-lookup"><span data-stu-id="01470-125">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="01470-126">**account**</span><span class="sxs-lookup"><span data-stu-id="01470-126">**account**</span></span>                   | <span data-ttu-id="01470-127">Необработанная закодированная строка утверждения SharePoint для человека или группы (например,</span><span class="sxs-lookup"><span data-stu-id="01470-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="01470-128">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="01470-128">i:0#.f</span></span>|<span data-ttu-id="01470-129">membership</span><span class="sxs-lookup"><span data-stu-id="01470-129">membership</span></span>|<span data-ttu-id="01470-130">olga@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="01470-130">jane@contoso.com).</span></span>
| <span data-ttu-id="01470-131">**department**</span><span class="sxs-lookup"><span data-stu-id="01470-131">**department**</span></span>                | <span data-ttu-id="01470-132">Отдел человека или группы.</span><span class="sxs-lookup"><span data-stu-id="01470-132">The person or group's department.</span></span>
| <span data-ttu-id="01470-133">**firstName**</span><span class="sxs-lookup"><span data-stu-id="01470-133">**firstName**</span></span>                 | <span data-ttu-id="01470-134">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="01470-134">The person's first name.</span></span>
| <span data-ttu-id="01470-135">**id**</span><span class="sxs-lookup"><span data-stu-id="01470-135">**id**</span></span>                        | <span data-ttu-id="01470-136">Идентификатор человека или группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="01470-136">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="01470-137">**lastName**</span><span class="sxs-lookup"><span data-stu-id="01470-137">**lastName**</span></span>                  | <span data-ttu-id="01470-138">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="01470-138">The person's last name.</span></span>
| <span data-ttu-id="01470-139">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="01470-139">**mobilePhone**</span></span>               | <span data-ttu-id="01470-140">Номер мобильного телефона человека.</span><span class="sxs-lookup"><span data-stu-id="01470-140">The person's mobile phone number.</span></span>
| <span data-ttu-id="01470-141">**name**</span><span class="sxs-lookup"><span data-stu-id="01470-141">**name**</span></span>                      | <span data-ttu-id="01470-142">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="01470-142">The person's name.</span></span>
| <span data-ttu-id="01470-143">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="01470-143">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="01470-144">Имя человека, а также его изображение и дополнительные сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="01470-144">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="01470-145">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="01470-145">**nameWithPresence**</span></span>          | <span data-ttu-id="01470-146">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="01470-146">Default.</span></span> <span data-ttu-id="01470-147">Имя человека со значком индикатора присутствия (доступен, занят и т. д.)</span><span class="sxs-lookup"><span data-stu-id="01470-147">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="01470-148">**office**</span><span class="sxs-lookup"><span data-stu-id="01470-148">**office**</span></span>                    | <span data-ttu-id="01470-149">Номер офиса человека.</span><span class="sxs-lookup"><span data-stu-id="01470-149">The person's office number.</span></span>
| <span data-ttu-id="01470-150">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="01470-150">**pictureOnly36x36**</span></span>          | <span data-ttu-id="01470-151">Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.</span><span class="sxs-lookup"><span data-stu-id="01470-151">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="01470-152">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="01470-152">**pictureOnly48x48**</span></span>          | <span data-ttu-id="01470-153">Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="01470-153">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="01470-154">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="01470-154">**pictureOnly72x72**</span></span>          | <span data-ttu-id="01470-155">Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.</span><span class="sxs-lookup"><span data-stu-id="01470-155">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="01470-156">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="01470-156">**sipAddress**</span></span>                | <span data-ttu-id="01470-157">SIP-адрес человека.</span><span class="sxs-lookup"><span data-stu-id="01470-157">The person's sip address.</span></span>
| <span data-ttu-id="01470-158">**title**</span><span class="sxs-lookup"><span data-stu-id="01470-158">**title**</span></span>                     | <span data-ttu-id="01470-159">Должность человека в организации.</span><span class="sxs-lookup"><span data-stu-id="01470-159">The person's title in the organization.</span></span>
| <span data-ttu-id="01470-160">**userName**</span><span class="sxs-lookup"><span data-stu-id="01470-160">**userName**</span></span>                  | <span data-ttu-id="01470-161">Имя пользователя человека или группы.</span><span class="sxs-lookup"><span data-stu-id="01470-161">The person or group's user name.</span></span>
| <span data-ttu-id="01470-162">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="01470-162">**workEmail**</span></span>                 | <span data-ttu-id="01470-163">Электронный адрес человека или группы.</span><span class="sxs-lookup"><span data-stu-id="01470-163">The person or group's email address.</span></span>
| <span data-ttu-id="01470-164">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="01470-164">**workPhone**</span></span>                 | <span data-ttu-id="01470-165">Номер рабочего телефона человека.</span><span class="sxs-lookup"><span data-stu-id="01470-165">The person's work phone number.</span></span>

<span data-ttu-id="01470-166">Примечание. Система может возвращать дополнительные типы DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="01470-166">Note: Additional DisplayAs types may be returned.</span></span>

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
