---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a1eb5b36f2af7b66da7fd891ccd324fa325504c3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923469"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="a2b46-102">Тип ресурса personOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="a2b46-102">PersonOrGroupColumn resource type</span></span>

> <span data-ttu-id="a2b46-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a2b46-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2b46-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2b46-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2b46-105">Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="a2b46-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2b46-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a2b46-106">JSON representation</span></span>

<span data-ttu-id="a2b46-107">Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2b46-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="a2b46-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2b46-108">Properties</span></span>

| <span data-ttu-id="a2b46-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a2b46-109">Property name</span></span>              | <span data-ttu-id="a2b46-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a2b46-110">Type</span></span>    | <span data-ttu-id="a2b46-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a2b46-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="a2b46-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="a2b46-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="a2b46-113">логический</span><span class="sxs-lookup"><span data-stu-id="a2b46-113">boolean</span></span> | <span data-ttu-id="a2b46-114">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="a2b46-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="a2b46-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="a2b46-115">**displayAs**</span></span>              | <span data-ttu-id="a2b46-116">строка</span><span class="sxs-lookup"><span data-stu-id="a2b46-116">string</span></span>  | <span data-ttu-id="a2b46-117">Указывает способ отображения сведений о выбранном человеке или группе.</span><span class="sxs-lookup"><span data-stu-id="a2b46-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="a2b46-118">См. ниже.</span><span class="sxs-lookup"><span data-stu-id="a2b46-118">See below.</span></span>
| <span data-ttu-id="a2b46-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="a2b46-119">**chooseFromType**</span></span>         | <span data-ttu-id="a2b46-120">строка</span><span class="sxs-lookup"><span data-stu-id="a2b46-120">string</span></span>  | <span data-ttu-id="a2b46-121">Указывает, что можно выбирать: только людей либо людей и группы.</span><span class="sxs-lookup"><span data-stu-id="a2b46-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="a2b46-122">Должно иметь тип `peopleAndGroups` или `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="a2b46-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="a2b46-123">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="a2b46-123">DisplayAs values</span></span>

| <span data-ttu-id="a2b46-124">Значение DisplayAs</span><span class="sxs-lookup"><span data-stu-id="a2b46-124">DisplayAs value</span></span>               | <span data-ttu-id="a2b46-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a2b46-125">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="a2b46-126">**account**</span><span class="sxs-lookup"><span data-stu-id="a2b46-126">**account**</span></span>                   | <span data-ttu-id="a2b46-127">Необработанная закодированная строка утверждения SharePoint для человека или группы (например,</span><span class="sxs-lookup"><span data-stu-id="a2b46-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="a2b46-128">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="a2b46-128">i:0#.f</span></span>|<span data-ttu-id="a2b46-129">membership</span><span class="sxs-lookup"><span data-stu-id="a2b46-129">membership</span></span>|<span data-ttu-id="a2b46-130">olga@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="a2b46-130">jane@contoso.com).</span></span>
| <span data-ttu-id="a2b46-131">**department**</span><span class="sxs-lookup"><span data-stu-id="a2b46-131">**department**</span></span>                | <span data-ttu-id="a2b46-132">Отдел человека или группы.</span><span class="sxs-lookup"><span data-stu-id="a2b46-132">The person or group's department.</span></span>
| <span data-ttu-id="a2b46-133">**firstName**</span><span class="sxs-lookup"><span data-stu-id="a2b46-133">**firstName**</span></span>                 | <span data-ttu-id="a2b46-134">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="a2b46-134">The person's first name.</span></span>
| <span data-ttu-id="a2b46-135">**id**</span><span class="sxs-lookup"><span data-stu-id="a2b46-135">**id**</span></span>                        | <span data-ttu-id="a2b46-136">Идентификатор человека или группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="a2b46-136">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="a2b46-137">**lastName**</span><span class="sxs-lookup"><span data-stu-id="a2b46-137">**lastName**</span></span>                  | <span data-ttu-id="a2b46-138">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="a2b46-138">The person's last name.</span></span>
| <span data-ttu-id="a2b46-139">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="a2b46-139">**mobilePhone**</span></span>               | <span data-ttu-id="a2b46-140">Номер мобильного телефона человека.</span><span class="sxs-lookup"><span data-stu-id="a2b46-140">The person's mobile phone number.</span></span>
| <span data-ttu-id="a2b46-141">**name**</span><span class="sxs-lookup"><span data-stu-id="a2b46-141">**name**</span></span>                      | <span data-ttu-id="a2b46-142">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="a2b46-142">The person's name.</span></span>
| <span data-ttu-id="a2b46-143">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="a2b46-143">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="a2b46-144">Имя человека, а также его изображение и дополнительные сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="a2b46-144">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="a2b46-145">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="a2b46-145">**nameWithPresence**</span></span>          | <span data-ttu-id="a2b46-146">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a2b46-146">Default.</span></span> <span data-ttu-id="a2b46-147">Имя человека со значком индикатора присутствия (доступен, занят и т. д.)</span><span class="sxs-lookup"><span data-stu-id="a2b46-147">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="a2b46-148">**office**</span><span class="sxs-lookup"><span data-stu-id="a2b46-148">**office**</span></span>                    | <span data-ttu-id="a2b46-149">Номер офиса человека.</span><span class="sxs-lookup"><span data-stu-id="a2b46-149">The person's office number.</span></span>
| <span data-ttu-id="a2b46-150">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="a2b46-150">**pictureOnly36x36**</span></span>          | <span data-ttu-id="a2b46-151">Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.</span><span class="sxs-lookup"><span data-stu-id="a2b46-151">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="a2b46-152">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="a2b46-152">**pictureOnly48x48**</span></span>          | <span data-ttu-id="a2b46-153">Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="a2b46-153">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="a2b46-154">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="a2b46-154">**pictureOnly72x72**</span></span>          | <span data-ttu-id="a2b46-155">Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.</span><span class="sxs-lookup"><span data-stu-id="a2b46-155">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="a2b46-156">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="a2b46-156">**sipAddress**</span></span>                | <span data-ttu-id="a2b46-157">SIP-адрес человека.</span><span class="sxs-lookup"><span data-stu-id="a2b46-157">The person's sip address.</span></span>
| <span data-ttu-id="a2b46-158">**title**</span><span class="sxs-lookup"><span data-stu-id="a2b46-158">**title**</span></span>                     | <span data-ttu-id="a2b46-159">Должность человека в организации.</span><span class="sxs-lookup"><span data-stu-id="a2b46-159">The person's title in the organization.</span></span>
| <span data-ttu-id="a2b46-160">**userName**</span><span class="sxs-lookup"><span data-stu-id="a2b46-160">**userName**</span></span>                  | <span data-ttu-id="a2b46-161">Имя пользователя человека или группы.</span><span class="sxs-lookup"><span data-stu-id="a2b46-161">The person or group's user name.</span></span>
| <span data-ttu-id="a2b46-162">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="a2b46-162">**workEmail**</span></span>                 | <span data-ttu-id="a2b46-163">Электронный адрес человека или группы.</span><span class="sxs-lookup"><span data-stu-id="a2b46-163">The person or group's email address.</span></span>
| <span data-ttu-id="a2b46-164">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="a2b46-164">**workPhone**</span></span>                 | <span data-ttu-id="a2b46-165">Номер рабочего телефона человека.</span><span class="sxs-lookup"><span data-stu-id="a2b46-165">The person's work phone number.</span></span>

<span data-ttu-id="a2b46-166">Примечание. Система может возвращать дополнительные типы DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="a2b46-166">Note: Additional DisplayAs types may be returned.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
