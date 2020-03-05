---
title: Тип ресурса Аусентикатиондетаил
description: Предоставляет сведения о проверке подлинности для входа пользователя, например сведения о многофакторной проверке подлинности (MFA) и сведения о ПТА/ФС.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 97375635d86b1be8149035c94d183026a3d49a25
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508089"
---
# <a name="authenticationdetail-resource-type"></a><span data-ttu-id="6c627-103">Тип ресурса Аусентикатиондетаил</span><span class="sxs-lookup"><span data-stu-id="6c627-103">authenticationDetail resource type</span></span>

<span data-ttu-id="6c627-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6c627-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c627-105">Предоставляет сведения о проверке подлинности для входа пользователя, например сведения о многофакторной проверке подлинности (MFA) и сведения о ПТА/ФС.</span><span class="sxs-lookup"><span data-stu-id="6c627-105">Provides the authentication details for a user sign-in, such as multi-factor authentication (MFA) information and PTA/PHS details.</span></span>

## <a name="properties"></a><span data-ttu-id="6c627-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c627-106">Properties</span></span>

| <span data-ttu-id="6c627-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c627-107">Property</span></span>     | <span data-ttu-id="6c627-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6c627-108">Type</span></span>        | <span data-ttu-id="6c627-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6c627-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6c627-110">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="6c627-110">authenticationMethod</span></span>|<span data-ttu-id="6c627-111">String</span><span class="sxs-lookup"><span data-stu-id="6c627-111">String</span></span>||<span data-ttu-id="6c627-112">Тип метода проверки подлинности, используемый для выполнения этого этапа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6c627-112">The type of authentication method used to perform this step of authentication.</span></span> <span data-ttu-id="6c627-113">Возможные значения: `Password`, `SMS`, `Voice`,` Authenticator App`, `Software OATH token`, `Satisfied by token`.</span><span class="sxs-lookup"><span data-stu-id="6c627-113">Possible values: `Password`, `SMS`, `Voice`,` Authenticator App`, `Software OATH token`, `Satisfied by token`.</span></span>|
|<span data-ttu-id="6c627-114">аусентикатионмесоддетаил</span><span class="sxs-lookup"><span data-stu-id="6c627-114">authenticationMethodDetail</span></span>|<span data-ttu-id="6c627-115">String</span><span class="sxs-lookup"><span data-stu-id="6c627-115">String</span></span>|<span data-ttu-id="6c627-116">Сведения о методе проверки подлинности, используемом для выполнения этой процедуры проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6c627-116">Details about the authentication method used to perform this authentication step.</span></span> <span data-ttu-id="6c627-117">Например, номер телефона (для SMS и голосовой связи), имя устройства (для приложения проверки подлинности) и источник пароля (Cloud, AD FS, ПТА, ФС).</span><span class="sxs-lookup"><span data-stu-id="6c627-117">For example, phone number (for SMS and voice), device name (for Authenticator app), and password source (e.g. cloud, AD FS, PTA, PHS).</span></span> |
|<span data-ttu-id="6c627-118">аусентикатионстепдатетиме</span><span class="sxs-lookup"><span data-stu-id="6c627-118">authenticationStepDateTime</span></span>|<span data-ttu-id="6c627-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c627-119">DateTimeOffset</span></span>|<span data-ttu-id="6c627-120">Представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6c627-120">Represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6c627-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6c627-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="6c627-122">аусентикатионстепрекуиремент</span><span class="sxs-lookup"><span data-stu-id="6c627-122">authenticationStepRequirement</span></span>|<span data-ttu-id="6c627-123">String</span><span class="sxs-lookup"><span data-stu-id="6c627-123">String</span></span>|<span data-ttu-id="6c627-124">Шаг проверки подлинности, который удовлетворен.</span><span class="sxs-lookup"><span data-stu-id="6c627-124">The step of authentication that this satisfied.</span></span> <span data-ttu-id="6c627-125">Например, Первичная проверка подлинности или многофакторная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="6c627-125">For example, primary authentication, or multi-factor authentication.</span></span>|
|<span data-ttu-id="6c627-126">аусентикатионстепресултдетаил</span><span class="sxs-lookup"><span data-stu-id="6c627-126">authenticationStepResultDetail</span></span>|<span data-ttu-id="6c627-127">String</span><span class="sxs-lookup"><span data-stu-id="6c627-127">String</span></span>|<span data-ttu-id="6c627-128">Сведения о причине успешного или неудачного завершения этапа.</span><span class="sxs-lookup"><span data-stu-id="6c627-128">Details about why the step succeeded or failed.</span></span> <span data-ttu-id="6c627-129">Например, пользователь блокируется, заменяется мошеннический код, не используется ввод с истекшим сроком ожидания, Телефон недоступен или утвержден в маркере.</span><span class="sxs-lookup"><span data-stu-id="6c627-129">For examples, user is blocked, fraud code entered, no phone input - timed out, phone unreachable, or claim in token.</span></span>|
|<span data-ttu-id="6c627-130">закончил</span><span class="sxs-lookup"><span data-stu-id="6c627-130">succeeded</span></span>|<span data-ttu-id="6c627-131">Логический</span><span class="sxs-lookup"><span data-stu-id="6c627-131">Boolean</span></span>|<span data-ttu-id="6c627-132">Указывает состояние этапа проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6c627-132">Indicates the status of the authentication step.</span></span>|<span data-ttu-id="6c627-133">Возможные значения: `succeeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="6c627-133">Possible values: `succeeded`, `failed`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c627-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c627-134">JSON representation</span></span>

<span data-ttu-id="6c627-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c627-135">The following is a JSON representation of the resource.</span></span>

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