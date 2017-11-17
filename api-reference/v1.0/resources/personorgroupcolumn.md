---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: 715c6ca22957cbd951784e6cf32edf2bf47f1098
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="2530d-102">Тип ресурса personOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="2530d-102">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="2530d-103">Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columnDefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="2530d-103">The **personOrGroupColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2530d-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2530d-104">JSON representation</span></span>

<span data-ttu-id="2530d-105">Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2530d-105">Here is a JSON representation of a **drive** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="2530d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2530d-106">Properties</span></span>

| <span data-ttu-id="2530d-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2530d-107">Property name</span></span>              | <span data-ttu-id="2530d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2530d-108">Type</span></span>    | <span data-ttu-id="2530d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2530d-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="2530d-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="2530d-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="2530d-111">логический</span><span class="sxs-lookup"><span data-stu-id="2530d-111">boolean</span></span> | <span data-ttu-id="2530d-112">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="2530d-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="2530d-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="2530d-113">**displayAs**</span></span>              | <span data-ttu-id="2530d-114">строка</span><span class="sxs-lookup"><span data-stu-id="2530d-114">string</span></span>  | <span data-ttu-id="2530d-115">Указывает способ отображения сведений о выбранном человеке или группе.</span><span class="sxs-lookup"><span data-stu-id="2530d-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="2530d-116">См. ниже.</span><span class="sxs-lookup"><span data-stu-id="2530d-116">See below.</span></span>
| <span data-ttu-id="2530d-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="2530d-117">**chooseFromType**</span></span>         | <span data-ttu-id="2530d-118">строка</span><span class="sxs-lookup"><span data-stu-id="2530d-118">string</span></span>  | <span data-ttu-id="2530d-119">Указывает, что можно выбирать: только людей либо людей и группы.</span><span class="sxs-lookup"><span data-stu-id="2530d-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="2530d-120">Должно иметь тип `peopleAndGroups` или `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="2530d-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="2530d-121">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="2530d-121">DisplayAs values</span></span>

| <span data-ttu-id="2530d-122">Значение DisplayAs</span><span class="sxs-lookup"><span data-stu-id="2530d-122">DisplayAs value</span></span>               | <span data-ttu-id="2530d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2530d-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="2530d-124">**account**</span><span class="sxs-lookup"><span data-stu-id="2530d-124">**Account**</span></span>                   | <span data-ttu-id="2530d-125">Необработанная закодированная строка утверждения SharePoint для человека или группы (например,</span><span class="sxs-lookup"><span data-stu-id="2530d-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="2530d-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="2530d-126">i:0#.f</span></span>|<span data-ttu-id="2530d-127">membership</span><span class="sxs-lookup"><span data-stu-id="2530d-127">membership</span></span>|<span data-ttu-id="2530d-128">olga@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="2530d-128">jane@contoso.com).</span></span>
| <span data-ttu-id="2530d-129">**department**</span><span class="sxs-lookup"><span data-stu-id="2530d-129">**department**</span></span>                | <span data-ttu-id="2530d-130">Отдел человека или группы.</span><span class="sxs-lookup"><span data-stu-id="2530d-130">The person or group's department.</span></span>
| <span data-ttu-id="2530d-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="2530d-131">**FirstName**</span></span>                 | <span data-ttu-id="2530d-132">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="2530d-132">The person's given name.</span></span>
| <span data-ttu-id="2530d-133">**id**</span><span class="sxs-lookup"><span data-stu-id="2530d-133">**id**</span></span>                        | <span data-ttu-id="2530d-134">Идентификатор человека или группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="2530d-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="2530d-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="2530d-135">**LastName**</span></span>                  | <span data-ttu-id="2530d-136">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="2530d-136">The person's given name.</span></span>
| <span data-ttu-id="2530d-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="2530d-137">**mobilePhone**</span></span>               | <span data-ttu-id="2530d-138">Номер мобильного телефона человека.</span><span class="sxs-lookup"><span data-stu-id="2530d-138">The contact's mobile phone number.</span></span>
| <span data-ttu-id="2530d-139">**name**</span><span class="sxs-lookup"><span data-stu-id="2530d-139">**name**</span></span>                      | <span data-ttu-id="2530d-140">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="2530d-140">The person's given name.</span></span>
| <span data-ttu-id="2530d-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="2530d-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="2530d-142">Имя человека, а также его изображение и дополнительные сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="2530d-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="2530d-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="2530d-143">**nameWithPresence**</span></span>          | <span data-ttu-id="2530d-144">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2530d-144">Default</span></span> <span data-ttu-id="2530d-145">Имя человека со значком индикатора присутствия (доступен, занят и т. д.)</span><span class="sxs-lookup"><span data-stu-id="2530d-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="2530d-146">**office**</span><span class="sxs-lookup"><span data-stu-id="2530d-146">**Office**</span></span>                    | <span data-ttu-id="2530d-147">Номер офиса человека.</span><span class="sxs-lookup"><span data-stu-id="2530d-147">The person's office number.</span></span>
| <span data-ttu-id="2530d-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="2530d-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="2530d-149">Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.</span><span class="sxs-lookup"><span data-stu-id="2530d-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="2530d-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="2530d-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="2530d-151">Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="2530d-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="2530d-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="2530d-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="2530d-153">Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.</span><span class="sxs-lookup"><span data-stu-id="2530d-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="2530d-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="2530d-154">**sipAddress**</span></span>                | <span data-ttu-id="2530d-155">SIP-адрес человека.</span><span class="sxs-lookup"><span data-stu-id="2530d-155">The person's sip address.</span></span>
| <span data-ttu-id="2530d-156">**title**</span><span class="sxs-lookup"><span data-stu-id="2530d-156">**title**</span></span>                     | <span data-ttu-id="2530d-157">Должность человека в организации.</span><span class="sxs-lookup"><span data-stu-id="2530d-157">The person's title in the organization.</span></span>
| <span data-ttu-id="2530d-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="2530d-158">**Username**</span></span>                  | <span data-ttu-id="2530d-159">Имя пользователя человека или группы.</span><span class="sxs-lookup"><span data-stu-id="2530d-159">The person or group's user name.</span></span>
| <span data-ttu-id="2530d-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="2530d-160">**workEmail**</span></span>                 | <span data-ttu-id="2530d-161">Электронный адрес человека или группы.</span><span class="sxs-lookup"><span data-stu-id="2530d-161">The person or group's email address.</span></span>
| <span data-ttu-id="2530d-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="2530d-162">**workPhone**</span></span>                 | <span data-ttu-id="2530d-163">Номер рабочего телефона человека.</span><span class="sxs-lookup"><span data-stu-id="2530d-163">The person's work phone number.</span></span>

<span data-ttu-id="2530d-164">Примечание. Система может возвращать дополнительные типы DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="2530d-164">Note: Additional DisplayAs types may be returned.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
