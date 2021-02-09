---
title: Тип ресурса relyingPartyDetailedSummary
description: Представляет в AD FS поднадзорную сторону.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a19132396f88797735801ee782c3c13e12a5e2ca
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161126"
---
# <a name="relyingpartydetailedsummary-resource-type"></a><span data-ttu-id="af895-103">Тип ресурса relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="af895-103">relyingPartyDetailedSummary resource type</span></span>

<span data-ttu-id="af895-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af895-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af895-105">Представляет поднадзорную сторону, настроенную со службами федерации Active Directory (AD FS), ее агрегированное использование и возможность переноса конфигурации с этой стороной в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="af895-105">Represents a relying party configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span>

## <a name="methods"></a><span data-ttu-id="af895-106">Методы</span><span class="sxs-lookup"><span data-stu-id="af895-106">Methods</span></span>

| <span data-ttu-id="af895-107">Метод</span><span class="sxs-lookup"><span data-stu-id="af895-107">Method</span></span>       | <span data-ttu-id="af895-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="af895-108">Return Type</span></span> | <span data-ttu-id="af895-109">Описание</span><span class="sxs-lookup"><span data-stu-id="af895-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="af895-110">Список</span><span class="sxs-lookup"><span data-stu-id="af895-110">List</span></span>](../api/relyingpartydetailedsummary-list.md) | [<span data-ttu-id="af895-111">relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="af895-111">relyingPartyDetailedSummary</span></span>](relyingpartydetailedsummary.md) | <span data-ttu-id="af895-112">Получить список объектов **relyingPartyDetailedSummary.**</span><span class="sxs-lookup"><span data-stu-id="af895-112">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span> |


## <a name="properties"></a><span data-ttu-id="af895-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="af895-113">Properties</span></span>

