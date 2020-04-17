---
title: Тип ресурса Релингпартидетаиледсуммари
description: Представляет проверяющую сторону в AD FS.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 306c20c31120d2f130562993d8ebd2d7e4083c23
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543481"
---
# <a name="relyingpartydetailedsummary-resource-type"></a><span data-ttu-id="f34c3-103">Тип ресурса Релингпартидетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="f34c3-103">relyingPartyDetailedSummary resource type</span></span>

<span data-ttu-id="f34c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f34c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f34c3-105">Представляет проверяющую сторону, настроенную с помощью служб федерации Active Directory (AD FS), его агрегированное использование и возможность переноса конфигурации проверяющей стороны в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f34c3-105">Represents a relying party configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span>

## <a name="methods"></a><span data-ttu-id="f34c3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f34c3-106">Methods</span></span>

| <span data-ttu-id="f34c3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f34c3-107">Method</span></span>       | <span data-ttu-id="f34c3-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f34c3-108">Return Type</span></span> | <span data-ttu-id="f34c3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f34c3-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f34c3-110">List</span><span class="sxs-lookup"><span data-stu-id="f34c3-110">List</span></span>](../api/relyingpartydetailedsummary-list.md) | [<span data-ttu-id="f34c3-111">релингпартидетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="f34c3-111">relyingPartyDetailedSummary</span></span>](relyingpartydetailedsummary.md) | <span data-ttu-id="f34c3-112">Получение списка объектов **релингпартидетаиледсуммари** .</span><span class="sxs-lookup"><span data-stu-id="f34c3-112">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span> |


## <a name="properties"></a><span data-ttu-id="f34c3-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="f34c3-113">Properties</span></span>

