---
author: simonhult
description: Ресурс personOrGroupColumn в ресурсе columnDefinition указывает, что значения столбца представляют человека или группу, выбранные в каталоге.
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 51a6f8653becc78d8bd95f3bc5a18d9ac342bda8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998035"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="54af8-103">Тип ресурса personOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="54af8-103">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="54af8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54af8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54af8-105">Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="54af8-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="54af8-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="54af8-106">JSON representation</span></span>

<span data-ttu-id="54af8-107">Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54af8-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="54af8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="54af8-108">Properties</span></span>

| <span data-ttu-id="54af8-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="54af8-109">Property name</span></span>              | <span data-ttu-id="54af8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="54af8-110">Type</span></span>    | <span data-ttu-id="54af8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="54af8-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="54af8-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="54af8-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="54af8-113">boolean</span><span class="sxs-lookup"><span data-stu-id="54af8-113">boolean</span></span> | <span data-ttu-id="54af8-114">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="54af8-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="54af8-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="54af8-115">**displayAs**</span></span>              | <span data-ttu-id="54af8-116">string</span><span class="sxs-lookup"><span data-stu-id="54af8-116">string</span></span>  | <span data-ttu-id="54af8-117">Указывает способ отображения сведений о выбранном человеке или группе.</span><span class="sxs-lookup"><span data-stu-id="54af8-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="54af8-118">См. ниже.</span><span class="sxs-lookup"><span data-stu-id="54af8-118">See below.</span></span>
| <span data-ttu-id="54af8-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="54af8-119">**chooseFromType**</span></span>         | <span data-ttu-id="54af8-120">string</span><span class="sxs-lookup"><span data-stu-id="54af8-120">string</span></span>  | <span data-ttu-id="54af8-121">Указывает, что можно выбирать: только людей либо людей и группы.</span><span class="sxs-lookup"><span data-stu-id="54af8-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="54af8-122">Должно иметь тип `peopleAndGroups` или `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="54af8-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="54af8-123">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="54af8-123">DisplayAs values</span></span>

| <span data-ttu-id="54af8-124">Значение DisplayAs</span><span class="sxs-lookup"><span data-stu-id="54af8-124">DisplayAs value</span></span>               | <span data-ttu-id="54af8-125">Описание</span><span class="sxs-lookup"><span data-stu-id="54af8-125">Description</span></span>                                                                                                 |
|:------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="54af8-126">**account**</span><span class="sxs-lookup"><span data-stu-id="54af8-126">**account**</span></span>                   | <span data-ttu-id="54af8-127">Необработанная закодированная строка утверждения SharePoint для человека или группы (например,</span><span class="sxs-lookup"><span data-stu-id="54af8-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="54af8-128">`i:0#.f|membership|jane@contoso.com`).</span><span class="sxs-lookup"><span data-stu-id="54af8-128">`i:0#.f|membership|jane@contoso.com`).</span></span> |
| <span data-ttu-id="54af8-129">**department**</span><span class="sxs-lookup"><span data-stu-id="54af8-129">**department**</span></span>                | <span data-ttu-id="54af8-130">Отдел человека или группы.</span><span class="sxs-lookup"><span data-stu-id="54af8-130">The person or group's department.</span></span>                                                                           |
| <span data-ttu-id="54af8-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="54af8-131">**firstName**</span></span>                 | <span data-ttu-id="54af8-132">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="54af8-132">The person's first name.</span></span>                                                                                    |
| <span data-ttu-id="54af8-133">**id**</span><span class="sxs-lookup"><span data-stu-id="54af8-133">**id**</span></span>                        | <span data-ttu-id="54af8-134">Идентификатор человека или группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="54af8-134">The id of the person or group in the directory.</span></span>                                                             |
| <span data-ttu-id="54af8-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="54af8-135">**lastName**</span></span>                  | <span data-ttu-id="54af8-136">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="54af8-136">The person's last name.</span></span>                                                                                     |
| <span data-ttu-id="54af8-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="54af8-137">**mobilePhone**</span></span>               | <span data-ttu-id="54af8-138">Номер мобильного телефона человека.</span><span class="sxs-lookup"><span data-stu-id="54af8-138">The person's mobile phone number.</span></span>                                                                           |
| <span data-ttu-id="54af8-139">**name**</span><span class="sxs-lookup"><span data-stu-id="54af8-139">**name**</span></span>                      | <span data-ttu-id="54af8-140">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="54af8-140">The person's name.</span></span>                                                                                          |
| <span data-ttu-id="54af8-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="54af8-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="54af8-142">Имя человека, а также его изображение и дополнительные сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="54af8-142">The person's name along with their picture and additional details.</span></span>                                          |
| <span data-ttu-id="54af8-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="54af8-143">**nameWithPresence**</span></span>          | <span data-ttu-id="54af8-144">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="54af8-144">Default.</span></span> <span data-ttu-id="54af8-145">Имя человека со значком индикатора присутствия (доступен, занят и т. д.)</span><span class="sxs-lookup"><span data-stu-id="54af8-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>                             |
| <span data-ttu-id="54af8-146">**office**</span><span class="sxs-lookup"><span data-stu-id="54af8-146">**office**</span></span>                    | <span data-ttu-id="54af8-147">Номер офиса человека.</span><span class="sxs-lookup"><span data-stu-id="54af8-147">The person's office number.</span></span>                                                                                 |
| <span data-ttu-id="54af8-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="54af8-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="54af8-149">Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.</span><span class="sxs-lookup"><span data-stu-id="54af8-149">The person's picture, bounded by a 36x36 px square.</span></span>                                                         |
| <span data-ttu-id="54af8-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="54af8-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="54af8-151">Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="54af8-151">The person's picture, bounded by a 48x48 px square.</span></span>                                                         |
| <span data-ttu-id="54af8-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="54af8-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="54af8-153">Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.</span><span class="sxs-lookup"><span data-stu-id="54af8-153">The person's picture, bounded by a 72x72 px square.</span></span>                                                         |
| <span data-ttu-id="54af8-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="54af8-154">**sipAddress**</span></span>                | <span data-ttu-id="54af8-155">SIP-адрес человека.</span><span class="sxs-lookup"><span data-stu-id="54af8-155">The person's sip address.</span></span>                                                                                   |
| <span data-ttu-id="54af8-156">**title**</span><span class="sxs-lookup"><span data-stu-id="54af8-156">**title**</span></span>                     | <span data-ttu-id="54af8-157">Должность человека в организации.</span><span class="sxs-lookup"><span data-stu-id="54af8-157">The person's title in the organization.</span></span>                                                                     |
| <span data-ttu-id="54af8-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="54af8-158">**userName**</span></span>                  | <span data-ttu-id="54af8-159">Имя пользователя человека или группы.</span><span class="sxs-lookup"><span data-stu-id="54af8-159">The person or group's user name.</span></span>                                                                            |
| <span data-ttu-id="54af8-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="54af8-160">**workEmail**</span></span>                 | <span data-ttu-id="54af8-161">Электронный адрес человека или группы.</span><span class="sxs-lookup"><span data-stu-id="54af8-161">The person or group's email address.</span></span>                                                                        |
| <span data-ttu-id="54af8-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="54af8-162">**workPhone**</span></span>                 | <span data-ttu-id="54af8-163">Номер рабочего телефона человека.</span><span class="sxs-lookup"><span data-stu-id="54af8-163">The person's work phone number.</span></span>                                                                             |

<span data-ttu-id="54af8-164">Примечание. Система может возвращать дополнительные типы DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="54af8-164">Note: Additional DisplayAs types may be returned.</span></span>

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


