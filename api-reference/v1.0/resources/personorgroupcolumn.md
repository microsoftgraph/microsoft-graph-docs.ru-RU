---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
description: Ресурс personOrGroupColumn в ресурсе columnDefinition указывает, что значения столбца представляют человека или группу, выбранные в каталоге.
doc_type: resourcePageType
ms.openlocfilehash: d8ce31e7eb044e588f73afefb2b370e161fa7cdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035520"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="89570-103">Тип ресурса personOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="89570-103">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="89570-104">Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="89570-104">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89570-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="89570-105">JSON representation</span></span>

<span data-ttu-id="89570-106">Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89570-106">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="89570-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="89570-107">Properties</span></span>

| <span data-ttu-id="89570-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="89570-108">Property name</span></span>              | <span data-ttu-id="89570-109">Тип</span><span class="sxs-lookup"><span data-stu-id="89570-109">Type</span></span>    | <span data-ttu-id="89570-110">Описание</span><span class="sxs-lookup"><span data-stu-id="89570-110">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="89570-111">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="89570-111">**allowMultipleSelection**</span></span> | <span data-ttu-id="89570-112">boolean</span><span class="sxs-lookup"><span data-stu-id="89570-112">boolean</span></span> | <span data-ttu-id="89570-113">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="89570-113">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="89570-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="89570-114">**displayAs**</span></span>              | <span data-ttu-id="89570-115">string</span><span class="sxs-lookup"><span data-stu-id="89570-115">string</span></span>  | <span data-ttu-id="89570-116">Указывает способ отображения сведений о выбранном человеке или группе.</span><span class="sxs-lookup"><span data-stu-id="89570-116">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="89570-117">См. ниже.</span><span class="sxs-lookup"><span data-stu-id="89570-117">See below.</span></span>
| <span data-ttu-id="89570-118">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="89570-118">**chooseFromType**</span></span>         | <span data-ttu-id="89570-119">string</span><span class="sxs-lookup"><span data-stu-id="89570-119">string</span></span>  | <span data-ttu-id="89570-120">Указывает, что можно выбирать: только людей либо людей и группы.</span><span class="sxs-lookup"><span data-stu-id="89570-120">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="89570-121">Должно иметь тип `peopleAndGroups` или `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="89570-121">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="89570-122">Параметры DisplayAs</span><span class="sxs-lookup"><span data-stu-id="89570-122">DisplayAs options</span></span>

| <span data-ttu-id="89570-123">Значение DisplayAs</span><span class="sxs-lookup"><span data-stu-id="89570-123">DisplayAs value</span></span>               | <span data-ttu-id="89570-124">Описание</span><span class="sxs-lookup"><span data-stu-id="89570-124">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="89570-125">**account**</span><span class="sxs-lookup"><span data-stu-id="89570-125">**account**</span></span>                   | <span data-ttu-id="89570-126">Необработанная закодированная строка утверждения SharePoint для человека или группы (например,</span><span class="sxs-lookup"><span data-stu-id="89570-126">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="89570-127">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="89570-127">i:0#.f</span></span>|<span data-ttu-id="89570-128">membership</span><span class="sxs-lookup"><span data-stu-id="89570-128">membership</span></span>|<span data-ttu-id="89570-129">olga@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="89570-129">jane@contoso.com).</span></span>
| <span data-ttu-id="89570-130">**department**</span><span class="sxs-lookup"><span data-stu-id="89570-130">**department**</span></span>                | <span data-ttu-id="89570-131">Отдел человека или группы.</span><span class="sxs-lookup"><span data-stu-id="89570-131">The person or group's department.</span></span>
| <span data-ttu-id="89570-132">**firstName**</span><span class="sxs-lookup"><span data-stu-id="89570-132">**firstName**</span></span>                 | <span data-ttu-id="89570-133">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="89570-133">The person's first name.</span></span>
| <span data-ttu-id="89570-134">**id**</span><span class="sxs-lookup"><span data-stu-id="89570-134">**id**</span></span>                        | <span data-ttu-id="89570-135">Идентификатор человека или группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="89570-135">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="89570-136">**lastName**</span><span class="sxs-lookup"><span data-stu-id="89570-136">**lastName**</span></span>                  | <span data-ttu-id="89570-137">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="89570-137">The person's last name.</span></span>
| <span data-ttu-id="89570-138">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="89570-138">**mobilePhone**</span></span>               | <span data-ttu-id="89570-139">Номер мобильного телефона человека.</span><span class="sxs-lookup"><span data-stu-id="89570-139">The person's mobile phone number.</span></span>
| <span data-ttu-id="89570-140">**name**</span><span class="sxs-lookup"><span data-stu-id="89570-140">**name**</span></span>                      | <span data-ttu-id="89570-141">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="89570-141">The person's name.</span></span>
| <span data-ttu-id="89570-142">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="89570-142">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="89570-143">Имя человека, а также его изображение и дополнительные сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="89570-143">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="89570-144">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="89570-144">**nameWithPresence**</span></span>          | <span data-ttu-id="89570-145">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="89570-145">Default.</span></span> <span data-ttu-id="89570-146">Имя человека со значком индикатора присутствия (доступен, занят и т. д.)</span><span class="sxs-lookup"><span data-stu-id="89570-146">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="89570-147">**office**</span><span class="sxs-lookup"><span data-stu-id="89570-147">**office**</span></span>                    | <span data-ttu-id="89570-148">Номер офиса человека.</span><span class="sxs-lookup"><span data-stu-id="89570-148">The person's office number.</span></span>
| <span data-ttu-id="89570-149">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="89570-149">**pictureOnly36x36**</span></span>          | <span data-ttu-id="89570-150">Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.</span><span class="sxs-lookup"><span data-stu-id="89570-150">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="89570-151">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="89570-151">**pictureOnly48x48**</span></span>          | <span data-ttu-id="89570-152">Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="89570-152">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="89570-153">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="89570-153">**pictureOnly72x72**</span></span>          | <span data-ttu-id="89570-154">Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.</span><span class="sxs-lookup"><span data-stu-id="89570-154">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="89570-155">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="89570-155">**sipAddress**</span></span>                | <span data-ttu-id="89570-156">SIP-адрес человека.</span><span class="sxs-lookup"><span data-stu-id="89570-156">The person's sip address.</span></span>
| <span data-ttu-id="89570-157">**title**</span><span class="sxs-lookup"><span data-stu-id="89570-157">**title**</span></span>                     | <span data-ttu-id="89570-158">Должность человека в организации.</span><span class="sxs-lookup"><span data-stu-id="89570-158">The person's title in the organization.</span></span>
| <span data-ttu-id="89570-159">**userName**</span><span class="sxs-lookup"><span data-stu-id="89570-159">**userName**</span></span>                  | <span data-ttu-id="89570-160">Имя пользователя человека или группы.</span><span class="sxs-lookup"><span data-stu-id="89570-160">The person or group's user name.</span></span>
| <span data-ttu-id="89570-161">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="89570-161">**workEmail**</span></span>                 | <span data-ttu-id="89570-162">Электронный адрес человека или группы.</span><span class="sxs-lookup"><span data-stu-id="89570-162">The person or group's email address.</span></span>
| <span data-ttu-id="89570-163">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="89570-163">**workPhone**</span></span>                 | <span data-ttu-id="89570-164">Номер рабочего телефона человека.</span><span class="sxs-lookup"><span data-stu-id="89570-164">The person's work phone number.</span></span>

<span data-ttu-id="89570-165">Примечание. Система может возвращать дополнительные типы DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="89570-165">Note: Additional DisplayAs types may be returned.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(peopleAndGroups,peopleOnly) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(account,contentType,created,department,...) are in resource, but () are in table"
  ],
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
