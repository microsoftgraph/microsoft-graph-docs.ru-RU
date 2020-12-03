---
title: Тип ресурса Релингпартидетаиледсуммари
description: Представляет проверяющую сторону в AD FS.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a3a6fd0ad84ce8e41902cd7c0e82a314fb1aa3ca
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524717"
---
# <a name="relyingpartydetailedsummary-resource-type"></a><span data-ttu-id="b88dd-103">Тип ресурса Релингпартидетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="b88dd-103">relyingPartyDetailedSummary resource type</span></span>

<span data-ttu-id="b88dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b88dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b88dd-105">Представляет проверяющую сторону, настроенную с помощью служб федерации Active Directory (AD FS), его агрегированное использование и возможность переноса конфигурации проверяющей стороны в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b88dd-105">Represents a relying party configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span>

## <a name="methods"></a><span data-ttu-id="b88dd-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b88dd-106">Methods</span></span>

| <span data-ttu-id="b88dd-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b88dd-107">Method</span></span>       | <span data-ttu-id="b88dd-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b88dd-108">Return Type</span></span> | <span data-ttu-id="b88dd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b88dd-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b88dd-110">Список</span><span class="sxs-lookup"><span data-stu-id="b88dd-110">List</span></span>](../api/relyingpartydetailedsummary-list.md) | [<span data-ttu-id="b88dd-111">релингпартидетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="b88dd-111">relyingPartyDetailedSummary</span></span>](relyingpartydetailedsummary.md) | <span data-ttu-id="b88dd-112">Получение списка объектов **релингпартидетаиледсуммари** .</span><span class="sxs-lookup"><span data-stu-id="b88dd-112">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span> |


## <a name="properties"></a><span data-ttu-id="b88dd-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="b88dd-113">Properties</span></span>

