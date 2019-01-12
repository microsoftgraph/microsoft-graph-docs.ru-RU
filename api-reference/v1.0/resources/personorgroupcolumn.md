---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 5ff8d61a2796edd615a66416b4f8f4d6d565909a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985453"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="ddb23-102">Тип ресурса personOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="ddb23-102">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="ddb23-103">Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="ddb23-103">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddb23-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ddb23-104">JSON representation</span></span>

<span data-ttu-id="ddb23-105">Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddb23-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="ddb23-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ddb23-106">Properties</span></span>

| <span data-ttu-id="ddb23-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ddb23-107">Property name</span></span>              | <span data-ttu-id="ddb23-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ddb23-108">Type</span></span>    | <span data-ttu-id="ddb23-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ddb23-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="ddb23-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="ddb23-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="ddb23-111">boolean</span><span class="sxs-lookup"><span data-stu-id="ddb23-111">boolean</span></span> | <span data-ttu-id="ddb23-112">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="ddb23-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="ddb23-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="ddb23-113">**displayAs**</span></span>              | <span data-ttu-id="ddb23-114">string</span><span class="sxs-lookup"><span data-stu-id="ddb23-114">string</span></span>  | <span data-ttu-id="ddb23-115">Указывает способ отображения сведений о выбранном человеке или группе.</span><span class="sxs-lookup"><span data-stu-id="ddb23-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="ddb23-116">См. ниже.</span><span class="sxs-lookup"><span data-stu-id="ddb23-116">See below.</span></span>
| <span data-ttu-id="ddb23-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="ddb23-117">**chooseFromType**</span></span>         | <span data-ttu-id="ddb23-118">string</span><span class="sxs-lookup"><span data-stu-id="ddb23-118">string</span></span>  | <span data-ttu-id="ddb23-119">Указывает, что можно выбирать: только людей либо людей и группы.</span><span class="sxs-lookup"><span data-stu-id="ddb23-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="ddb23-120">Должно иметь тип `peopleAndGroups` или `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="ddb23-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="ddb23-121">Параметры displayAs</span><span class="sxs-lookup"><span data-stu-id="ddb23-121">DisplayAs options</span></span>

| <span data-ttu-id="ddb23-122">Значение DisplayAs</span><span class="sxs-lookup"><span data-stu-id="ddb23-122">DisplayAs value</span></span>               | <span data-ttu-id="ddb23-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ddb23-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="ddb23-124">**account**</span><span class="sxs-lookup"><span data-stu-id="ddb23-124">**account**</span></span>                   | <span data-ttu-id="ddb23-125">Необработанная закодированная строка утверждения SharePoint для человека или группы (например,</span><span class="sxs-lookup"><span data-stu-id="ddb23-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="ddb23-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="ddb23-126">i:0#.f</span></span>|<span data-ttu-id="ddb23-127">membership</span><span class="sxs-lookup"><span data-stu-id="ddb23-127">membership</span></span>|<span data-ttu-id="ddb23-128">olga@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="ddb23-128">jane@contoso.com).</span></span>
| <span data-ttu-id="ddb23-129">**department**</span><span class="sxs-lookup"><span data-stu-id="ddb23-129">**department**</span></span>                | <span data-ttu-id="ddb23-130">Отдел человека или группы.</span><span class="sxs-lookup"><span data-stu-id="ddb23-130">The person or group's department.</span></span>
| <span data-ttu-id="ddb23-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="ddb23-131">**firstName**</span></span>                 | <span data-ttu-id="ddb23-132">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="ddb23-132">The person's first name.</span></span>
| <span data-ttu-id="ddb23-133">**id**</span><span class="sxs-lookup"><span data-stu-id="ddb23-133">**id**</span></span>                        | <span data-ttu-id="ddb23-134">Идентификатор человека или группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="ddb23-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="ddb23-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="ddb23-135">**lastName**</span></span>                  | <span data-ttu-id="ddb23-136">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="ddb23-136">The person's last name.</span></span>
| <span data-ttu-id="ddb23-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="ddb23-137">**mobilePhone**</span></span>               | <span data-ttu-id="ddb23-138">Номер мобильного телефона человека.</span><span class="sxs-lookup"><span data-stu-id="ddb23-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="ddb23-139">**name**</span><span class="sxs-lookup"><span data-stu-id="ddb23-139">**name**</span></span>                      | <span data-ttu-id="ddb23-140">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="ddb23-140">The person's name.</span></span>
| <span data-ttu-id="ddb23-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="ddb23-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="ddb23-142">Имя человека, а также его изображение и дополнительные сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="ddb23-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="ddb23-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="ddb23-143">**nameWithPresence**</span></span>          | <span data-ttu-id="ddb23-144">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ddb23-144">Default.</span></span> <span data-ttu-id="ddb23-145">Имя человека со значком индикатора присутствия (доступен, занят и т. д.)</span><span class="sxs-lookup"><span data-stu-id="ddb23-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="ddb23-146">**office**</span><span class="sxs-lookup"><span data-stu-id="ddb23-146">**office**</span></span>                    | <span data-ttu-id="ddb23-147">Номер офиса человека.</span><span class="sxs-lookup"><span data-stu-id="ddb23-147">The person's office number.</span></span>
| <span data-ttu-id="ddb23-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="ddb23-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="ddb23-149">Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.</span><span class="sxs-lookup"><span data-stu-id="ddb23-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="ddb23-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="ddb23-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="ddb23-151">Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="ddb23-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="ddb23-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="ddb23-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="ddb23-153">Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.</span><span class="sxs-lookup"><span data-stu-id="ddb23-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="ddb23-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="ddb23-154">**sipAddress**</span></span>                | <span data-ttu-id="ddb23-155">SIP-адрес человека.</span><span class="sxs-lookup"><span data-stu-id="ddb23-155">The person's sip address.</span></span>
| <span data-ttu-id="ddb23-156">**title**</span><span class="sxs-lookup"><span data-stu-id="ddb23-156">**title**</span></span>                     | <span data-ttu-id="ddb23-157">Должность человека в организации.</span><span class="sxs-lookup"><span data-stu-id="ddb23-157">The person's title in the organization.</span></span>
| <span data-ttu-id="ddb23-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="ddb23-158">**userName**</span></span>                  | <span data-ttu-id="ddb23-159">Имя пользователя человека или группы.</span><span class="sxs-lookup"><span data-stu-id="ddb23-159">The person or group's user name.</span></span>
| <span data-ttu-id="ddb23-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="ddb23-160">**workEmail**</span></span>                 | <span data-ttu-id="ddb23-161">Электронный адрес человека или группы.</span><span class="sxs-lookup"><span data-stu-id="ddb23-161">The person or group's email address.</span></span>
| <span data-ttu-id="ddb23-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="ddb23-162">**workPhone**</span></span>                 | <span data-ttu-id="ddb23-163">Номер рабочего телефона человека.</span><span class="sxs-lookup"><span data-stu-id="ddb23-163">The person's work phone number.</span></span>

<span data-ttu-id="ddb23-164">Примечание. Система может возвращать дополнительные типы DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="ddb23-164">Note: Additional DisplayAs types may be returned.</span></span>

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
