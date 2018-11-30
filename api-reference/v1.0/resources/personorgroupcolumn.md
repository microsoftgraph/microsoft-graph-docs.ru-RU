---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: b0c6eab7d2111870192a4ed6c30c1cbd72e4163e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027168"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="e4d61-102">Тип ресурса personOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="e4d61-102">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="e4d61-103">Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="e4d61-103">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4d61-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e4d61-104">JSON representation</span></span>

<span data-ttu-id="e4d61-105">Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4d61-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="e4d61-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4d61-106">Properties</span></span>

| <span data-ttu-id="e4d61-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e4d61-107">Property name</span></span>              | <span data-ttu-id="e4d61-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e4d61-108">Type</span></span>    | <span data-ttu-id="e4d61-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e4d61-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="e4d61-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="e4d61-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="e4d61-111">boolean</span><span class="sxs-lookup"><span data-stu-id="e4d61-111">boolean</span></span> | <span data-ttu-id="e4d61-112">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="e4d61-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="e4d61-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="e4d61-113">**displayAs**</span></span>              | <span data-ttu-id="e4d61-114">string</span><span class="sxs-lookup"><span data-stu-id="e4d61-114">string</span></span>  | <span data-ttu-id="e4d61-115">Указывает способ отображения сведений о выбранном человеке или группе.</span><span class="sxs-lookup"><span data-stu-id="e4d61-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="e4d61-116">См. ниже.</span><span class="sxs-lookup"><span data-stu-id="e4d61-116">See below.</span></span>
| <span data-ttu-id="e4d61-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="e4d61-117">**chooseFromType**</span></span>         | <span data-ttu-id="e4d61-118">string</span><span class="sxs-lookup"><span data-stu-id="e4d61-118">string</span></span>  | <span data-ttu-id="e4d61-119">Указывает, что можно выбирать: только людей либо людей и группы.</span><span class="sxs-lookup"><span data-stu-id="e4d61-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="e4d61-120">Должно иметь тип `peopleAndGroups` или `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="e4d61-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="e4d61-121">Параметры displayAs</span><span class="sxs-lookup"><span data-stu-id="e4d61-121">DisplayAs options</span></span>

| <span data-ttu-id="e4d61-122">Значение DisplayAs</span><span class="sxs-lookup"><span data-stu-id="e4d61-122">DisplayAs value</span></span>               | <span data-ttu-id="e4d61-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e4d61-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="e4d61-124">**account**</span><span class="sxs-lookup"><span data-stu-id="e4d61-124">**account**</span></span>                   | <span data-ttu-id="e4d61-125">Необработанная закодированная строка утверждения SharePoint для человека или группы (например,</span><span class="sxs-lookup"><span data-stu-id="e4d61-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="e4d61-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="e4d61-126">i:0#.f</span></span>|<span data-ttu-id="e4d61-127">membership</span><span class="sxs-lookup"><span data-stu-id="e4d61-127">membership</span></span>|<span data-ttu-id="e4d61-128">olga@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="e4d61-128">jane@contoso.com).</span></span>
| <span data-ttu-id="e4d61-129">**department**</span><span class="sxs-lookup"><span data-stu-id="e4d61-129">**department**</span></span>                | <span data-ttu-id="e4d61-130">Отдел человека или группы.</span><span class="sxs-lookup"><span data-stu-id="e4d61-130">The person or group's department.</span></span>
| <span data-ttu-id="e4d61-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="e4d61-131">**firstName**</span></span>                 | <span data-ttu-id="e4d61-132">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="e4d61-132">The person's first name.</span></span>
| <span data-ttu-id="e4d61-133">**id**</span><span class="sxs-lookup"><span data-stu-id="e4d61-133">**id**</span></span>                        | <span data-ttu-id="e4d61-134">Идентификатор человека или группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="e4d61-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="e4d61-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="e4d61-135">**lastName**</span></span>                  | <span data-ttu-id="e4d61-136">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="e4d61-136">The person's last name.</span></span>
| <span data-ttu-id="e4d61-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="e4d61-137">**mobilePhone**</span></span>               | <span data-ttu-id="e4d61-138">Номер мобильного телефона человека.</span><span class="sxs-lookup"><span data-stu-id="e4d61-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="e4d61-139">**name**</span><span class="sxs-lookup"><span data-stu-id="e4d61-139">**name**</span></span>                      | <span data-ttu-id="e4d61-140">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="e4d61-140">The person's name.</span></span>
| <span data-ttu-id="e4d61-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="e4d61-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="e4d61-142">Имя человека, а также его изображение и дополнительные сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="e4d61-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="e4d61-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="e4d61-143">**nameWithPresence**</span></span>          | <span data-ttu-id="e4d61-144">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e4d61-144">Default.</span></span> <span data-ttu-id="e4d61-145">Имя человека со значком индикатора присутствия (доступен, занят и т. д.)</span><span class="sxs-lookup"><span data-stu-id="e4d61-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="e4d61-146">**office**</span><span class="sxs-lookup"><span data-stu-id="e4d61-146">**office**</span></span>                    | <span data-ttu-id="e4d61-147">Номер офиса человека.</span><span class="sxs-lookup"><span data-stu-id="e4d61-147">The person's office number.</span></span>
| <span data-ttu-id="e4d61-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="e4d61-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="e4d61-149">Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.</span><span class="sxs-lookup"><span data-stu-id="e4d61-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="e4d61-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="e4d61-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="e4d61-151">Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="e4d61-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="e4d61-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="e4d61-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="e4d61-153">Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.</span><span class="sxs-lookup"><span data-stu-id="e4d61-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="e4d61-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="e4d61-154">**sipAddress**</span></span>                | <span data-ttu-id="e4d61-155">SIP-адрес человека.</span><span class="sxs-lookup"><span data-stu-id="e4d61-155">The person's sip address.</span></span>
| <span data-ttu-id="e4d61-156">**title**</span><span class="sxs-lookup"><span data-stu-id="e4d61-156">**title**</span></span>                     | <span data-ttu-id="e4d61-157">Должность человека в организации.</span><span class="sxs-lookup"><span data-stu-id="e4d61-157">The person's title in the organization.</span></span>
| <span data-ttu-id="e4d61-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="e4d61-158">**userName**</span></span>                  | <span data-ttu-id="e4d61-159">Имя пользователя человека или группы.</span><span class="sxs-lookup"><span data-stu-id="e4d61-159">The person or group's user name.</span></span>
| <span data-ttu-id="e4d61-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="e4d61-160">**workEmail**</span></span>                 | <span data-ttu-id="e4d61-161">Электронный адрес человека или группы.</span><span class="sxs-lookup"><span data-stu-id="e4d61-161">The person or group's email address.</span></span>
| <span data-ttu-id="e4d61-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="e4d61-162">**workPhone**</span></span>                 | <span data-ttu-id="e4d61-163">Номер рабочего телефона человека.</span><span class="sxs-lookup"><span data-stu-id="e4d61-163">The person's work phone number.</span></span>

<span data-ttu-id="e4d61-164">Примечание. Система может возвращать дополнительные типы DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="e4d61-164">Note: Additional DisplayAs types may be returned.</span></span>

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
