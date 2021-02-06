---
title: Тип ресурса relyingPartyDetailedSummary
description: Представляет в AD FS поднадзорную сторону.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c1c0195302c4b01e39a6223797567c750807e9f6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136230"
---
# <a name="relyingpartydetailedsummary-resource-type"></a><span data-ttu-id="3a581-103">Тип ресурса relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="3a581-103">relyingPartyDetailedSummary resource type</span></span>

<span data-ttu-id="3a581-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a581-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a581-105">Представляет поднадзорную сторону, настроенную со службами федерации Active Directory (AD FS), ее агрегированное использование и возможность переноса конфигурации с этой стороной в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3a581-105">Represents a relying party configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span>

## <a name="methods"></a><span data-ttu-id="3a581-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3a581-106">Methods</span></span>

| <span data-ttu-id="3a581-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3a581-107">Method</span></span>       | <span data-ttu-id="3a581-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3a581-108">Return Type</span></span> | <span data-ttu-id="3a581-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3a581-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3a581-110">Список</span><span class="sxs-lookup"><span data-stu-id="3a581-110">List</span></span>](../api/relyingpartydetailedsummary-list.md) | [<span data-ttu-id="3a581-111">relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="3a581-111">relyingPartyDetailedSummary</span></span>](relyingpartydetailedsummary.md) | <span data-ttu-id="3a581-112">Получить список объектов **relyingPartyDetailedSummary.**</span><span class="sxs-lookup"><span data-stu-id="3a581-112">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span> |


## <a name="properties"></a><span data-ttu-id="3a581-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a581-113">Properties</span></span>

