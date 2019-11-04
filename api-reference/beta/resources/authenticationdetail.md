---
title: Тип ресурса Аусентикатиондетаил
description: Предоставляет сведения о проверке подлинности для входа пользователя, например сведения о многофакторной проверке подлинности (MFA) и сведения о ПТА/ФС.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 715685ee485b538d6be3dd45cb87949483324382
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939399"
---
# <a name="authenticationdetail-resource-type"></a><span data-ttu-id="da360-103">Тип ресурса Аусентикатиондетаил</span><span class="sxs-lookup"><span data-stu-id="da360-103">authenticationDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da360-104">Предоставляет сведения о проверке подлинности для входа пользователя, например сведения о многофакторной проверке подлинности (MFA) и сведения о ПТА/ФС.</span><span class="sxs-lookup"><span data-stu-id="da360-104">Provides the authentication details for a user sign-in, such as multi-factor authentication (MFA) information and PTA/PHS details.</span></span>

## <a name="properties"></a><span data-ttu-id="da360-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="da360-105">Properties</span></span>

| <span data-ttu-id="da360-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="da360-106">Property</span></span>     | <span data-ttu-id="da360-107">Тип</span><span class="sxs-lookup"><span data-stu-id="da360-107">Type</span></span>        | <span data-ttu-id="da360-108">Описание</span><span class="sxs-lookup"><span data-stu-id="da360-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da360-109">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="da360-109">authenticationMethod</span></span>|<span data-ttu-id="da360-110">Строка</span><span class="sxs-lookup"><span data-stu-id="da360-110">String</span></span>||<span data-ttu-id="da360-111">Тип метода проверки подлинности, используемый для выполнения этого этапа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="da360-111">The type of authentication method used to perform this step of authentication.</span></span> <span data-ttu-id="da360-112">Возможные значения: `Password`, `SMS`, `Voice`,` Authenticator App`, `Software OATH token`, `Satisfied by token`.</span><span class="sxs-lookup"><span data-stu-id="da360-112">Possible values: `Password`, `SMS`, `Voice`,` Authenticator App`, `Software OATH token`, `Satisfied by token`.</span></span>|
|<span data-ttu-id="da360-113">аусентикатионмесоддетаил</span><span class="sxs-lookup"><span data-stu-id="da360-113">authenticationMethodDetail</span></span>|<span data-ttu-id="da360-114">Строка</span><span class="sxs-lookup"><span data-stu-id="da360-114">String</span></span>|<span data-ttu-id="da360-115">Сведения о методе проверки подлинности, используемом для выполнения этой процедуры проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="da360-115">Details about the authentication method used to perform this authentication step.</span></span> <span data-ttu-id="da360-116">Например, номер телефона (для SMS и голосовой связи), имя устройства (для приложения проверки подлинности) и источник пароля (Cloud, AD FS, ПТА, ФС).</span><span class="sxs-lookup"><span data-stu-id="da360-116">For example, phone number (for SMS and voice), device name (for Authenticator app), and password source (e.g. cloud, AD FS, PTA, PHS).</span></span> |
|<span data-ttu-id="da360-117">аусентикатионстепдатетиме</span><span class="sxs-lookup"><span data-stu-id="da360-117">authenticationStepDateTime</span></span>|<span data-ttu-id="da360-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da360-118">DateTimeOffset</span></span>|<span data-ttu-id="da360-119">Представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="da360-119">Represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="da360-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="da360-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="da360-121">аусентикатионстепрекуиремент</span><span class="sxs-lookup"><span data-stu-id="da360-121">authenticationStepRequirement</span></span>|<span data-ttu-id="da360-122">Строка</span><span class="sxs-lookup"><span data-stu-id="da360-122">String</span></span>|<span data-ttu-id="da360-123">Шаг проверки подлинности, который удовлетворен.</span><span class="sxs-lookup"><span data-stu-id="da360-123">The step of authentication that this satisfied.</span></span> <span data-ttu-id="da360-124">Например, Первичная проверка подлинности или многофакторная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="da360-124">For example, primary authentication, or multi-factor authentication.</span></span>|
|<span data-ttu-id="da360-125">аусентикатионстепресултдетаил</span><span class="sxs-lookup"><span data-stu-id="da360-125">authenticationStepResultDetail</span></span>|<span data-ttu-id="da360-126">Строка</span><span class="sxs-lookup"><span data-stu-id="da360-126">String</span></span>|<span data-ttu-id="da360-127">Сведения о причине успешного или неудачного завершения этапа.</span><span class="sxs-lookup"><span data-stu-id="da360-127">Details about why the step succeeded or failed.</span></span> <span data-ttu-id="da360-128">Например, пользователь блокируется, заменяется мошеннический код, не используется ввод с истекшим сроком ожидания, Телефон недоступен или утвержден в маркере.</span><span class="sxs-lookup"><span data-stu-id="da360-128">For examples, user is blocked, fraud code entered, no phone input - timed out, phone unreachable, or claim in token.</span></span>|
|<span data-ttu-id="da360-129">закончил</span><span class="sxs-lookup"><span data-stu-id="da360-129">succeeded</span></span>|<span data-ttu-id="da360-130">Логический</span><span class="sxs-lookup"><span data-stu-id="da360-130">Boolean</span></span>|<span data-ttu-id="da360-131">Указывает состояние этапа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="da360-131">Indicates the status of the authentication step.</span></span>|<span data-ttu-id="da360-132">Возможные значения: `succeeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="da360-132">Possible values: `succeeded`, `failed`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da360-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da360-133">JSON representation</span></span>

<span data-ttu-id="da360-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da360-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationDetail",
  "baseType": null
}-->

```json
{
  "authenticationMethod": "String",
  "authenticationMethodDetail": "String",
  "authenticationStepDateTime": "String (timestamp)",
  "authenticationStepRequirement": "String",
  "authenticationStepResultDetail": "String",
  "succeeded": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->