| <span data-ttu-id="af895-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="af895-114">Property</span></span>     | <span data-ttu-id="af895-115">Тип</span><span class="sxs-lookup"><span data-stu-id="af895-115">Type</span></span>        | <span data-ttu-id="af895-116">Описание</span><span class="sxs-lookup"><span data-stu-id="af895-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="af895-117">id</span><span class="sxs-lookup"><span data-stu-id="af895-117">id</span></span>|<span data-ttu-id="af895-118">String</span><span class="sxs-lookup"><span data-stu-id="af895-118">String</span></span>| <span data-ttu-id="af895-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="af895-119">Read-only.</span></span> <span data-ttu-id="af895-120">Уникальный идентификатор, созданный на уровне API.</span><span class="sxs-lookup"><span data-stu-id="af895-120">Unique Identifier generated at API level.</span></span>| 
|<span data-ttu-id="af895-121">relyingPartyId</span><span class="sxs-lookup"><span data-stu-id="af895-121">relyingPartyId</span></span>|<span data-ttu-id="af895-122">String</span><span class="sxs-lookup"><span data-stu-id="af895-122">String</span></span>|<span data-ttu-id="af895-123">Этот идентификатор используется для идентификации службящей стороны для этой службы федерации.</span><span class="sxs-lookup"><span data-stu-id="af895-123">This identifier is used to identify the relying party to this Federation Service.</span></span> <span data-ttu-id="af895-124">Он используется при выдаче утверждений в подавную сторону.</span><span class="sxs-lookup"><span data-stu-id="af895-124">It is used when issuing claims to the relying party.</span></span>|
|<span data-ttu-id="af895-125">serviceId</span><span class="sxs-lookup"><span data-stu-id="af895-125">serviceId</span></span>|<span data-ttu-id="af895-126">String</span><span class="sxs-lookup"><span data-stu-id="af895-126">String</span></span>|<span data-ttu-id="af895-127">Уникально идентифицирует лес Active Directory.</span><span class="sxs-lookup"><span data-stu-id="af895-127">Uniquely identifies the Active Directory forest.</span></span>|
|<span data-ttu-id="af895-128">migrationStatus</span><span class="sxs-lookup"><span data-stu-id="af895-128">migrationStatus</span></span>|<span data-ttu-id="af895-129">string</span><span class="sxs-lookup"><span data-stu-id="af895-129">string</span></span>| <span data-ttu-id="af895-130">Указывает, может ли приложение быть перемещено в Azure AD или требуется более подробное исследование.</span><span class="sxs-lookup"><span data-stu-id="af895-130">Indication of whether the application can be moved to Azure AD or require more investigation.</span></span> <span data-ttu-id="af895-131">Возможные значения: `ready`, `needsReview`, `additionalStepsRequired`.</span><span class="sxs-lookup"><span data-stu-id="af895-131">Possible values are: `ready`, `needsReview`, `additionalStepsRequired`.</span></span>|
|<span data-ttu-id="af895-132">migrationValidationDetails</span><span class="sxs-lookup"><span data-stu-id="af895-132">migrationValidationDetails</span></span>|<span data-ttu-id="af895-133">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="af895-133">[keyValuePair](keyvaluepair.md) collection</span></span>|<span data-ttu-id="af895-134">Указывает все проверки, которые необходимо проверить для сведений о конфигурации приложений, чтобы оценить, готово ли приложение к перемещению в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="af895-134">Specifies all the validations check done on applications configuration details to evaluate if the application is ready to be moved to Azure AD.</span></span> <span data-ttu-id="af895-135">Возможные имена: `AdditionalWSFedEndpointCheckResult` , , , , , , ,  `AllowedAuthenticationClassReferencesCheckResult` , `AlwaysRequireAuthenticationCheckResult` , , ,   `AutoUpdateEnabledCheckResult` `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult` ,  `EncryptedNameIdRequiredCheckResult` `MonitoringEnabledCheckResult` `NotBeforeSkewCheckResult`  `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult`  `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult` `IssuanceTransformRulesCheckResult` .</span><span class="sxs-lookup"><span data-stu-id="af895-135">Possible names are: `AdditionalWSFedEndpointCheckResult`,  `AllowedAuthenticationClassReferencesCheckResult`, `AlwaysRequireAuthenticationCheckResult`,   `AutoUpdateEnabledCheckResult`, `ClaimsProviderNameCheckResult`, `EncryptClaimsCheckResult`,  `EncryptedNameIdRequiredCheckResult`, `MonitoringEnabledCheckResult`,`NotBeforeSkewCheckResult`,  `RequestMFAFromClaimsProvidersCheckResult`, `SignedSamlRequestsRequiredCheckResult`, `AdditionalAuthenticationRulesCheckResult`, `TokenLifetimeCheckResult`,  `DelegationAuthorizationRulesCheckResult`, `IssuanceAuthorizationRulesCheckResult`, `IssuanceTransformRulesCheckResult`.</span></span> <span data-ttu-id="af895-136">Возможные значения результатов: `0` `1` , или `2` .</span><span class="sxs-lookup"><span data-stu-id="af895-136">Possible result values are `0`, `1`, or `2`.</span></span> <span data-ttu-id="af895-137">`0` когда проверка проверки пройдена, когда проверка не пройдена, и когда проверка проверки является `1` `2` предупреждением.</span><span class="sxs-lookup"><span data-stu-id="af895-137">`0` when the validation check passed, `1` when the validation check failed and `2` when the validation check is a warning.</span></span> |
|<span data-ttu-id="af895-138">relyingPartyName</span><span class="sxs-lookup"><span data-stu-id="af895-138">relyingPartyName</span></span>|<span data-ttu-id="af895-139">String</span><span class="sxs-lookup"><span data-stu-id="af895-139">String</span></span>|<span data-ttu-id="af895-140">Имя приложения или другой сущности в Интернете, использующей поставщика удостоверений для проверки подлинности пользователя, который хочет войти в систему.</span><span class="sxs-lookup"><span data-stu-id="af895-140">Name of application or other entity on the internet that uses an identity provider to authenticate a user who wants to log in.</span></span>|
|<span data-ttu-id="af895-141">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="af895-141">failedSignInCount</span></span>|<span data-ttu-id="af895-142">Int64</span><span class="sxs-lookup"><span data-stu-id="af895-142">Int64</span></span>| <span data-ttu-id="af895-143">Количество неудачных входов в службу федерации Active Directory за указанный период.</span><span class="sxs-lookup"><span data-stu-id="af895-143">Number of failed sign in on Active Directory Federation Service in the period specified.</span></span> |
|<span data-ttu-id="af895-144">replyUrls</span><span class="sxs-lookup"><span data-stu-id="af895-144">replyUrls</span></span>|<span data-ttu-id="af895-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="af895-145">String collection</span></span>|<span data-ttu-id="af895-146">Указывает, где ожидается получение маркера.</span><span class="sxs-lookup"><span data-stu-id="af895-146">Specifies where the relying party expects to receive the token.</span></span>|
|<span data-ttu-id="af895-147">signInSuccessRate</span><span class="sxs-lookup"><span data-stu-id="af895-147">signInSuccessRate</span></span>|<span data-ttu-id="af895-148">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="af895-148">Double</span></span>|<span data-ttu-id="af895-149">Количество успешных или успешных входов в службу федерации Active Directory (число успешных и неудачных входов) в указанном периоде.</span><span class="sxs-lookup"><span data-stu-id="af895-149">Number of successful / (number of successful + number of failed sign ins) on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="af895-150">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="af895-150">successfulSignInCount</span></span>|<span data-ttu-id="af895-151">Int64</span><span class="sxs-lookup"><span data-stu-id="af895-151">Int64</span></span>|<span data-ttu-id="af895-152">Количество успешных входов в службу федерации Active Directory.</span><span class="sxs-lookup"><span data-stu-id="af895-152">Number of successful sign ins on Active Directory Federation Service.</span></span>|
|<span data-ttu-id="af895-153">totalSignInCount</span><span class="sxs-lookup"><span data-stu-id="af895-153">totalSignInCount</span></span>|<span data-ttu-id="af895-154">Int64</span><span class="sxs-lookup"><span data-stu-id="af895-154">Int64</span></span>|<span data-ttu-id="af895-155">Количество успешных и неудачных входов в службу федерации Active Directory в указанный период.</span><span class="sxs-lookup"><span data-stu-id="af895-155">Number of successful + failed sign ins failed sign ins on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="af895-156">uniqueUserCount</span><span class="sxs-lookup"><span data-stu-id="af895-156">uniqueUserCount</span></span>|<span data-ttu-id="af895-157">Int64</span><span class="sxs-lookup"><span data-stu-id="af895-157">Int64</span></span>|<span data-ttu-id="af895-158">Количество уникальных пользователей, которые вписались в приложение.</span><span class="sxs-lookup"><span data-stu-id="af895-158">Number of unique users that have signed into the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af895-159">Связи</span><span class="sxs-lookup"><span data-stu-id="af895-159">Relationships</span></span>

<span data-ttu-id="af895-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="af895-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af895-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="af895-161">JSON representation</span></span>

<span data-ttu-id="af895-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af895-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary",
  "keyProperty": "id"
}-->

```json
{
  "failedSignInCount": 10,
  "id": "String (identifier)",
  "migrationStatus": "ready | needsReview | additionalStepsRequired",
  "migrationValidationDetails": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "relyingPartyId": "String",
  "relyingPartyName": "String",
  "replyUrls": ["String"],
  "serviceId": "String (identifier)",
  "signInSuccessRate": 90.0,
  "successfulSignInCount": 90,
  "totalSignInCount": 100,
  "uniqueUserCount": 10
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "relyingPartyDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


