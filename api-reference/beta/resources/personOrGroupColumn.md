---
author: simonhult
description: Ресурс personOrGroupColumn в ресурсе columnDefinition указывает, что значения столбца представляют человека или группу, выбранные в каталоге.
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 261ed729bc865b6679bf6dc9d08060148f32006a
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176411"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="667a4-103">Тип ресурса personOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="667a4-103">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="667a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="667a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="667a4-105">Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="667a4-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="667a4-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="667a4-106">JSON representation</span></span>

<span data-ttu-id="667a4-107">Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="667a4-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="667a4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="667a4-108">Properties</span></span>

| <span data-ttu-id="667a4-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="667a4-109">Property name</span></span>              | <span data-ttu-id="667a4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="667a4-110">Type</span></span>    | <span data-ttu-id="667a4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="667a4-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="667a4-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="667a4-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="667a4-113">boolean</span><span class="sxs-lookup"><span data-stu-id="667a4-113">boolean</span></span> | <span data-ttu-id="667a4-114">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="667a4-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="667a4-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="667a4-115">**displayAs**</span></span>              | <span data-ttu-id="667a4-116">string</span><span class="sxs-lookup"><span data-stu-id="667a4-116">string</span></span>  | <span data-ttu-id="667a4-117">Указывает способ отображения сведений о выбранном человеке или группе.</span><span class="sxs-lookup"><span data-stu-id="667a4-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="667a4-118">См. ниже.</span><span class="sxs-lookup"><span data-stu-id="667a4-118">See below.</span></span>
| <span data-ttu-id="667a4-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="667a4-119">**chooseFromType**</span></span>         | <span data-ttu-id="667a4-120">string</span><span class="sxs-lookup"><span data-stu-id="667a4-120">string</span></span>  | <span data-ttu-id="667a4-121">Указывает, что можно выбирать: только людей либо людей и группы.</span><span class="sxs-lookup"><span data-stu-id="667a4-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="667a4-122">Должно иметь тип `peopleAndGroups` или `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="667a4-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="667a4-123">Значения displayAs</span><span class="sxs-lookup"><span data-stu-id="667a4-123">displayAs values</span></span>

| <span data-ttu-id="667a4-124">Значение</span><span class="sxs-lookup"><span data-stu-id="667a4-124">Value</span></span>               | <span data-ttu-id="667a4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="667a4-125">Description</span></span>                                                                                                 |
|:------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="667a4-126">**account**</span><span class="sxs-lookup"><span data-stu-id="667a4-126">**account**</span></span>                   | <span data-ttu-id="667a4-127">Необработанная закодированная строка утверждения SharePoint для человека или группы (например,</span><span class="sxs-lookup"><span data-stu-id="667a4-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="667a4-128">`i:0#.f|membership|jane@contoso.com`).</span><span class="sxs-lookup"><span data-stu-id="667a4-128">`i:0#.f|membership|jane@contoso.com`).</span></span> |
| <span data-ttu-id="667a4-129">**department**</span><span class="sxs-lookup"><span data-stu-id="667a4-129">**department**</span></span>                | <span data-ttu-id="667a4-130">Отдел человека или группы.</span><span class="sxs-lookup"><span data-stu-id="667a4-130">The person or group's department.</span></span>                                                                           |
| <span data-ttu-id="667a4-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="667a4-131">**firstName**</span></span>                 | <span data-ttu-id="667a4-132">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="667a4-132">The person's first name.</span></span>                                                                                    |
| <span data-ttu-id="667a4-133">**id**</span><span class="sxs-lookup"><span data-stu-id="667a4-133">**id**</span></span>                        | <span data-ttu-id="667a4-134">Идентификатор человека или группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="667a4-134">The id of the person or group in the directory.</span></span>                                                             |
| <span data-ttu-id="667a4-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="667a4-135">**lastName**</span></span>                  | <span data-ttu-id="667a4-136">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="667a4-136">The person's last name.</span></span>                                                                                     |
| <span data-ttu-id="667a4-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="667a4-137">**mobilePhone**</span></span>               | <span data-ttu-id="667a4-138">Номер мобильного телефона человека.</span><span class="sxs-lookup"><span data-stu-id="667a4-138">The person's mobile phone number.</span></span>                                                                           |
| <span data-ttu-id="667a4-139">**name**</span><span class="sxs-lookup"><span data-stu-id="667a4-139">**name**</span></span>                      | <span data-ttu-id="667a4-140">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="667a4-140">The person's name.</span></span>                                                                                          |
| <span data-ttu-id="667a4-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="667a4-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="667a4-142">Имя человека, а также его изображение и дополнительные сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="667a4-142">The person's name along with their picture and additional details.</span></span>                                          |
| <span data-ttu-id="667a4-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="667a4-143">**nameWithPresence**</span></span>          | <span data-ttu-id="667a4-144">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="667a4-144">Default.</span></span> <span data-ttu-id="667a4-145">Имя человека со значком индикатора присутствия (доступен, занят и т. д.)</span><span class="sxs-lookup"><span data-stu-id="667a4-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>                             |
| <span data-ttu-id="667a4-146">**office**</span><span class="sxs-lookup"><span data-stu-id="667a4-146">**office**</span></span>                    | <span data-ttu-id="667a4-147">Номер офиса человека.</span><span class="sxs-lookup"><span data-stu-id="667a4-147">The person's office number.</span></span>                                                                                 |
| <span data-ttu-id="667a4-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="667a4-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="667a4-149">Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.</span><span class="sxs-lookup"><span data-stu-id="667a4-149">The person's picture, bounded by a 36x36 px square.</span></span>                                                         |
| <span data-ttu-id="667a4-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="667a4-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="667a4-151">Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="667a4-151">The person's picture, bounded by a 48x48 px square.</span></span>                                                         |
| <span data-ttu-id="667a4-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="667a4-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="667a4-153">Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.</span><span class="sxs-lookup"><span data-stu-id="667a4-153">The person's picture, bounded by a 72x72 px square.</span></span>                                                         |
| <span data-ttu-id="667a4-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="667a4-154">**sipAddress**</span></span>                | <span data-ttu-id="667a4-155">SIP-адрес человека.</span><span class="sxs-lookup"><span data-stu-id="667a4-155">The person's sip address.</span></span>                                                                                   |
| <span data-ttu-id="667a4-156">**title**</span><span class="sxs-lookup"><span data-stu-id="667a4-156">**title**</span></span>                     | <span data-ttu-id="667a4-157">Должность человека в организации.</span><span class="sxs-lookup"><span data-stu-id="667a4-157">The person's title in the organization.</span></span>                                                                     |
| <span data-ttu-id="667a4-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="667a4-158">**userName**</span></span>                  | <span data-ttu-id="667a4-159">Имя пользователя человека или группы.</span><span class="sxs-lookup"><span data-stu-id="667a4-159">The person or group's user name.</span></span>                                                                            |
| <span data-ttu-id="667a4-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="667a4-160">**workEmail**</span></span>                 | <span data-ttu-id="667a4-161">Электронный адрес человека или группы.</span><span class="sxs-lookup"><span data-stu-id="667a4-161">The person or group's email address.</span></span>                                                                        |
| <span data-ttu-id="667a4-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="667a4-162">**workPhone**</span></span>                 | <span data-ttu-id="667a4-163">Номер рабочего телефона человека.</span><span class="sxs-lookup"><span data-stu-id="667a4-163">The person's work phone number.</span></span>                                                                             |

<span data-ttu-id="667a4-164">Примечание. Система может возвращать дополнительные типы DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="667a4-164">Note: Additional DisplayAs types may be returned.</span></span>

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


