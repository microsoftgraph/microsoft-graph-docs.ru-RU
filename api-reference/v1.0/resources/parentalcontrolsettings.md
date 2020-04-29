---
title: Тип ресурса Паренталконтролсеттингс
description: Указывает параметры родительского контроля для приложения. Эти параметры управляют согласия пользователя.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 8e54b8b437eb7a287102e67234a4f9b692136b79
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43353691"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="a715b-104">Тип ресурса Паренталконтролсеттингс</span><span class="sxs-lookup"><span data-stu-id="a715b-104">parentalControlSettings resource type</span></span>

<span data-ttu-id="a715b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a715b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a715b-106">Указывает параметры родительского контроля для приложения.</span><span class="sxs-lookup"><span data-stu-id="a715b-106">Specifies parental control settings for an application.</span></span> <span data-ttu-id="a715b-107">Эти параметры управляют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="a715b-107">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="a715b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a715b-108">Properties</span></span>

| <span data-ttu-id="a715b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a715b-109">Property</span></span> | <span data-ttu-id="a715b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a715b-110">Type</span></span> | <span data-ttu-id="a715b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a715b-111">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="a715b-112">каунтриесблоккедформинорс</span><span class="sxs-lookup"><span data-stu-id="a715b-112">countriesBlockedForMinors</span></span>|<span data-ttu-id="a715b-113">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a715b-113">String collection</span></span>| <span data-ttu-id="a715b-114">Задает [двузначные коды стран ISO](https://www.iso.org/iso-3166-country-codes.html).</span><span class="sxs-lookup"><span data-stu-id="a715b-114">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="a715b-115">Доступ к приложению будет заблокирован для небольших стран из стран, указанных в этом списке.</span><span class="sxs-lookup"><span data-stu-id="a715b-115">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="a715b-116">легалажеграупруле</span><span class="sxs-lookup"><span data-stu-id="a715b-116">legalAgeGroupRule</span></span>| <span data-ttu-id="a715b-117">String</span><span class="sxs-lookup"><span data-stu-id="a715b-117">String</span></span> | <span data-ttu-id="a715b-118">Указывает правило группы допустимых возрастов, которое применяется к пользователям приложения.</span><span class="sxs-lookup"><span data-stu-id="a715b-118">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="a715b-119">Может иметь одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="a715b-119">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="a715b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a715b-120">Value</span></span></th><th><span data-ttu-id="a715b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a715b-121">Description</span></span></th></tr><tr><td><span data-ttu-id="a715b-122">Разрешить</span><span class="sxs-lookup"><span data-stu-id="a715b-122">Allow</span></span></td><td><span data-ttu-id="a715b-123">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a715b-123">Default.</span></span> <span data-ttu-id="a715b-124">Применяет юридическое минимальное значение.</span><span class="sxs-lookup"><span data-stu-id="a715b-124">Enforces the legal minimum.</span></span> <span data-ttu-id="a715b-125">Это означает, что для второстепенных стран Европейского союза и Корее требуются разрешения родителей.</span><span class="sxs-lookup"><span data-stu-id="a715b-125">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="a715b-126">рекуиреконсентфорпривацисервицес</span><span class="sxs-lookup"><span data-stu-id="a715b-126">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="a715b-127">Указывает, что пользователь должен указать дату рождения для обеспечения соответствия правилам Коппа.</span><span class="sxs-lookup"><span data-stu-id="a715b-127">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="a715b-128">рекуиреконсентформинорс</span><span class="sxs-lookup"><span data-stu-id="a715b-128">RequireConsentForMinors</span></span></td><td><span data-ttu-id="a715b-129">Для более ранних версий, независимо от правил для стран, требуется согласие пользователя в течение 18 лет.</span><span class="sxs-lookup"><span data-stu-id="a715b-129">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="a715b-130">рекуиреконсентфоркидс</span><span class="sxs-lookup"><span data-stu-id="a715b-130">RequireConsentForKids</span></span></td><td><span data-ttu-id="a715b-131">Для более ранних версий, независимо от правил для стран, требуется согласие на родителей в течение 14 лет.</span><span class="sxs-lookup"><span data-stu-id="a715b-131">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="a715b-132">блоккминорс</span><span class="sxs-lookup"><span data-stu-id="a715b-132">BlockMinors</span></span></td><td><span data-ttu-id="a715b-133">Блокирует небольшие из использования приложения.</span><span class="sxs-lookup"><span data-stu-id="a715b-133">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="a715b-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a715b-134">JSON representation</span></span>
<span data-ttu-id="a715b-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a715b-135">Here is a JSON representation of the resource.</span></span>

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
