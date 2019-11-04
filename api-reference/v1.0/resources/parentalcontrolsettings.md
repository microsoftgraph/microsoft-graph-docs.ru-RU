---
title: Тип ресурса Паренталконтролсеттингс
description: Указывает параметры родительского контроля для приложения. Эти параметры управляют согласия пользователя.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 91adec95d9755d998dd48e7f100366ed9d38aa5d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938865"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="954d3-104">Тип ресурса Паренталконтролсеттингс</span><span class="sxs-lookup"><span data-stu-id="954d3-104">parentalControlSettings resource type</span></span>

<span data-ttu-id="954d3-105">Указывает параметры родительского контроля для приложения.</span><span class="sxs-lookup"><span data-stu-id="954d3-105">Specifies parental control settings for an application.</span></span> <span data-ttu-id="954d3-106">Эти параметры управляют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="954d3-106">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="954d3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="954d3-107">Properties</span></span>

| <span data-ttu-id="954d3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="954d3-108">Property</span></span> | <span data-ttu-id="954d3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="954d3-109">Type</span></span> | <span data-ttu-id="954d3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="954d3-110">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="954d3-111">каунтриесблоккедформинорс</span><span class="sxs-lookup"><span data-stu-id="954d3-111">countriesBlockedForMinors</span></span>|<span data-ttu-id="954d3-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="954d3-112">String collection</span></span>| <span data-ttu-id="954d3-113">Задает [двузначные коды стран ISO](https://www.iso.org/iso-3166-country-codes.html).</span><span class="sxs-lookup"><span data-stu-id="954d3-113">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="954d3-114">Доступ к приложению будет заблокирован для небольших стран из стран, указанных в этом списке.</span><span class="sxs-lookup"><span data-stu-id="954d3-114">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="954d3-115">легалажеграупруле</span><span class="sxs-lookup"><span data-stu-id="954d3-115">legalAgeGroupRule</span></span>| <span data-ttu-id="954d3-116">String</span><span class="sxs-lookup"><span data-stu-id="954d3-116">String</span></span> | <span data-ttu-id="954d3-117">Указывает правило группы допустимых возрастов, которое применяется к пользователям приложения.</span><span class="sxs-lookup"><span data-stu-id="954d3-117">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="954d3-118">Может иметь одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="954d3-118">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="954d3-119">Значение</span><span class="sxs-lookup"><span data-stu-id="954d3-119">Value</span></span></th><th><span data-ttu-id="954d3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="954d3-120">Description</span></span></th></tr><tr><td><span data-ttu-id="954d3-121">Разрешить</span><span class="sxs-lookup"><span data-stu-id="954d3-121">Allow</span></span></td><td><span data-ttu-id="954d3-122">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="954d3-122">Default.</span></span> <span data-ttu-id="954d3-123">Применяет юридическое минимальное значение.</span><span class="sxs-lookup"><span data-stu-id="954d3-123">Enforces the legal minimum.</span></span> <span data-ttu-id="954d3-124">Это означает, что для второстепенных стран Европейского союза и Корее требуются разрешения родителей.</span><span class="sxs-lookup"><span data-stu-id="954d3-124">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="954d3-125">рекуиреконсентфорпривацисервицес</span><span class="sxs-lookup"><span data-stu-id="954d3-125">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="954d3-126">Указывает, что пользователь должен указать дату рождения для обеспечения соответствия правилам Коппа.</span><span class="sxs-lookup"><span data-stu-id="954d3-126">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="954d3-127">рекуиреконсентформинорс</span><span class="sxs-lookup"><span data-stu-id="954d3-127">RequireConsentForMinors</span></span></td><td><span data-ttu-id="954d3-128">Для более ранних версий, независимо от правил для стран, требуется согласие пользователя в течение 18 лет.</span><span class="sxs-lookup"><span data-stu-id="954d3-128">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="954d3-129">рекуиреконсентфоркидс</span><span class="sxs-lookup"><span data-stu-id="954d3-129">RequireConsentForKids</span></span></td><td><span data-ttu-id="954d3-130">Для более ранних версий, независимо от правил для стран, требуется согласие на родителей в течение 14 лет.</span><span class="sxs-lookup"><span data-stu-id="954d3-130">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="954d3-131">блоккминорс</span><span class="sxs-lookup"><span data-stu-id="954d3-131">BlockMinors</span></span></td><td><span data-ttu-id="954d3-132">Блокирует небольшие из использования приложения.</span><span class="sxs-lookup"><span data-stu-id="954d3-132">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="954d3-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="954d3-133">JSON representation</span></span>
<span data-ttu-id="954d3-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="954d3-134">Here is a JSON representation of the resource.</span></span>

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
