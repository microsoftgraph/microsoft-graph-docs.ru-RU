---
title: Тип ресурса authenticationDetail
description: Предоставляет сведения о проверке подлинности для входного пользователя, такие как сведения о многофакторной проверке подлинности (MFA) и сведения о PTA/PHS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 134c3e502fa39fea626216315056adfeef5aef13
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720342"
---
# <a name="authenticationdetail-resource-type"></a><span data-ttu-id="2a779-103">Тип ресурса authenticationDetail</span><span class="sxs-lookup"><span data-stu-id="2a779-103">authenticationDetail resource type</span></span>

<span data-ttu-id="2a779-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a779-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a779-105">Предоставляет сведения о проверке подлинности для входного пользователя, такие как сведения о многофакторной проверке подлинности (MFA) и сведения о PTA/PHS.</span><span class="sxs-lookup"><span data-stu-id="2a779-105">Provides the authentication details for a user sign-in, such as multi-factor authentication (MFA) information and PTA/PHS details.</span></span>

## <a name="properties"></a><span data-ttu-id="2a779-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a779-106">Properties</span></span>

| <span data-ttu-id="2a779-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a779-107">Property</span></span>                       | <span data-ttu-id="2a779-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2a779-108">Type</span></span>           | <span data-ttu-id="2a779-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2a779-109">Description</span></span>                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2a779-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2a779-110">authenticationMethod</span></span>           | <span data-ttu-id="2a779-111">String</span><span class="sxs-lookup"><span data-stu-id="2a779-111">String</span></span>         | <span data-ttu-id="2a779-112">Тип метода проверки подлинности, используемого для выполнения этого шага проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2a779-112">The type of authentication method used to perform this step of authentication.</span></span> <span data-ttu-id="2a779-113">Возможные значения: `Password` , , , , `SMS` `Voice` `Authenticator App` `Software OATH token` `Satisfied by token` .</span><span class="sxs-lookup"><span data-stu-id="2a779-113">Possible values: `Password`, `SMS`, `Voice`, `Authenticator App`, `Software OATH token`, `Satisfied by token`.</span></span>                            |
| <span data-ttu-id="2a779-114">authenticationMethodDetail</span><span class="sxs-lookup"><span data-stu-id="2a779-114">authenticationMethodDetail</span></span>     | <span data-ttu-id="2a779-115">String</span><span class="sxs-lookup"><span data-stu-id="2a779-115">String</span></span>         | <span data-ttu-id="2a779-116">Сведения о методе проверки подлинности, используемом для выполнения этого шага проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2a779-116">Details about the authentication method used to perform this authentication step.</span></span> <span data-ttu-id="2a779-117">Например, номер телефона (для SMS и голосовой связи), имя устройства (для приложения Authenticator) и источник паролей (например, облако, AD FS, PTA, PHS).</span><span class="sxs-lookup"><span data-stu-id="2a779-117">For example, phone number (for SMS and voice), device name (for Authenticator app), and password source (e.g. cloud, AD FS, PTA, PHS).</span></span> |
| <span data-ttu-id="2a779-118">authenticationStepDateTime</span><span class="sxs-lookup"><span data-stu-id="2a779-118">authenticationStepDateTime</span></span>     | <span data-ttu-id="2a779-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a779-119">DateTimeOffset</span></span> | <span data-ttu-id="2a779-120">Представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="2a779-120">Represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2a779-121">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="2a779-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>                                           |
| <span data-ttu-id="2a779-122">authenticationStepRequirement</span><span class="sxs-lookup"><span data-stu-id="2a779-122">authenticationStepRequirement</span></span>  | <span data-ttu-id="2a779-123">String</span><span class="sxs-lookup"><span data-stu-id="2a779-123">String</span></span>         | <span data-ttu-id="2a779-124">Шаг проверки подлинности, который это удовлетворит.</span><span class="sxs-lookup"><span data-stu-id="2a779-124">The step of authentication that this satisfied.</span></span> <span data-ttu-id="2a779-125">Например, первичная проверка подлинности или многофакторная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="2a779-125">For example, primary authentication, or multi-factor authentication.</span></span>                                                                                                     |
| <span data-ttu-id="2a779-126">authenticationStepResultDetail</span><span class="sxs-lookup"><span data-stu-id="2a779-126">authenticationStepResultDetail</span></span> | <span data-ttu-id="2a779-127">String</span><span class="sxs-lookup"><span data-stu-id="2a779-127">String</span></span>         | <span data-ttu-id="2a779-128">Сведения о том, почему этот шаг был успешным или неудачным.</span><span class="sxs-lookup"><span data-stu-id="2a779-128">Details about why the step succeeded or failed.</span></span> <span data-ttu-id="2a779-129">Например, пользователь заблокирован, введен код мошенничества, нет ввода телефона - приурочиваемый, телефон недоступен, или утверждение в маркере.</span><span class="sxs-lookup"><span data-stu-id="2a779-129">For examples, user is blocked, fraud code entered, no phone input - timed out, phone unreachable, or claim in token.</span></span>                                                     |
| <span data-ttu-id="2a779-130">успешно</span><span class="sxs-lookup"><span data-stu-id="2a779-130">succeeded</span></span>                      | <span data-ttu-id="2a779-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a779-131">Boolean</span></span>        | <span data-ttu-id="2a779-132">Указывает состояние шага проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2a779-132">Indicates the status of the authentication step.</span></span> <span data-ttu-id="2a779-133">Возможные значения: `succeeded` , `failed` .</span><span class="sxs-lookup"><span data-stu-id="2a779-133">Possible values: `succeeded`, `failed`.</span></span>                                                                                                                                 |

## <a name="json-representation"></a><span data-ttu-id="2a779-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a779-134">JSON representation</span></span>

<span data-ttu-id="2a779-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a779-135">The following is a JSON representation of the resource.</span></span>

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

