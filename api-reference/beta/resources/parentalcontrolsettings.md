---
title: Тип ресурса parentalControlSettings
description: Указывает параметры родительского элемента управления для приложения. Эти параметры определяют на взаимодействие с согласия пользователя.
localization_priority: Normal
ms.openlocfilehash: 52a808cd4c3e6f29e4d43c7c4ea5c9e30a81447b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528405"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="f6080-104">Тип ресурса parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="f6080-104">parentalControlSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6080-105">Указывает параметры родительского элемента управления для приложения.</span><span class="sxs-lookup"><span data-stu-id="f6080-105">Specifies parental control settings for an application.</span></span> <span data-ttu-id="f6080-106">Эти параметры определяют на взаимодействие с согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="f6080-106">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="f6080-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6080-107">Properties</span></span>

| <span data-ttu-id="f6080-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6080-108">Property</span></span> | <span data-ttu-id="f6080-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f6080-109">Type</span></span> | <span data-ttu-id="f6080-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f6080-110">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="f6080-111">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="f6080-111">countriesBlockedForMinors</span></span>|<span data-ttu-id="f6080-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f6080-112">String collection</span></span>| <span data-ttu-id="f6080-113">Указывает [двухбуквенный код страны ISO](https://www.iso.org/iso-3166-country-codes.html).</span><span class="sxs-lookup"><span data-stu-id="f6080-113">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="f6080-114">Доступ к приложению будут блокироваться для минорам из указанной в этом списке.</span><span class="sxs-lookup"><span data-stu-id="f6080-114">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="f6080-115">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="f6080-115">legalAgeGroupRule</span></span>| <span data-ttu-id="f6080-116">String</span><span class="sxs-lookup"><span data-stu-id="f6080-116">String</span></span> | <span data-ttu-id="f6080-117">Правило срок хранения в юридическом группы, которая применяется для пользователей приложения.</span><span class="sxs-lookup"><span data-stu-id="f6080-117">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="f6080-118">Может быть установлено одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="f6080-118">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="f6080-119">Значение</span><span class="sxs-lookup"><span data-stu-id="f6080-119">Value</span></span></th><th><span data-ttu-id="f6080-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f6080-120">Description</span></span></th></tr><tr><td><span data-ttu-id="f6080-121">Allow (разрешить)</span><span class="sxs-lookup"><span data-stu-id="f6080-121">Allow</span></span></td><td><span data-ttu-id="f6080-122">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6080-122">Default.</span></span> <span data-ttu-id="f6080-123">Требуют соблюдения юридических по меньшей мере.</span><span class="sxs-lookup"><span data-stu-id="f6080-123">Enforces the legal minimum.</span></span> <span data-ttu-id="f6080-124">Это означает, что является обязательным для минорам в Европейском союзе и Корея, родительское согласие.</span><span class="sxs-lookup"><span data-stu-id="f6080-124">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="f6080-125">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="f6080-125">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="f6080-126">Обеспечивает пользователю для указания Дата рождения в соответствии с правилами COPPA.</span><span class="sxs-lookup"><span data-stu-id="f6080-126">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="f6080-127">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="f6080-127">RequireConsentForMinors</span></span></td><td><span data-ttu-id="f6080-128">Требуется родительское согласие для возраста ниже 18, вне зависимости от страны дополнительный номер правила.</span><span class="sxs-lookup"><span data-stu-id="f6080-128">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="f6080-129">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="f6080-129">RequireConsentForKids</span></span></td><td><span data-ttu-id="f6080-130">Требуется родительское согласие для возраста ниже 14, вне зависимости от страны дополнительный номер правила.</span><span class="sxs-lookup"><span data-stu-id="f6080-130">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="f6080-131">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="f6080-131">BlockMinors</span></span></td><td><span data-ttu-id="f6080-132">Блоки минорам с помощью приложения.</span><span class="sxs-lookup"><span data-stu-id="f6080-132">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="f6080-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6080-133">JSON representation</span></span>
<span data-ttu-id="f6080-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6080-134">Here is a JSON representation of the resource.</span></span>

```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/parentalcontrolsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