| <span data-ttu-id="f34c3-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="f34c3-114">Property</span></span>     | <span data-ttu-id="f34c3-115">Тип</span><span class="sxs-lookup"><span data-stu-id="f34c3-115">Type</span></span>        | <span data-ttu-id="f34c3-116">Описание</span><span class="sxs-lookup"><span data-stu-id="f34c3-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f34c3-117">id</span><span class="sxs-lookup"><span data-stu-id="f34c3-117">id</span></span>|<span data-ttu-id="f34c3-118">String</span><span class="sxs-lookup"><span data-stu-id="f34c3-118">String</span></span>| <span data-ttu-id="f34c3-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f34c3-119">Read-only.</span></span> <span data-ttu-id="f34c3-120">Уникальный идентификатор, созданный на уровне API.</span><span class="sxs-lookup"><span data-stu-id="f34c3-120">Unique Identifier generated at API level.</span></span>| 
|<span data-ttu-id="f34c3-121">релингпартид</span><span class="sxs-lookup"><span data-stu-id="f34c3-121">relyingPartyId</span></span>|<span data-ttu-id="f34c3-122">String</span><span class="sxs-lookup"><span data-stu-id="f34c3-122">String</span></span>|<span data-ttu-id="f34c3-123">Этот идентификатор используется для идентификации проверяющей стороны в службе Федерации.</span><span class="sxs-lookup"><span data-stu-id="f34c3-123">This identifier is used to identify the relying party to this Federation Service.</span></span> <span data-ttu-id="f34c3-124">Он используется при выдаче утверждений проверяющей стороне.</span><span class="sxs-lookup"><span data-stu-id="f34c3-124">It is used when issuing claims to the relying party.</span></span>|
|<span data-ttu-id="f34c3-125">serviceId</span><span class="sxs-lookup"><span data-stu-id="f34c3-125">serviceId</span></span>|<span data-ttu-id="f34c3-126">String</span><span class="sxs-lookup"><span data-stu-id="f34c3-126">String</span></span>|<span data-ttu-id="f34c3-127">Уникальный идентификатор леса Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f34c3-127">Uniquely identifies the Active Directory forest.</span></span>|
|<span data-ttu-id="f34c3-128">мигратионстатус</span><span class="sxs-lookup"><span data-stu-id="f34c3-128">migrationStatus</span></span>|<span data-ttu-id="f34c3-129">string</span><span class="sxs-lookup"><span data-stu-id="f34c3-129">string</span></span>| <span data-ttu-id="f34c3-130">Указывает, можно ли переместить приложение в Azure AD или потребовать больше расследований.</span><span class="sxs-lookup"><span data-stu-id="f34c3-130">Indication of whether the application can be moved to Azure AD or require more investigation.</span></span> <span data-ttu-id="f34c3-131">Возможные значения: `ready`, `needsReview`, `additionalStepsRequired`.</span><span class="sxs-lookup"><span data-stu-id="f34c3-131">Possible values are: `ready`, `needsReview`, `additionalStepsRequired`.</span></span>|
|<span data-ttu-id="f34c3-132">мигратионвалидатиондетаилс</span><span class="sxs-lookup"><span data-stu-id="f34c3-132">migrationValidationDetails</span></span>|<span data-ttu-id="f34c3-133">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f34c3-133">[keyValuePair](keyvaluepair.md) collection</span></span>|<span data-ttu-id="f34c3-134">Указывает все проверки на правильность конфигурации приложений, которые позволяют оценить, готово ли приложение к перемещению в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f34c3-134">Specifies all the validations check done on applications configuration details to evaluate if the application is ready to be moved to Azure AD.</span></span> <span data-ttu-id="f34c3-135">Возможные `AdditionalWSFedEndpointCheckResult`имена:, `AllowedAuthenticationClassReferencesCheckResult`, `AlwaysRequireAuthenticationCheckResult`, `AutoUpdateEnabledCheckResult`, `ClaimsProviderNameCheckResult`, `EncryptClaimsCheckResult`, `EncryptedNameIdRequiredCheckResult`, `MonitoringEnabledCheckResult`,`NotBeforeSkewCheckResult` `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult`,,,, `TokenLifetimeCheckResult`, `DelegationAuthorizationRulesCheckResult`, `IssuanceAuthorizationRulesCheckResult`,. `IssuanceTransformRulesCheckResult`</span><span class="sxs-lookup"><span data-stu-id="f34c3-135">Possible names are: `AdditionalWSFedEndpointCheckResult`,  `AllowedAuthenticationClassReferencesCheckResult`, `AlwaysRequireAuthenticationCheckResult`,   `AutoUpdateEnabledCheckResult`, `ClaimsProviderNameCheckResult`, `EncryptClaimsCheckResult`,  `EncryptedNameIdRequiredCheckResult`, `MonitoringEnabledCheckResult`,`NotBeforeSkewCheckResult`,  `RequestMFAFromClaimsProvidersCheckResult`, `SignedSamlRequestsRequiredCheckResult`, `AdditionalAuthenticationRulesCheckResult`, `TokenLifetimeCheckResult`,  `DelegationAuthorizationRulesCheckResult`, `IssuanceAuthorizationRulesCheckResult`, `IssuanceTransformRulesCheckResult`.</span></span> <span data-ttu-id="f34c3-136">Возможные значения result: `0`, `1`, или `2`.</span><span class="sxs-lookup"><span data-stu-id="f34c3-136">Possible result values are `0`, `1`, or `2`.</span></span> <span data-ttu-id="f34c3-137">`0`Когда проверка проверки пройдена, `1` при неудачной проверке и `2` при проверке на наличие предупреждения.</span><span class="sxs-lookup"><span data-stu-id="f34c3-137">`0` when the validation check passed, `1` when the validation check failed and `2` when the validation check is a warning.</span></span> |
|<span data-ttu-id="f34c3-138">релингпартинаме</span><span class="sxs-lookup"><span data-stu-id="f34c3-138">relyingPartyName</span></span>|<span data-ttu-id="f34c3-139">String</span><span class="sxs-lookup"><span data-stu-id="f34c3-139">String</span></span>|<span data-ttu-id="f34c3-140">Имя приложения или другой сущности в Интернете, которая использует поставщика удостоверений для проверки подлинности пользователя, который хочет войти в систему.</span><span class="sxs-lookup"><span data-stu-id="f34c3-140">Name of application or other entity on the internet that uses an identity provider to authenticate a user who wants to log in.</span></span>|
|<span data-ttu-id="f34c3-141">фаиледсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="f34c3-141">failedSignInCount</span></span>|<span data-ttu-id="f34c3-142">Int64</span><span class="sxs-lookup"><span data-stu-id="f34c3-142">Int64</span></span>| <span data-ttu-id="f34c3-143">Количество неудачных входов в службу федерации Active Directory в указанном периоде.</span><span class="sxs-lookup"><span data-stu-id="f34c3-143">Number of failed sign in on Active Directory Federation Service in the period specified.</span></span> |
|<span data-ttu-id="f34c3-144">replyUrls</span><span class="sxs-lookup"><span data-stu-id="f34c3-144">replyUrls</span></span>|<span data-ttu-id="f34c3-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f34c3-145">String collection</span></span>|<span data-ttu-id="f34c3-146">Указывает, где ожидается получение маркера проверяющей стороной.</span><span class="sxs-lookup"><span data-stu-id="f34c3-146">Specifies where the relying party expects to receive the token.</span></span>|
|<span data-ttu-id="f34c3-147">сигнинсукцессрате</span><span class="sxs-lookup"><span data-stu-id="f34c3-147">signInSuccessRate</span></span>|<span data-ttu-id="f34c3-148">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="f34c3-148">Double</span></span>|<span data-ttu-id="f34c3-149">Количество успешных/(количество успешных и неудачных входов + количество неудачных входов) в службе федерации Active Directory в указанном периоде.</span><span class="sxs-lookup"><span data-stu-id="f34c3-149">Number of successful / (number of successful + number of failed sign ins) on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="f34c3-150">сукцессфулсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="f34c3-150">successfulSignInCount</span></span>|<span data-ttu-id="f34c3-151">Int64</span><span class="sxs-lookup"><span data-stu-id="f34c3-151">Int64</span></span>|<span data-ttu-id="f34c3-152">Количество успешных входов в службу федерации Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f34c3-152">Number of successful sign ins on Active Directory Federation Service.</span></span>|
|<span data-ttu-id="f34c3-153">тоталсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="f34c3-153">totalSignInCount</span></span>|<span data-ttu-id="f34c3-154">Int64</span><span class="sxs-lookup"><span data-stu-id="f34c3-154">Int64</span></span>|<span data-ttu-id="f34c3-155">Количество успешных и неудачных входных входов в службу федерации Active Directory в указанном периоде.</span><span class="sxs-lookup"><span data-stu-id="f34c3-155">Number of successful + failed sign ins failed sign ins on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="f34c3-156">уникуеусеркаунт</span><span class="sxs-lookup"><span data-stu-id="f34c3-156">uniqueUserCount</span></span>|<span data-ttu-id="f34c3-157">Int64</span><span class="sxs-lookup"><span data-stu-id="f34c3-157">Int64</span></span>|<span data-ttu-id="f34c3-158">Количество уникальных пользователей, выполнивших вход в приложение.</span><span class="sxs-lookup"><span data-stu-id="f34c3-158">Number of unique users that have signed into the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f34c3-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="f34c3-159">Relationships</span></span>

<span data-ttu-id="f34c3-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f34c3-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f34c3-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f34c3-161">JSON representation</span></span>

<span data-ttu-id="f34c3-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f34c3-162">The following is a JSON representation of the resource.</span></span>

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
