---
title: Тип ресурса parentalControlSettings
description: Указывает параметры родительского контроля для приложения. Эти параметры контролируют условия получения согласия.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 1f145ecabb4eccfe15eaedc856b1349fc6ce9f5a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128500"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="eb84f-104">Тип ресурса parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="eb84f-104">parentalControlSettings resource type</span></span>

<span data-ttu-id="eb84f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb84f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb84f-106">Указывает параметры родительского контроля для приложения.</span><span class="sxs-lookup"><span data-stu-id="eb84f-106">Specifies parental control settings for an application.</span></span> <span data-ttu-id="eb84f-107">Эти параметры контролируют условия получения согласия.</span><span class="sxs-lookup"><span data-stu-id="eb84f-107">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="eb84f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb84f-108">Properties</span></span>

| <span data-ttu-id="eb84f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb84f-109">Property</span></span> | <span data-ttu-id="eb84f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eb84f-110">Type</span></span> | <span data-ttu-id="eb84f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eb84f-111">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="eb84f-112">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="eb84f-112">countriesBlockedForMinors</span></span>|<span data-ttu-id="eb84f-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="eb84f-113">String collection</span></span>| <span data-ttu-id="eb84f-114">Указывает двух [буквы кодов стран ISO.](https://www.iso.org/iso-3166-country-codes.html)</span><span class="sxs-lookup"><span data-stu-id="eb84f-114">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="eb84f-115">Доступ к приложению будет заблокирован для несовершеннолетних из стран, указанных в этом списке.</span><span class="sxs-lookup"><span data-stu-id="eb84f-115">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="eb84f-116">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="eb84f-116">legalAgeGroupRule</span></span>| <span data-ttu-id="eb84f-117">String</span><span class="sxs-lookup"><span data-stu-id="eb84f-117">String</span></span> | <span data-ttu-id="eb84f-118">Указывает правило юридической возрастной группы, которое применяется к пользователям приложения.</span><span class="sxs-lookup"><span data-stu-id="eb84f-118">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="eb84f-119">Может иметь одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="eb84f-119">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="eb84f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="eb84f-120">Value</span></span></th><th><span data-ttu-id="eb84f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="eb84f-121">Description</span></span></th></tr><tr><td><span data-ttu-id="eb84f-122">Разрешить</span><span class="sxs-lookup"><span data-stu-id="eb84f-122">Allow</span></span></td><td><span data-ttu-id="eb84f-123">Значение, используемое по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="eb84f-123">Default.</span></span> <span data-ttu-id="eb84f-124">Принудительно применяет минимальный юридический уровень.</span><span class="sxs-lookup"><span data-stu-id="eb84f-124">Enforces the legal minimum.</span></span> <span data-ttu-id="eb84f-125">Это означает, что для несовершеннолетних в Европейском Союзе и Корее требуется родительское согласие.</span><span class="sxs-lookup"><span data-stu-id="eb84f-125">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="eb84f-126">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="eb84f-126">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="eb84f-127">Принудительно применяет пользователя к указанию даты рождения в соответствии с правилами COPPA.</span><span class="sxs-lookup"><span data-stu-id="eb84f-127">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="eb84f-128">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="eb84f-128">RequireConsentForMinors</span></span></td><td><span data-ttu-id="eb84f-129">Требуется родительское согласие возрастом до 18 лет, независимо от правил для несовершеннолетних в стране.</span><span class="sxs-lookup"><span data-stu-id="eb84f-129">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="eb84f-130">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="eb84f-130">RequireConsentForKids</span></span></td><td><span data-ttu-id="eb84f-131">Требуется родительское согласие для детей до 14 лет, независимо от правил для несовершеннолетних в стране.</span><span class="sxs-lookup"><span data-stu-id="eb84f-131">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="eb84f-132">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="eb84f-132">BlockMinors</span></span></td><td><span data-ttu-id="eb84f-133">Блокирует использование приложения несовершеннолетних.</span><span class="sxs-lookup"><span data-stu-id="eb84f-133">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="eb84f-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb84f-134">JSON representation</span></span>
<span data-ttu-id="eb84f-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb84f-135">Here is a JSON representation of the resource.</span></span>

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

