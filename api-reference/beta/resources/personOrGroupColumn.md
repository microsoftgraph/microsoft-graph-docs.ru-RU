---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a3136d7c5b9563999eb9b21a9235317afdaeb63e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573944"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="45194-102">Тип ресурса personOrGroupColumn</span><span class="sxs-lookup"><span data-stu-id="45194-102">PersonOrGroupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45194-103">Ресурс **personOrGroupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют человека или группу, выбранные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="45194-103">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="45194-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="45194-104">JSON representation</span></span>

<span data-ttu-id="45194-105">Ниже показано представление ресурса **personOrGroupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45194-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="45194-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="45194-106">Properties</span></span>

| <span data-ttu-id="45194-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="45194-107">Property name</span></span>              | <span data-ttu-id="45194-108">Тип</span><span class="sxs-lookup"><span data-stu-id="45194-108">Type</span></span>    | <span data-ttu-id="45194-109">Описание</span><span class="sxs-lookup"><span data-stu-id="45194-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="45194-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="45194-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="45194-111">boolean</span><span class="sxs-lookup"><span data-stu-id="45194-111">boolean</span></span> | <span data-ttu-id="45194-112">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="45194-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="45194-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="45194-113">**displayAs**</span></span>              | <span data-ttu-id="45194-114">string</span><span class="sxs-lookup"><span data-stu-id="45194-114">string</span></span>  | <span data-ttu-id="45194-115">Указывает способ отображения сведений о выбранном человеке или группе.</span><span class="sxs-lookup"><span data-stu-id="45194-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="45194-116">См. ниже.</span><span class="sxs-lookup"><span data-stu-id="45194-116">See below.</span></span>
| <span data-ttu-id="45194-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="45194-117">**chooseFromType**</span></span>         | <span data-ttu-id="45194-118">string</span><span class="sxs-lookup"><span data-stu-id="45194-118">string</span></span>  | <span data-ttu-id="45194-119">Указывает, что можно выбирать: только людей либо людей и группы.</span><span class="sxs-lookup"><span data-stu-id="45194-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="45194-120">Должно иметь тип `peopleAndGroups` или `peopleOnly`.</span><span class="sxs-lookup"><span data-stu-id="45194-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="45194-121">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="45194-121">DisplayAs values</span></span>

| <span data-ttu-id="45194-122">Значение DisplayAs</span><span class="sxs-lookup"><span data-stu-id="45194-122">DisplayAs value</span></span>               | <span data-ttu-id="45194-123">Описание</span><span class="sxs-lookup"><span data-stu-id="45194-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="45194-124">**account**</span><span class="sxs-lookup"><span data-stu-id="45194-124">**account**</span></span>                   | <span data-ttu-id="45194-125">Необработанная закодированная строка утверждения SharePoint для человека или группы (например,</span><span class="sxs-lookup"><span data-stu-id="45194-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="45194-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="45194-126">i:0#.f</span></span>|<span data-ttu-id="45194-127">membership</span><span class="sxs-lookup"><span data-stu-id="45194-127">membership</span></span>|<span data-ttu-id="45194-128">olga@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="45194-128">jane@contoso.com).</span></span>
| <span data-ttu-id="45194-129">**department**</span><span class="sxs-lookup"><span data-stu-id="45194-129">**department**</span></span>                | <span data-ttu-id="45194-130">Отдел человека или группы.</span><span class="sxs-lookup"><span data-stu-id="45194-130">The person or group's department.</span></span>
| <span data-ttu-id="45194-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="45194-131">**firstName**</span></span>                 | <span data-ttu-id="45194-132">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="45194-132">The person's first name.</span></span>
| <span data-ttu-id="45194-133">**id**</span><span class="sxs-lookup"><span data-stu-id="45194-133">**id**</span></span>                        | <span data-ttu-id="45194-134">Идентификатор человека или группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="45194-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="45194-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="45194-135">**lastName**</span></span>                  | <span data-ttu-id="45194-136">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="45194-136">The person's last name.</span></span>
| <span data-ttu-id="45194-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="45194-137">**mobilePhone**</span></span>               | <span data-ttu-id="45194-138">Номер мобильного телефона человека.</span><span class="sxs-lookup"><span data-stu-id="45194-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="45194-139">**name**</span><span class="sxs-lookup"><span data-stu-id="45194-139">**name**</span></span>                      | <span data-ttu-id="45194-140">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="45194-140">The person's name.</span></span>
| <span data-ttu-id="45194-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="45194-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="45194-142">Имя человека, а также его изображение и дополнительные сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="45194-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="45194-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="45194-143">**nameWithPresence**</span></span>          | <span data-ttu-id="45194-144">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="45194-144">Default.</span></span> <span data-ttu-id="45194-145">Имя человека со значком индикатора присутствия (доступен, занят и т. д.)</span><span class="sxs-lookup"><span data-stu-id="45194-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="45194-146">**office**</span><span class="sxs-lookup"><span data-stu-id="45194-146">**office**</span></span>                    | <span data-ttu-id="45194-147">Номер офиса человека.</span><span class="sxs-lookup"><span data-stu-id="45194-147">The person's office number.</span></span>
| <span data-ttu-id="45194-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="45194-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="45194-149">Изображение человека, ограниченное квадратом размером 36 x 36 пикселей.</span><span class="sxs-lookup"><span data-stu-id="45194-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="45194-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="45194-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="45194-151">Изображение человека, ограниченное квадратом размером 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="45194-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="45194-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="45194-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="45194-153">Изображение человека, ограниченное квадратом размером 72 x 72 пикселей.</span><span class="sxs-lookup"><span data-stu-id="45194-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="45194-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="45194-154">**sipAddress**</span></span>                | <span data-ttu-id="45194-155">SIP-адрес человека.</span><span class="sxs-lookup"><span data-stu-id="45194-155">The person's sip address.</span></span>
| <span data-ttu-id="45194-156">**title**</span><span class="sxs-lookup"><span data-stu-id="45194-156">**title**</span></span>                     | <span data-ttu-id="45194-157">Должность человека в организации.</span><span class="sxs-lookup"><span data-stu-id="45194-157">The person's title in the organization.</span></span>
| <span data-ttu-id="45194-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="45194-158">**userName**</span></span>                  | <span data-ttu-id="45194-159">Имя пользователя человека или группы.</span><span class="sxs-lookup"><span data-stu-id="45194-159">The person or group's user name.</span></span>
| <span data-ttu-id="45194-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="45194-160">**workEmail**</span></span>                 | <span data-ttu-id="45194-161">Электронный адрес человека или группы.</span><span class="sxs-lookup"><span data-stu-id="45194-161">The person or group's email address.</span></span>
| <span data-ttu-id="45194-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="45194-162">**workPhone**</span></span>                 | <span data-ttu-id="45194-163">Номер рабочего телефона человека.</span><span class="sxs-lookup"><span data-stu-id="45194-163">The person's work phone number.</span></span>

<span data-ttu-id="45194-164">Примечание. Система может возвращать дополнительные типы DisplayAs.</span><span class="sxs-lookup"><span data-stu-id="45194-164">Note: Additional DisplayAs types may be returned.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/personOrGroupColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
