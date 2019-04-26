---
title: Тип ресурса Паренталконтролсеттингс
description: Указывает параметры родительского контроля для приложения. Эти параметры управляют согласия пользователя.
localization_priority: Normal
ms.openlocfilehash: 52a808cd4c3e6f29e4d43c7c4ea5c9e30a81447b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568670"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="1daca-104">Тип ресурса Паренталконтролсеттингс</span><span class="sxs-lookup"><span data-stu-id="1daca-104">parentalControlSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1daca-105">Указывает параметры родительского контроля для приложения.</span><span class="sxs-lookup"><span data-stu-id="1daca-105">Specifies parental control settings for an application.</span></span> <span data-ttu-id="1daca-106">Эти параметры управляют согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="1daca-106">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="1daca-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1daca-107">Properties</span></span>

| <span data-ttu-id="1daca-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1daca-108">Property</span></span> | <span data-ttu-id="1daca-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1daca-109">Type</span></span> | <span data-ttu-id="1daca-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1daca-110">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="1daca-111">Каунтриесблоккедформинорс</span><span class="sxs-lookup"><span data-stu-id="1daca-111">countriesBlockedForMinors</span></span>|<span data-ttu-id="1daca-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1daca-112">String collection</span></span>| <span data-ttu-id="1daca-113">Задает [двузначные коды стран ISO](https://www.iso.org/iso-3166-country-codes.html).</span><span class="sxs-lookup"><span data-stu-id="1daca-113">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="1daca-114">Доступ к приложению будет заблокирован для небольших стран из стран, указанных в этом списке.</span><span class="sxs-lookup"><span data-stu-id="1daca-114">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="1daca-115">Легалажеграупруле</span><span class="sxs-lookup"><span data-stu-id="1daca-115">legalAgeGroupRule</span></span>| <span data-ttu-id="1daca-116">String</span><span class="sxs-lookup"><span data-stu-id="1daca-116">String</span></span> | <span data-ttu-id="1daca-117">Указывает правило группы допустимых возрастов, которое применяется к пользователям приложения.</span><span class="sxs-lookup"><span data-stu-id="1daca-117">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="1daca-118">Может иметь одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="1daca-118">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="1daca-119">Значение</span><span class="sxs-lookup"><span data-stu-id="1daca-119">Value</span></span></th><th><span data-ttu-id="1daca-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1daca-120">Description</span></span></th></tr><tr><td><span data-ttu-id="1daca-121">Разрешить</span><span class="sxs-lookup"><span data-stu-id="1daca-121">Allow</span></span></td><td><span data-ttu-id="1daca-122">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1daca-122">Default.</span></span> <span data-ttu-id="1daca-123">ПриМеняет юридическое минимальное значение.</span><span class="sxs-lookup"><span data-stu-id="1daca-123">Enforces the legal minimum.</span></span> <span data-ttu-id="1daca-124">Это означает, что для второстепенных стран Европейского союза и Корее требуются разрешения родителей.</span><span class="sxs-lookup"><span data-stu-id="1daca-124">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="1daca-125">Рекуиреконсентфорпривацисервицес</span><span class="sxs-lookup"><span data-stu-id="1daca-125">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="1daca-126">Указывает, что пользователь должен указать дату рождения для обеспечения соответствия правилам Коппа.</span><span class="sxs-lookup"><span data-stu-id="1daca-126">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="1daca-127">Рекуиреконсентформинорс</span><span class="sxs-lookup"><span data-stu-id="1daca-127">RequireConsentForMinors</span></span></td><td><span data-ttu-id="1daca-128">Для более ранних версий, независимо от правил для стран, требуется согласие пользователя в течение 18 лет.</span><span class="sxs-lookup"><span data-stu-id="1daca-128">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="1daca-129">Рекуиреконсентфоркидс</span><span class="sxs-lookup"><span data-stu-id="1daca-129">RequireConsentForKids</span></span></td><td><span data-ttu-id="1daca-130">Для более ранних версий, независимо от правил для стран, требуется согласие на родителей в течение 14 лет.</span><span class="sxs-lookup"><span data-stu-id="1daca-130">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="1daca-131">Блоккминорс</span><span class="sxs-lookup"><span data-stu-id="1daca-131">BlockMinors</span></span></td><td><span data-ttu-id="1daca-132">Блокирует небольшие из использования приложения.</span><span class="sxs-lookup"><span data-stu-id="1daca-132">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="1daca-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1daca-133">JSON representation</span></span>
<span data-ttu-id="1daca-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1daca-134">Here is a JSON representation of the resource.</span></span>

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
