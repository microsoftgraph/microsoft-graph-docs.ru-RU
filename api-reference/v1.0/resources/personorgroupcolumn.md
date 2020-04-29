---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
description: Ресурс personOrGroupColumn в ресурсе columnDefinition указывает, что значения столбца представляют человека или группу, выбранные в каталоге.
doc_type: resourcePageType
ms.openlocfilehash: ea89377f38f820ec00fc38343ba714ec22a10c1c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447201"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="f21f5-103">Тип ресурса personOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="f21f5-103">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="f21f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f21f5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f21f5-105">Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="f21f5-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f21f5-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f21f5-106">JSON representation</span></span>

<span data-ttu-id="f21f5-107">Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f21f5-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="f21f5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f21f5-108">Properties</span></span>

| <span data-ttu-id="f21f5-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f21f5-109">Property name</span></span>              | <span data-ttu-id="f21f5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f21f5-110">Type</span></span>    | <span data-ttu-id="f21f5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f21f5-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="f21f5-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="f21f5-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="f21f5-113">boolean</span><span class="sxs-lookup"><span data-stu-id="f21f5-113">boolean</span></span> | <span data-ttu-id="f21f5-114">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="f21f5-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="f21f5-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="f21f5-115">**displayAs**</span></span>              | <span data-ttu-id="f21f5-116">string</span><span class="sxs-lookup"><span data-stu-id="f21f5-116">string</span></span>  | <span data-ttu-id="f21f5-117">Указывает способ отображения сведений о выбранном человеке или группе.</span><span class="sxs-lookup"><span data-stu-id="f21f5-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="f21f5-118">См. ниже.</span><span class="sxs-lookup"><span data-stu-id="f21f5-118">See below.</span></span>
| <span data-ttu-id="f21f5-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="f21f5-119">**chooseFromType**</span></span>         | <span data-ttu-id="f21f5-120">string</span><span class="sxs-lookup"><span data-stu-id="f21f5-120">string</span></span>  | <span data-ttu-id="f21f5-121">Указывает, что можно выбирать: только людей либо людей и группы.</span><span class="sxs-lookup"><span data-stu-id="f21f5-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="f21f5-122">Должно иметь тип `peopleAndGroups` или `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="f21f5-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="f21f5-123">Параметры DisplayAs</span><span class="sxs-lookup"><span data-stu-id="f21f5-123">DisplayAs options</span></span>

| <span data-ttu-id="f21f5-124">Значение DisplayAs</span><span class="sxs-lookup"><span data-stu-id="f21f5-124">DisplayAs value</span></span>               | <span data-ttu-id="f21f5-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f21f5-125">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="f21f5-126">**account**</span><span class="sxs-lookup"><span data-stu-id="f21f5-126">**account**</span></span>                   | <span data-ttu-id="f21f5-127">Необработанная закодированная строка утверждения SharePoint для человека или группы (например,</span><span class="sxs-lookup"><span data-stu-id="f21f5-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="f21f5-128">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="f21f5-128">i:0#.f</span></span>|<span data-ttu-id="f21f5-129">membership</span><span class="sxs-lookup"><span data-stu-id="f21f5-129">membership</span></span>|<span data-ttu-id="f21f5-130">olga@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="f21f5-130">jane@contoso.com).</span></span>
| <span data-ttu-id="f21f5-131">**department**</span><span class="sxs-lookup"><span data-stu-id="f21f5-131">**department**</span></span>                | <span data-ttu-id="f21f5-132">Отдел человека или группы.</span><span class="sxs-lookup"><span data-stu-id="f21f5-132">The person or group's department.</span></span>
| <span data-ttu-id="f21f5-133">**firstName**</span><span class="sxs-lookup"><span data-stu-id="f21f5-133">**firstName**</span></span>                 | <span data-ttu-id="f21f5-134">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="f21f5-134">The person's first name.</span></span>
| <span data-ttu-id="f21f5-135">**id**</span><span class="sxs-lookup"><span data-stu-id="f21f5-135">**id**</span></span>                        | <span data-ttu-id="f21f5-136">Идентификатор человека или группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="f21f5-136">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="f21f5-137">**lastName**</span><span class="sxs-lookup"><span data-stu-id="f21f5-137">**lastName**</span></span>                  | <span data-ttu-id="f21f5-138">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="f21f5-138">The person's last name.</span></span>
| <span data-ttu-id="f21f5-139">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="f21f5-139">**mobilePhone**</span></span>               | <span data-ttu-id="f21f5-140">Номер мобильного телефона человека.</span><span class="sxs-lookup"><span data-stu-id="f21f5-140">The person's mobile phone number.</span></span>
| <span data-ttu-id="f21f5-141">**name**</span><span class="sxs-lookup"><span data-stu-id="f21f5-141">**name**</span></span>                      | <span data-ttu-id="f21f5-142">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="f21f5-142">The person's name.</span></span>
| <span data-ttu-id="f21f5-143">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="f21f5-143">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="f21f5-144">Имя человека, а также его изображение и дополнительные сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="f21f5-144">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="f21f5-145">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="f21f5-145">**nameWithPresence**</span></span>          | <span data-ttu-id="f21f5-146">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f21f5-146">Default.</span></span> <span data-ttu-id="f21f5-147">Имя человека со значком индикатора присутствия (доступен, занят и т. д.)</span><span class="sxs-lookup"><span data-stu-id="f21f5-147">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="f21f5-148">**office**</span><span class="sxs-lookup"><span data-stu-id="f21f5-148">**office**</span></span>                    | <span data-ttu-id="f21f5-149">Номер офиса человека.</span><span class="sxs-lookup"><span data-stu-id="f21f5-149">The person's office number.</span></span>
| <span data-ttu-id="f21f5-150">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="f21f5-150">**pictureOnly36x36**</span></span>          | <span data-ttu-id="f21f5-151">Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.</span><span class="sxs-lookup"><span data-stu-id="f21f5-151">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="f21f5-152">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="f21f5-152">**pictureOnly48x48**</span></span>          | <span data-ttu-id="f21f5-153">Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="f21f5-153">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="f21f5-154">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="f21f5-154">**pictureOnly72x72**</span></span>          | <span data-ttu-id="f21f5-155">Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.</span><span class="sxs-lookup"><span data-stu-id="f21f5-155">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="f21f5-156">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="f21f5-156">**sipAddress**</span></span>                | <span data-ttu-id="f21f5-157">SIP-адрес человека.</span><span class="sxs-lookup"><span data-stu-id="f21f5-157">The person's sip address.</span></span>
| <span data-ttu-id="f21f5-158">**title**</span><span class="sxs-lookup"><span data-stu-id="f21f5-158">**title**</span></span>                     | <span data-ttu-id="f21f5-159">Должность человека в организации.</span><span class="sxs-lookup"><span data-stu-id="f21f5-159">The person's title in the organization.</span></span>
| <span data-ttu-id="f21f5-160">**userName**</span><span class="sxs-lookup"><span data-stu-id="f21f5-160">**userName**</span></span>                  | <span data-ttu-id="f21f5-161">Имя пользователя человека или группы.</span><span class="sxs-lookup"><span data-stu-id="f21f5-161">The person or group's user name.</span></span>
| <span data-ttu-id="f21f5-162">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="f21f5-162">**workEmail**</span></span>                 | <span data-ttu-id="f21f5-163">Электронный адрес человека или группы.</span><span class="sxs-lookup"><span data-stu-id="f21f5-163">The person or group's email address.</span></span>
| <span data-ttu-id="f21f5-164">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="f21f5-164">**workPhone**</span></span>                 | <span data-ttu-id="f21f5-165">Номер рабочего телефона человека.</span><span class="sxs-lookup"><span data-stu-id="f21f5-165">The person's work phone number.</span></span>

<span data-ttu-id="f21f5-166">Примечание. Система может возвращать дополнительные типы DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="f21f5-166">Note: Additional DisplayAs types may be returned.</span></span>

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