| <span data-ttu-id="b88dd-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="b88dd-114">Property</span></span>     | <span data-ttu-id="b88dd-115">Тип</span><span class="sxs-lookup"><span data-stu-id="b88dd-115">Type</span></span>        | <span data-ttu-id="b88dd-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b88dd-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b88dd-117">id</span><span class="sxs-lookup"><span data-stu-id="b88dd-117">id</span></span>|<span data-ttu-id="b88dd-118">String</span><span class="sxs-lookup"><span data-stu-id="b88dd-118">String</span></span>| <span data-ttu-id="b88dd-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b88dd-119">Read-only.</span></span> <span data-ttu-id="b88dd-120">Уникальный идентификатор, созданный на уровне API.</span><span class="sxs-lookup"><span data-stu-id="b88dd-120">Unique Identifier generated at API level.</span></span>| 
|<span data-ttu-id="b88dd-121">релингпартид</span><span class="sxs-lookup"><span data-stu-id="b88dd-121">relyingPartyId</span></span>|<span data-ttu-id="b88dd-122">String</span><span class="sxs-lookup"><span data-stu-id="b88dd-122">String</span></span>|<span data-ttu-id="b88dd-123">Этот идентификатор используется для идентификации проверяющей стороны в службе Федерации.</span><span class="sxs-lookup"><span data-stu-id="b88dd-123">This identifier is used to identify the relying party to this Federation Service.</span></span> <span data-ttu-id="b88dd-124">Он используется при выдаче утверждений проверяющей стороне.</span><span class="sxs-lookup"><span data-stu-id="b88dd-124">It is used when issuing claims to the relying party.</span></span>|
|<span data-ttu-id="b88dd-125">serviceId</span><span class="sxs-lookup"><span data-stu-id="b88dd-125">serviceId</span></span>|<span data-ttu-id="b88dd-126">String</span><span class="sxs-lookup"><span data-stu-id="b88dd-126">String</span></span>|<span data-ttu-id="b88dd-127">Уникальный идентификатор леса Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b88dd-127">Uniquely identifies the Active Directory forest.</span></span>|
|<span data-ttu-id="b88dd-128">мигратионстатус</span><span class="sxs-lookup"><span data-stu-id="b88dd-128">migrationStatus</span></span>|<span data-ttu-id="b88dd-129">string</span><span class="sxs-lookup"><span data-stu-id="b88dd-129">string</span></span>| <span data-ttu-id="b88dd-130">Указывает, можно ли переместить приложение в Azure AD или потребовать больше расследований.</span><span class="sxs-lookup"><span data-stu-id="b88dd-130">Indication of whether the application can be moved to Azure AD or require more investigation.</span></span> <span data-ttu-id="b88dd-131">Возможные значения: `ready`, `needsReview`, `additionalStepsRequired`.</span><span class="sxs-lookup"><span data-stu-id="b88dd-131">Possible values are: `ready`, `needsReview`, `additionalStepsRequired`.</span></span>|
|<span data-ttu-id="b88dd-132">мигратионвалидатиондетаилс</span><span class="sxs-lookup"><span data-stu-id="b88dd-132">migrationValidationDetails</span></span>|<span data-ttu-id="b88dd-133">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b88dd-133">[keyValuePair](keyvaluepair.md) collection</span></span>|<span data-ttu-id="b88dd-134">Указывает все проверки на правильность конфигурации приложений, которые позволяют оценить, готово ли приложение к перемещению в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b88dd-134">Specifies all the validations check done on applications configuration details to evaluate if the application is ready to be moved to Azure AD.</span></span> <span data-ttu-id="b88dd-135">Возможные имена: `AdditionalWSFedEndpointCheckResult` ,,,,,,,,,,,,  `AllowedAuthenticationClassReferencesCheckResult` `AlwaysRequireAuthenticationCheckResult`   `AutoUpdateEnabledCheckResult` `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult`  `EncryptedNameIdRequiredCheckResult` `MonitoringEnabledCheckResult` `NotBeforeSkewCheckResult`  `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult` ,  `DelegationAuthorizationRulesCheckResult` , `IssuanceAuthorizationRulesCheckResult` , `IssuanceTransformRulesCheckResult` .</span><span class="sxs-lookup"><span data-stu-id="b88dd-135">Possible names are: `AdditionalWSFedEndpointCheckResult`,  `AllowedAuthenticationClassReferencesCheckResult`, `AlwaysRequireAuthenticationCheckResult`,   `AutoUpdateEnabledCheckResult`, `ClaimsProviderNameCheckResult`, `EncryptClaimsCheckResult`,  `EncryptedNameIdRequiredCheckResult`, `MonitoringEnabledCheckResult`,`NotBeforeSkewCheckResult`,  `RequestMFAFromClaimsProvidersCheckResult`, `SignedSamlRequestsRequiredCheckResult`, `AdditionalAuthenticationRulesCheckResult`, `TokenLifetimeCheckResult`,  `DelegationAuthorizationRulesCheckResult`, `IssuanceAuthorizationRulesCheckResult`, `IssuanceTransformRulesCheckResult`.</span></span> <span data-ttu-id="b88dd-136">Возможные значения result: `0` , `1` , или `2` .</span><span class="sxs-lookup"><span data-stu-id="b88dd-136">Possible result values are `0`, `1`, or `2`.</span></span> <span data-ttu-id="b88dd-137">`0` Когда проверка проверки пройдена, `1` при неудачной проверке и `2` при проверке на наличие предупреждения.</span><span class="sxs-lookup"><span data-stu-id="b88dd-137">`0` when the validation check passed, `1` when the validation check failed and `2` when the validation check is a warning.</span></span> |
|<span data-ttu-id="b88dd-138">релингпартинаме</span><span class="sxs-lookup"><span data-stu-id="b88dd-138">relyingPartyName</span></span>|<span data-ttu-id="b88dd-139">String</span><span class="sxs-lookup"><span data-stu-id="b88dd-139">String</span></span>|<span data-ttu-id="b88dd-140">Имя приложения или другой сущности в Интернете, которая использует поставщика удостоверений для проверки подлинности пользователя, который хочет войти в систему.</span><span class="sxs-lookup"><span data-stu-id="b88dd-140">Name of application or other entity on the internet that uses an identity provider to authenticate a user who wants to log in.</span></span>|
|<span data-ttu-id="b88dd-141">фаиледсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="b88dd-141">failedSignInCount</span></span>|<span data-ttu-id="b88dd-142">Int64</span><span class="sxs-lookup"><span data-stu-id="b88dd-142">Int64</span></span>| <span data-ttu-id="b88dd-143">Количество неудачных входов в службу федерации Active Directory в указанном периоде.</span><span class="sxs-lookup"><span data-stu-id="b88dd-143">Number of failed sign in on Active Directory Federation Service in the period specified.</span></span> |
|<span data-ttu-id="b88dd-144">replyUrls</span><span class="sxs-lookup"><span data-stu-id="b88dd-144">replyUrls</span></span>|<span data-ttu-id="b88dd-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b88dd-145">String collection</span></span>|<span data-ttu-id="b88dd-146">Указывает, где ожидается получение маркера проверяющей стороной.</span><span class="sxs-lookup"><span data-stu-id="b88dd-146">Specifies where the relying party expects to receive the token.</span></span>|
|<span data-ttu-id="b88dd-147">сигнинсукцессрате</span><span class="sxs-lookup"><span data-stu-id="b88dd-147">signInSuccessRate</span></span>|<span data-ttu-id="b88dd-148">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b88dd-148">Double</span></span>|<span data-ttu-id="b88dd-149">Количество успешных/(количество успешных и неудачных входов + количество неудачных входов) в службе федерации Active Directory в указанном периоде.</span><span class="sxs-lookup"><span data-stu-id="b88dd-149">Number of successful / (number of successful + number of failed sign ins) on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="b88dd-150">сукцессфулсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="b88dd-150">successfulSignInCount</span></span>|<span data-ttu-id="b88dd-151">Int64</span><span class="sxs-lookup"><span data-stu-id="b88dd-151">Int64</span></span>|<span data-ttu-id="b88dd-152">Количество успешных входов в службу федерации Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b88dd-152">Number of successful sign ins on Active Directory Federation Service.</span></span>|
|<span data-ttu-id="b88dd-153">тоталсигнинкаунт</span><span class="sxs-lookup"><span data-stu-id="b88dd-153">totalSignInCount</span></span>|<span data-ttu-id="b88dd-154">Int64</span><span class="sxs-lookup"><span data-stu-id="b88dd-154">Int64</span></span>|<span data-ttu-id="b88dd-155">Количество успешных и неудачных входных входов в службу федерации Active Directory в указанном периоде.</span><span class="sxs-lookup"><span data-stu-id="b88dd-155">Number of successful + failed sign ins failed sign ins on Active Directory Federation Service in the period specified.</span></span>|
|<span data-ttu-id="b88dd-156">уникуеусеркаунт</span><span class="sxs-lookup"><span data-stu-id="b88dd-156">uniqueUserCount</span></span>|<span data-ttu-id="b88dd-157">Int64</span><span class="sxs-lookup"><span data-stu-id="b88dd-157">Int64</span></span>|<span data-ttu-id="b88dd-158">Количество уникальных пользователей, выполнивших вход в приложение.</span><span class="sxs-lookup"><span data-stu-id="b88dd-158">Number of unique users that have signed into the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b88dd-159">Связи</span><span class="sxs-lookup"><span data-stu-id="b88dd-159">Relationships</span></span>

<span data-ttu-id="b88dd-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b88dd-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b88dd-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b88dd-161">JSON representation</span></span>

<span data-ttu-id="b88dd-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b88dd-162">The following is a JSON representation of the resource.</span></span>

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


