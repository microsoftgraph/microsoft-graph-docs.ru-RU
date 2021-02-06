---
title: Тип ресурса parentalControlSettings
description: Указывает параметры родительского контроля для приложения. Эти параметры контролируют условия получения согласия.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f63f81af9e35183a15ab07b1f8e8fce9e8488bae
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136005"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="7ebfc-104">Тип ресурса parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="7ebfc-104">parentalControlSettings resource type</span></span>

<span data-ttu-id="7ebfc-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ebfc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ebfc-106">Указывает параметры родительского контроля для приложения.</span><span class="sxs-lookup"><span data-stu-id="7ebfc-106">Specifies parental control settings for an application.</span></span> <span data-ttu-id="7ebfc-107">Эти параметры контролируют условия получения согласия.</span><span class="sxs-lookup"><span data-stu-id="7ebfc-107">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="7ebfc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ebfc-108">Properties</span></span>

| <span data-ttu-id="7ebfc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ebfc-109">Property</span></span> | <span data-ttu-id="7ebfc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7ebfc-110">Type</span></span> | <span data-ttu-id="7ebfc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7ebfc-111">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="7ebfc-112">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="7ebfc-112">countriesBlockedForMinors</span></span>|<span data-ttu-id="7ebfc-113">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="7ebfc-113">String collection</span></span>| <span data-ttu-id="7ebfc-114">Указывает [коды стран ISO](https://www.iso.org/iso-3166-country-codes.html)из двух букв.</span><span class="sxs-lookup"><span data-stu-id="7ebfc-114">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="7ebfc-115">Доступ к приложению будет заблокирован для несовершеннолетних из стран, указанных в этом списке.</span><span class="sxs-lookup"><span data-stu-id="7ebfc-115">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="7ebfc-116">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="7ebfc-116">legalAgeGroupRule</span></span>| <span data-ttu-id="7ebfc-117">Строка</span><span class="sxs-lookup"><span data-stu-id="7ebfc-117">String</span></span> | <span data-ttu-id="7ebfc-118">Указывает правило юридической возрастной группы, которое применяется к пользователям приложения.</span><span class="sxs-lookup"><span data-stu-id="7ebfc-118">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="7ebfc-119">Может иметь одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="7ebfc-119">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="7ebfc-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7ebfc-120">Value</span></span></th><th><span data-ttu-id="7ebfc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7ebfc-121">Description</span></span></th></tr><tr><td><span data-ttu-id="7ebfc-122">Разрешить</span><span class="sxs-lookup"><span data-stu-id="7ebfc-122">Allow</span></span></td><td><span data-ttu-id="7ebfc-123">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7ebfc-123">Default.</span></span> <span data-ttu-id="7ebfc-124">Принудительно применяет минимальный юридический уровень.</span><span class="sxs-lookup"><span data-stu-id="7ebfc-124">Enforces the legal minimum.</span></span> <span data-ttu-id="7ebfc-125">Это означает, что для несовершеннолетних в Европейском Союзе и Республике Корея требуется родительское согласие.</span><span class="sxs-lookup"><span data-stu-id="7ebfc-125">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="7ebfc-126">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="7ebfc-126">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="7ebfc-127">Принудительно применяет пользователя к указанию даты рождения в соответствии с правилами COPPA.</span><span class="sxs-lookup"><span data-stu-id="7ebfc-127">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="7ebfc-128">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="7ebfc-128">RequireConsentForMinors</span></span></td><td><span data-ttu-id="7ebfc-129">Требуется родительское согласие для детей не ниже 18 лет, независимо от правил для несовершеннолетних в стране.</span><span class="sxs-lookup"><span data-stu-id="7ebfc-129">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="7ebfc-130">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="7ebfc-130">RequireConsentForKids</span></span></td><td><span data-ttu-id="7ebfc-131">Требуется родительское согласие для детей до 14 лет, независимо от правил для несовершеннолетних в стране.</span><span class="sxs-lookup"><span data-stu-id="7ebfc-131">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="7ebfc-132">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="7ebfc-132">BlockMinors</span></span></td><td><span data-ttu-id="7ebfc-133">Блокирует использование приложения несовершеннолетних.</span><span class="sxs-lookup"><span data-stu-id="7ebfc-133">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="7ebfc-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7ebfc-134">JSON representation</span></span>
<span data-ttu-id="7ebfc-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ebfc-135">Here is a JSON representation of the resource.</span></span>

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


