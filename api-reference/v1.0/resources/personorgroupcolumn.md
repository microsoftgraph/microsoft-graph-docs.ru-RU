---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
description: Ресурс personOrGroupColumn в ресурсе columnDefinition указывает, что значения столбца представляют человека или группу, выбранные в каталоге.
doc_type: resourcePageType
ms.openlocfilehash: 8d4875ba813f5c1491135b2d1615c4146b438304
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032420"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="07705-103">Тип ресурса personOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="07705-103">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="07705-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07705-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="07705-105">Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="07705-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07705-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="07705-106">JSON representation</span></span>

<span data-ttu-id="07705-107">Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07705-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="07705-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="07705-108">Properties</span></span>

| <span data-ttu-id="07705-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="07705-109">Property name</span></span>              | <span data-ttu-id="07705-110">Тип</span><span class="sxs-lookup"><span data-stu-id="07705-110">Type</span></span>    | <span data-ttu-id="07705-111">Описание</span><span class="sxs-lookup"><span data-stu-id="07705-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="07705-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="07705-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="07705-113">boolean</span><span class="sxs-lookup"><span data-stu-id="07705-113">boolean</span></span> | <span data-ttu-id="07705-114">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="07705-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="07705-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="07705-115">**displayAs**</span></span>              | <span data-ttu-id="07705-116">string</span><span class="sxs-lookup"><span data-stu-id="07705-116">string</span></span>  | <span data-ttu-id="07705-117">Указывает способ отображения сведений о выбранном человеке или группе.</span><span class="sxs-lookup"><span data-stu-id="07705-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="07705-118">См. ниже.</span><span class="sxs-lookup"><span data-stu-id="07705-118">See below.</span></span>
| <span data-ttu-id="07705-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="07705-119">**chooseFromType**</span></span>         | <span data-ttu-id="07705-120">string</span><span class="sxs-lookup"><span data-stu-id="07705-120">string</span></span>  | <span data-ttu-id="07705-121">Указывает, что можно выбирать: только людей либо людей и группы.</span><span class="sxs-lookup"><span data-stu-id="07705-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="07705-122">Должно иметь тип `peopleAndGroups` или `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="07705-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="07705-123">Параметры DisplayAs</span><span class="sxs-lookup"><span data-stu-id="07705-123">DisplayAs options</span></span>

| <span data-ttu-id="07705-124">Значение DisplayAs</span><span class="sxs-lookup"><span data-stu-id="07705-124">DisplayAs value</span></span>               | <span data-ttu-id="07705-125">Описание</span><span class="sxs-lookup"><span data-stu-id="07705-125">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="07705-126">**account**</span><span class="sxs-lookup"><span data-stu-id="07705-126">**account**</span></span>                   | <span data-ttu-id="07705-127">Необработанная закодированная строка утверждения SharePoint для человека или группы (например,</span><span class="sxs-lookup"><span data-stu-id="07705-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="07705-128">`i:0#.f|membership|jane@contoso.com`).</span><span class="sxs-lookup"><span data-stu-id="07705-128">`i:0#.f|membership|jane@contoso.com`).</span></span>
| <span data-ttu-id="07705-129">**department**</span><span class="sxs-lookup"><span data-stu-id="07705-129">**department**</span></span>                | <span data-ttu-id="07705-130">Отдел человека или группы.</span><span class="sxs-lookup"><span data-stu-id="07705-130">The person or group's department.</span></span>
| <span data-ttu-id="07705-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="07705-131">**firstName**</span></span>                 | <span data-ttu-id="07705-132">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="07705-132">The person's first name.</span></span>
| <span data-ttu-id="07705-133">**id**</span><span class="sxs-lookup"><span data-stu-id="07705-133">**id**</span></span>                        | <span data-ttu-id="07705-134">Идентификатор человека или группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="07705-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="07705-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="07705-135">**lastName**</span></span>                  | <span data-ttu-id="07705-136">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="07705-136">The person's last name.</span></span>
| <span data-ttu-id="07705-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="07705-137">**mobilePhone**</span></span>               | <span data-ttu-id="07705-138">Номер мобильного телефона человека.</span><span class="sxs-lookup"><span data-stu-id="07705-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="07705-139">**name**</span><span class="sxs-lookup"><span data-stu-id="07705-139">**name**</span></span>                      | <span data-ttu-id="07705-140">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="07705-140">The person's name.</span></span>
| <span data-ttu-id="07705-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="07705-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="07705-142">Имя человека, а также его изображение и дополнительные сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="07705-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="07705-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="07705-143">**nameWithPresence**</span></span>          | <span data-ttu-id="07705-144">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="07705-144">Default.</span></span> <span data-ttu-id="07705-145">Имя человека со значком индикатора присутствия (доступен, занят и т. д.)</span><span class="sxs-lookup"><span data-stu-id="07705-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="07705-146">**office**</span><span class="sxs-lookup"><span data-stu-id="07705-146">**office**</span></span>                    | <span data-ttu-id="07705-147">Номер офиса человека.</span><span class="sxs-lookup"><span data-stu-id="07705-147">The person's office number.</span></span>
| <span data-ttu-id="07705-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="07705-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="07705-149">Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.</span><span class="sxs-lookup"><span data-stu-id="07705-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="07705-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="07705-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="07705-151">Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="07705-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="07705-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="07705-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="07705-153">Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.</span><span class="sxs-lookup"><span data-stu-id="07705-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="07705-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="07705-154">**sipAddress**</span></span>                | <span data-ttu-id="07705-155">SIP-адрес человека.</span><span class="sxs-lookup"><span data-stu-id="07705-155">The person's sip address.</span></span>
| <span data-ttu-id="07705-156">**title**</span><span class="sxs-lookup"><span data-stu-id="07705-156">**title**</span></span>                     | <span data-ttu-id="07705-157">Должность человека в организации.</span><span class="sxs-lookup"><span data-stu-id="07705-157">The person's title in the organization.</span></span>
| <span data-ttu-id="07705-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="07705-158">**userName**</span></span>                  | <span data-ttu-id="07705-159">Имя пользователя человека или группы.</span><span class="sxs-lookup"><span data-stu-id="07705-159">The person or group's user name.</span></span>
| <span data-ttu-id="07705-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="07705-160">**workEmail**</span></span>                 | <span data-ttu-id="07705-161">Электронный адрес человека или группы.</span><span class="sxs-lookup"><span data-stu-id="07705-161">The person or group's email address.</span></span>
| <span data-ttu-id="07705-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="07705-162">**workPhone**</span></span>                 | <span data-ttu-id="07705-163">Номер рабочего телефона человека.</span><span class="sxs-lookup"><span data-stu-id="07705-163">The person's work phone number.</span></span>

<span data-ttu-id="07705-164">Примечание. Система может возвращать дополнительные типы DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="07705-164">Note: Additional DisplayAs types may be returned.</span></span>

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