| <span data-ttu-id="3a581-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a581-114">Property</span></span>     | <span data-ttu-id="3a581-115">Тип</span><span class="sxs-lookup"><span data-stu-id="3a581-115">Type</span></span>        | <span data-ttu-id="3a581-116">Описание</span><span class="sxs-lookup"><span data-stu-id="3a581-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3a581-117">id</span><span class="sxs-lookup"><span data-stu-id="3a581-117">id</span></span>|<span data-ttu-id="3a581-118">String</span><span class="sxs-lookup"><span data-stu-id="3a581-118">String</span></span>| <span data-ttu-id="3a581-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3a581-119">Read-only.</span></span> <span data-ttu-id="3a581-120">Уникальный идентификатор, созданный на уровне API.</span><span class="sxs-lookup"><span data-stu-id="3a581-120">Unique Identifier generated at API level.</span></span>| 
|<span data-ttu-id="3a581-121">relyingPartyId</span><span class="sxs-lookup"><span data-stu-id="3a581-121">relyingPartyId</span></span>|<span data-ttu-id="3a581-122">Строка</span><span class="sxs-lookup"><span data-stu-id="3a581-122">String</span></span>|<span data-ttu-id="3a581-123">Этот идентификатор используется для идентификации службящей стороны для этой службы федерации.</span><span class="sxs-lookup"><span data-stu-id="3a581-123">This identifier is used to identify the relying party to this Federation Service.</span></span> <span data-ttu-id="3a581-124">Он используется при выдаче утверждений в подавную сторону.</span><span class="sxs-lookup"><span data-stu-id="3a581-124">It is used when issuing claims to the relying party.</span></span>|
|<span data-ttu-id="3a581-125">serviceId</span><span class="sxs-lookup"><span data-stu-id="3a581-125">serviceId</span></span>|<span data-ttu-id="3a581-126">Строка</span><span class="sxs-lookup"><span data-stu-id="3a581-126">String</span></span>|<span data-ttu-id="3a581-127">Уникально идентифицирует лес Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3a581-127">Uniquely identifies the Active Directory forest.</span></span>|
|<span data-ttu-id="3a581-128">migrationStatus</span><span class="sxs-lookup"><span data-stu-id="3a581-128">migrationStatus</span></span>|<span data-ttu-id="3a581-129">string</span><span class="sxs-lookup"><span data-stu-id="3a581-129">string</span></span>| <span data-ttu-id="3a581-130">Указывает, может ли приложение быть перемещено в Azure AD или требуется более подробное исследование.</span><span class="sxs-lookup"><span data-stu-id="3a581-130">Indication of whether the application can be moved to Azure AD or require more investigation.</span></span> <span data-ttu-id="3a581-131">Возможные значения: `ready`, `needsReview`, `additionalStepsRequired`.</span><span class="sxs-lookup"><span data-stu-id="3a581-131">Possible values are: `ready`, `needsReview`, `additionalStepsRequired`.</span></span>|
|<span data-ttu-id="3a581-132">migrationValidationDetails</span><span class="sxs-lookup"><span data-stu-id="3a581-132">migrationValidationDetails</span></span>|<span data-ttu-id="3a581-133">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3a581-133">[keyValuePair](keyvaluepair.md) collection</span></span>|<span data-ttu-id="3a581-134">Указывает все проверки, которые необходимо проверить для сведений о конфигурации приложений, чтобы оценить, готово ли приложение к перемещению в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3a581-134">Specifies all the validations check done on applications configuration details to evaluate if the application is ready to be moved to Azure AD.</span></span> <span data-ttu-id="3a581-135">Возможные имена: `AdditionalWSFedEndpointCheckResult` , , , , , , ,  `AllowedAuthenticationClassReferencesCheckResult` , `AlwaysRequireAuthenticationCheckResult` , , , ,   `AutoUpdateEnabledCheckResult` `ClaimsProviderNameCheckResult` , `EncryptClaimsCheckResult`  `EncryptedNameIdRequiredCheckResult` `MonitoringEnabledCheckResult` `NotBeforeSkewCheckResult`  `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult`  `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult` `IssuanceTransformRulesCheckResult` .</span><span class="sxs-lookup"><span data-stu-id="3a581-135">Possible names are: `AdditionalWSFedEndpointCheckResult`,  `AllowedAuthenticationClassReferencesCheckResult`, `AlwaysRequireAuthenticationCheckResult`,   `AutoUpdateEnabledCheckResult`, `ClaimsProviderNameCheckResult`, `EncryptClaimsCheckResult`,  `EncryptedNameIdRequiredCheckResult`, `MonitoringEnabledCheckResult`,`NotBeforeSkewCheckResult`,  `RequestMFAFromClaimsProvidersCheckResult`, `SignedSamlRequestsRequiredCheckResult`, `AdditionalAuthenticationRulesCheckResult`, `TokenLifetimeCheckResult`,  `DelegationAuthorizationRulesCheckResult`, `IssuanceAuthorizationRulesCheckResult`, `IssuanceTransformRulesCheckResult`.</span></span> <span data-ttu-id="3a581-136">Возможные значения результатов: `0` `1` , или `2` .</span><span class="sxs-lookup"><span data-stu-id="3a581-136">Possible result values are `0`, `1`, or `2`.</span></span> <span data-ttu-id="3a581-137">`0` когда проверка проверки пройдена, когда проверка не пройдена, и когда проверка проверки является `1` `2` предупреждением.</span><span class="sxs-lookup"><span data-stu-id="3a581-137">`0` when the validation check passed, `1` when the validation check failed and `2` when the validation check is a warning.</span></span> |
|<span data-ttu-id="3a581-138">relyingPartyName</span><span class="sxs-lookup"><span data-stu-id="3a581-138">relyingPartyName</span></span>|<span data-ttu-id="3a581-139">Строка</span><span class="sxs-lookup"><span data-stu-id="3a581-139">String</span></span>|<span data-ttu-id="3a581-140">Имя приложения или другой сущности в Интернете, использующей поставщика удостоверений для проверки подлинности пользователя, который хочет войти в систему.</span><span class="sxs-lookup"><span data-stu-id="3a581-140">Name of application or other entity on the internet that uses an identity provider to authenticate a user who wants to log in.</span></span>|
|<span data-ttu-id="3a581-141">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="3a581-141">failedSignInCount</span></span>|<span data-ttu-id="3a581-142">Int64</span><span class="sxs-lookup"><span data-stu-id="3a581-142">Int64</span></span>| <span data-ttu-id="3a581-143">Количество неудачных входов в службу федерации Active Directory за указанный период.</span><span class="sxs-lookup"><span data-stu-id="3a581-143">Number of failed sign in on Active Directory Federation Service in the period specified.</span></span> |
|<span data-ttu-id="3a581-144">replyUrls</span><span class="sxs-lookup"><span data-stu-id="3a581-144">replyUrls</span></span>|<span data-ttu-id="3a581-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3a581-145">String collection</span></span>|<span data-ttu-id="3a581-146">Указывает, где ожидается получение маркера.</span><span class="sxs-lookup"><span data-stu-id="3a581-146">Specifies where the relying party expects to receive the token.</span></span>|
|<span data-ttu-id="3a581-147">signInSuccessRate</span><span class="sxs-lookup"><span data-stu-id="3a581-147">signInSuccessRate</span></span>|<span data-ttu-id="3a581-148">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="3a581-148">Double</span></span>|<span data-ttu-id="3a581-149">Количество успешных или успешных входов в службу федерации Active Directory (число успешных и неудачных входов) в указанном периоде.</span><span class="sxs-lookup"><span data-stu-id="3a581-149">Number of successful / (number of successful + number of failed sign ins) on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="3a581-150">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="3a581-150">successfulSignInCount</span></span>|<span data-ttu-id="3a581-151">Int64</span><span class="sxs-lookup"><span data-stu-id="3a581-151">Int64</span></span>|<span data-ttu-id="3a581-152">Количество успешных входов в службу федерации Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3a581-152">Number of successful sign ins on Active Directory Federation Service.</span></span>|
|<span data-ttu-id="3a581-153">totalSignInCount</span><span class="sxs-lookup"><span data-stu-id="3a581-153">totalSignInCount</span></span>|<span data-ttu-id="3a581-154">Int64</span><span class="sxs-lookup"><span data-stu-id="3a581-154">Int64</span></span>|<span data-ttu-id="3a581-155">Количество успешных и неудачных входов в службу федерации Active Directory в указанный период.</span><span class="sxs-lookup"><span data-stu-id="3a581-155">Number of successful + failed sign ins failed sign ins on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="3a581-156">uniqueUserCount</span><span class="sxs-lookup"><span data-stu-id="3a581-156">uniqueUserCount</span></span>|<span data-ttu-id="3a581-157">Int64</span><span class="sxs-lookup"><span data-stu-id="3a581-157">Int64</span></span>|<span data-ttu-id="3a581-158">Количество уникальных пользователей, которые вписались в приложение.</span><span class="sxs-lookup"><span data-stu-id="3a581-158">Number of unique users that have signed into the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a581-159">Связи</span><span class="sxs-lookup"><span data-stu-id="3a581-159">Relationships</span></span>

<span data-ttu-id="3a581-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3a581-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a581-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3a581-161">JSON representation</span></span>

<span data-ttu-id="3a581-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a581-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary",
  "baseType": "",
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


