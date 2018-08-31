---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: 37c324ddb1863e3e589e7d17ea60bd879e50771f
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267558"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="86e44-102">Тип ресурса personOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="86e44-102">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="86e44-103">Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columnDefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="86e44-103">The **personOrGroupColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="86e44-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="86e44-104">JSON representation</span></span>

<span data-ttu-id="86e44-105">Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86e44-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="86e44-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="86e44-106">Properties</span></span>

| <span data-ttu-id="86e44-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="86e44-107">Property name</span></span>              | <span data-ttu-id="86e44-108">Тип</span><span class="sxs-lookup"><span data-stu-id="86e44-108">Type</span></span>    | <span data-ttu-id="86e44-109">Описание</span><span class="sxs-lookup"><span data-stu-id="86e44-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="86e44-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="86e44-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="86e44-111">логический</span><span class="sxs-lookup"><span data-stu-id="86e44-111">boolean</span></span> | <span data-ttu-id="86e44-112">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="86e44-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="86e44-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="86e44-113">**displayAs**</span></span>              | <span data-ttu-id="86e44-114">строка</span><span class="sxs-lookup"><span data-stu-id="86e44-114">string</span></span>  | <span data-ttu-id="86e44-115">Указывает способ отображения сведений о выбранном человеке или группе.</span><span class="sxs-lookup"><span data-stu-id="86e44-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="86e44-116">См. ниже.</span><span class="sxs-lookup"><span data-stu-id="86e44-116">See below.</span></span>
| <span data-ttu-id="86e44-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="86e44-117">**chooseFromType**</span></span>         | <span data-ttu-id="86e44-118">строка</span><span class="sxs-lookup"><span data-stu-id="86e44-118">string</span></span>  | <span data-ttu-id="86e44-119">Указывает, что можно выбирать: только людей либо людей и группы.</span><span class="sxs-lookup"><span data-stu-id="86e44-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="86e44-120">Должно иметь тип `peopleAndGroups` или `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="86e44-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="86e44-121">Параметры displayAs</span><span class="sxs-lookup"><span data-stu-id="86e44-121">DisplayAs options</span></span>

| <span data-ttu-id="86e44-122">Значение DisplayAs</span><span class="sxs-lookup"><span data-stu-id="86e44-122">DisplayAs value</span></span>               | <span data-ttu-id="86e44-123">Описание</span><span class="sxs-lookup"><span data-stu-id="86e44-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="86e44-124">**учетная запись**</span><span class="sxs-lookup"><span data-stu-id="86e44-124">**account**</span></span>                   | <span data-ttu-id="86e44-125">Необработанная закодированная строка утверждения SharePoint для человека или группы (например,</span><span class="sxs-lookup"><span data-stu-id="86e44-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="86e44-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="86e44-126">i:0#.f</span></span>|<span data-ttu-id="86e44-127">членство</span><span class="sxs-lookup"><span data-stu-id="86e44-127">membership</span></span>|<span data-ttu-id="86e44-128">olga@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="86e44-128">jane@contoso.com).</span></span>
| <span data-ttu-id="86e44-129">**отдел**</span><span class="sxs-lookup"><span data-stu-id="86e44-129">**department**</span></span>                | <span data-ttu-id="86e44-130">Отдел человека или группы.</span><span class="sxs-lookup"><span data-stu-id="86e44-130">The person or group's department.</span></span>
| <span data-ttu-id="86e44-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="86e44-131">**firstName**</span></span>                 | <span data-ttu-id="86e44-132">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="86e44-132">The person's first name.</span></span>
| <span data-ttu-id="86e44-133">**ИД**</span><span class="sxs-lookup"><span data-stu-id="86e44-133">**id**</span></span>                        | <span data-ttu-id="86e44-134">Идентификатор человека или группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="86e44-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="86e44-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="86e44-135">**lastName**</span></span>                  | <span data-ttu-id="86e44-136">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="86e44-136">The person's last name.</span></span>
| <span data-ttu-id="86e44-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="86e44-137">**mobilePhone**</span></span>               | <span data-ttu-id="86e44-138">Номер мобильного телефона человека.</span><span class="sxs-lookup"><span data-stu-id="86e44-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="86e44-139">**имя**</span><span class="sxs-lookup"><span data-stu-id="86e44-139">**name**</span></span>                      | <span data-ttu-id="86e44-140">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="86e44-140">The person's name.</span></span>
| <span data-ttu-id="86e44-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="86e44-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="86e44-142">Имя человека, а также его изображение и дополнительные сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="86e44-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="86e44-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="86e44-143">**nameWithPresence**</span></span>          | <span data-ttu-id="86e44-144">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="86e44-144">Default.</span></span> <span data-ttu-id="86e44-145">Имя человека со значком индикатора присутствия (доступен, занят и т. д.)</span><span class="sxs-lookup"><span data-stu-id="86e44-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="86e44-146">**офис**</span><span class="sxs-lookup"><span data-stu-id="86e44-146">**office**</span></span>                    | <span data-ttu-id="86e44-147">Номер офиса человека.</span><span class="sxs-lookup"><span data-stu-id="86e44-147">The person's office number.</span></span>
| <span data-ttu-id="86e44-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="86e44-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="86e44-149">Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.</span><span class="sxs-lookup"><span data-stu-id="86e44-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="86e44-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="86e44-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="86e44-151">Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="86e44-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="86e44-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="86e44-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="86e44-153">Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.</span><span class="sxs-lookup"><span data-stu-id="86e44-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="86e44-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="86e44-154">**sipAddress**</span></span>                | <span data-ttu-id="86e44-155">SIP-адрес человека.</span><span class="sxs-lookup"><span data-stu-id="86e44-155">The person's sip address.</span></span>
| <span data-ttu-id="86e44-156">**должность**</span><span class="sxs-lookup"><span data-stu-id="86e44-156">**title**</span></span>                     | <span data-ttu-id="86e44-157">Должность человека в организации.</span><span class="sxs-lookup"><span data-stu-id="86e44-157">The person's title in the organization.</span></span>
| <span data-ttu-id="86e44-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="86e44-158">**userName**</span></span>                  | <span data-ttu-id="86e44-159">Имя пользователя человека или группы.</span><span class="sxs-lookup"><span data-stu-id="86e44-159">The person or group's user name.</span></span>
| <span data-ttu-id="86e44-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="86e44-160">**workEmail**</span></span>                 | <span data-ttu-id="86e44-161">Электронный адрес человека или группы.</span><span class="sxs-lookup"><span data-stu-id="86e44-161">The person or group's email address.</span></span>
| <span data-ttu-id="86e44-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="86e44-162">**workPhone**</span></span>                 | <span data-ttu-id="86e44-163">Номер рабочего телефона человека.</span><span class="sxs-lookup"><span data-stu-id="86e44-163">The person's work phone number.</span></span>

<span data-ttu-id="86e44-164">Примечание. Система может возвращать дополнительные типы DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="86e44-164">Note: Additional DisplayAs types may be returned.</span></span>

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
