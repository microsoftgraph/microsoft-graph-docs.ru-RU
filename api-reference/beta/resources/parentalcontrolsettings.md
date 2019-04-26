---
title: Тип ресурса Паренталконтролсеттингс
description: Указывает параметры родительского контроля для приложения. Эти параметры управляют согласия пользователя.
localization_priority: Normal
ms.openlocfilehash: 8e62e137b872437626a5c77c114f14c6ad0c5eb2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345001"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="1b4ea-104">Тип ресурса Паренталконтролсеттингс</span><span class="sxs-lookup"><span data-stu-id="1b4ea-104">parentalControlSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b4ea-105">Указывает параметры родительского контроля для приложения.</span><span class="sxs-lookup"><span data-stu-id="1b4ea-105">Specifies parental control settings for an application.</span></span> <span data-ttu-id="1b4ea-106">Эти параметры управляют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b4ea-106">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="1b4ea-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b4ea-107">Properties</span></span>

| <span data-ttu-id="1b4ea-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b4ea-108">Property</span></span> | <span data-ttu-id="1b4ea-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1b4ea-109">Type</span></span> | <span data-ttu-id="1b4ea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1b4ea-110">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="1b4ea-111">Каунтриесблоккедформинорс</span><span class="sxs-lookup"><span data-stu-id="1b4ea-111">countriesBlockedForMinors</span></span>|<span data-ttu-id="1b4ea-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1b4ea-112">String collection</span></span>| <span data-ttu-id="1b4ea-113">Задает [двузначные коды стран ISO](https://www.iso.org/iso-3166-country-codes.html).</span><span class="sxs-lookup"><span data-stu-id="1b4ea-113">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="1b4ea-114">Доступ к приложению будет заблокирован для небольших стран из стран, указанных в этом списке.</span><span class="sxs-lookup"><span data-stu-id="1b4ea-114">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="1b4ea-115">Легалажеграупруле</span><span class="sxs-lookup"><span data-stu-id="1b4ea-115">legalAgeGroupRule</span></span>| <span data-ttu-id="1b4ea-116">String</span><span class="sxs-lookup"><span data-stu-id="1b4ea-116">String</span></span> | <span data-ttu-id="1b4ea-117">Указывает правило группы допустимых возрастов, которое применяется к пользователям приложения.</span><span class="sxs-lookup"><span data-stu-id="1b4ea-117">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="1b4ea-118">Может иметь одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="1b4ea-118">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="1b4ea-119">Значение</span><span class="sxs-lookup"><span data-stu-id="1b4ea-119">Value</span></span></th><th><span data-ttu-id="1b4ea-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1b4ea-120">Description</span></span></th></tr><tr><td><span data-ttu-id="1b4ea-121">Разрешить</span><span class="sxs-lookup"><span data-stu-id="1b4ea-121">Allow</span></span></td><td><span data-ttu-id="1b4ea-122">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1b4ea-122">Default.</span></span> <span data-ttu-id="1b4ea-123">ПриМеняет юридическое минимальное значение.</span><span class="sxs-lookup"><span data-stu-id="1b4ea-123">Enforces the legal minimum.</span></span> <span data-ttu-id="1b4ea-124">Это означает, что для второстепенных стран Европейского союза и Корее требуются разрешения родителей.</span><span class="sxs-lookup"><span data-stu-id="1b4ea-124">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="1b4ea-125">Рекуиреконсентфорпривацисервицес</span><span class="sxs-lookup"><span data-stu-id="1b4ea-125">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="1b4ea-126">Указывает, что пользователь должен указать дату рождения для обеспечения соответствия правилам Коппа.</span><span class="sxs-lookup"><span data-stu-id="1b4ea-126">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="1b4ea-127">Рекуиреконсентформинорс</span><span class="sxs-lookup"><span data-stu-id="1b4ea-127">RequireConsentForMinors</span></span></td><td><span data-ttu-id="1b4ea-128">Для более ранних версий, независимо от правил для стран, требуется согласие пользователя в течение 18 лет.</span><span class="sxs-lookup"><span data-stu-id="1b4ea-128">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="1b4ea-129">Рекуиреконсентфоркидс</span><span class="sxs-lookup"><span data-stu-id="1b4ea-129">RequireConsentForKids</span></span></td><td><span data-ttu-id="1b4ea-130">Для более ранних версий, независимо от правил для стран, требуется согласие на родителей в течение 14 лет.</span><span class="sxs-lookup"><span data-stu-id="1b4ea-130">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="1b4ea-131">Блоккминорс</span><span class="sxs-lookup"><span data-stu-id="1b4ea-131">BlockMinors</span></span></td><td><span data-ttu-id="1b4ea-132">Блокирует небольшие из использования приложения.</span><span class="sxs-lookup"><span data-stu-id="1b4ea-132">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="1b4ea-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b4ea-133">JSON representation</span></span>
<span data-ttu-id="1b4ea-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b4ea-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.parentalControlSettings"
}-->
```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
