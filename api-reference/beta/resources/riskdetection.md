---
title: тип ресурса riskDetection
description: Представляет все обнаружения рисков в клиентах AzureAD.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 40fa938f94f5f43a61c191a3d3c14b0dbbb10d6f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440138"
---
# <a name="riskdetection-resource-type"></a><span data-ttu-id="473a9-103">тип ресурса riskDetection</span><span class="sxs-lookup"><span data-stu-id="473a9-103">riskDetection resource type</span></span>

<span data-ttu-id="473a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="473a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="473a9-105">Представляет сведения об обнаруженном риске в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="473a9-105">Represents information about a detected risk in an Azure AD tenant.</span></span> 

<span data-ttu-id="473a9-106">Azure AD непрерывно [](riskyuser.md) оценивает риски пользователей и [](signin.md) рисков, связанных с входом приложения или пользователя на основе различных сигналов и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="473a9-106">Azure AD continually evaluates [user risks](riskyuser.md) and app or user [sign-in](signin.md) risks based on various signals and machine learning.</span></span> <span data-ttu-id="473a9-107">Этот API предоставляет программный доступ ко всем обнаружениям рисков в среде Azure AD.</span><span class="sxs-lookup"><span data-stu-id="473a9-107">This API provides programmatic access to all risk detections in your Azure AD environment.</span></span>

<span data-ttu-id="473a9-108">Дополнительные сведения о событиях с рисками см. в [видеоролике Azure Active Directory Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="473a9-108">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

>[!NOTE]
><span data-ttu-id="473a9-109">Чтобы использовать API обнаружения рисков, необходимо иметь лицензию Azure AD Premium P1 или P2.</span><span class="sxs-lookup"><span data-stu-id="473a9-109">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="methods"></a><span data-ttu-id="473a9-110">Методы</span><span class="sxs-lookup"><span data-stu-id="473a9-110">Methods</span></span>

| <span data-ttu-id="473a9-111">Метод</span><span class="sxs-lookup"><span data-stu-id="473a9-111">Method</span></span>   | <span data-ttu-id="473a9-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="473a9-112">Return Type</span></span>|<span data-ttu-id="473a9-113">Описание</span><span class="sxs-lookup"><span data-stu-id="473a9-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="473a9-114">List riskDetection</span><span class="sxs-lookup"><span data-stu-id="473a9-114">List riskDetection</span></span>](../api/riskdetection-list.md) | <span data-ttu-id="473a9-115">[коллекция riskDetection](riskdetection.md)</span><span class="sxs-lookup"><span data-stu-id="473a9-115">[riskDetection](riskdetection.md) collection</span></span>|<span data-ttu-id="473a9-116">Список обнаружения рисков и их свойств.</span><span class="sxs-lookup"><span data-stu-id="473a9-116">List risk detections and their properties.</span></span>|
|[<span data-ttu-id="473a9-117">Get riskDetection</span><span class="sxs-lookup"><span data-stu-id="473a9-117">Get riskDetection</span></span>](../api/riskdetection-get.md) | [<span data-ttu-id="473a9-118">riskDetection</span><span class="sxs-lookup"><span data-stu-id="473a9-118">riskDetection</span></span>](riskdetection.md)|<span data-ttu-id="473a9-119">Получите определенное обнаружение рисков и его свойства.</span><span class="sxs-lookup"><span data-stu-id="473a9-119">Get a specific risky detection and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="473a9-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="473a9-120">Properties</span></span>

| <span data-ttu-id="473a9-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="473a9-121">Property</span></span>   | <span data-ttu-id="473a9-122">Тип</span><span class="sxs-lookup"><span data-stu-id="473a9-122">Type</span></span>|<span data-ttu-id="473a9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="473a9-123">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="473a9-124">Уникальный ID обнаружения рисков.</span><span class="sxs-lookup"><span data-stu-id="473a9-124">Unique ID of the risk detection.</span></span> |
|`requestId`|`string`|<span data-ttu-id="473a9-125">Запрос iD входного знака, связанного с обнаружением рисков.</span><span class="sxs-lookup"><span data-stu-id="473a9-125">Request ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="473a9-126">Это свойство является null, если обнаружение риска не связано с входом.</span><span class="sxs-lookup"><span data-stu-id="473a9-126">This property is null if the risk detection is not associated with a sign-in.</span></span>|
|`correlationId`|`string`|<span data-ttu-id="473a9-127">Корреляция ID входного знака, связанного с обнаружением риска.</span><span class="sxs-lookup"><span data-stu-id="473a9-127">Correlation ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="473a9-128">Это свойство является null, если обнаружение риска не связано с входом.</span><span class="sxs-lookup"><span data-stu-id="473a9-128">This property is null if the risk detection is not associated with a sign-in.</span></span> |
|`riskEventType`|`string`|<span data-ttu-id="473a9-129">Тип обнаруженного события риска.</span><span class="sxs-lookup"><span data-stu-id="473a9-129">The type of risk event detected.</span></span> <span data-ttu-id="473a9-130">Возможные `unlikelyTravel` значения: `anonymizedIPAddress` , `maliciousIPAddress` , , , , , , , , `unfamiliarFeatures` и `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="473a9-130">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
|`riskType`|`riskEventType`|<span data-ttu-id="473a9-131">Список типов событий риска.</span><span class="sxs-lookup"><span data-stu-id="473a9-131">List of risk event types.</span></span><br/><span data-ttu-id="473a9-132">**Примечание:** Это свойство обесценилось.</span><span class="sxs-lookup"><span data-stu-id="473a9-132">**Note:** This property is deprecated.</span></span> <span data-ttu-id="473a9-133">Вместо **этого используйте riskEventTypes.**</span><span class="sxs-lookup"><span data-stu-id="473a9-133">Use **riskEventTypes** instead.</span></span> |
|`riskState`|`riskState`|<span data-ttu-id="473a9-134">Состояние обнаруженного рискованного пользователя или входной записи.</span><span class="sxs-lookup"><span data-stu-id="473a9-134">The state of a detected risky user or sign-in.</span></span> <span data-ttu-id="473a9-135">Возможные значения не являются никакими, подтвержденнымиSafe, исправленными, уволенными, atRisk, confirmedCompromised и unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="473a9-135">The possible values are none, confirmedSafe, remediated, dismissed, atRisk, confirmedCompromised, and unknownFutureValue.</span></span> |
|`riskLevel`|`riskLevel`|<span data-ttu-id="473a9-136">Уровень обнаруженного риска.</span><span class="sxs-lookup"><span data-stu-id="473a9-136">Level of the detected risk.</span></span> <span data-ttu-id="473a9-137">Возможные значения : низкие, средние, высокие, скрытые, неизвестные.</span><span class="sxs-lookup"><span data-stu-id="473a9-137">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span> <span data-ttu-id="473a9-138">**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="473a9-138">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="473a9-139">Клиенты P1 будут `hidden` возвращены.</span><span class="sxs-lookup"><span data-stu-id="473a9-139">P1 customers will be returned `hidden`.</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="473a9-140">Сведения об обнаружении риска.</span><span class="sxs-lookup"><span data-stu-id="473a9-140">Details of the detected risk.</span></span> <span data-ttu-id="473a9-141">Возможные значения не являются никакими, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="473a9-141">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span> <span data-ttu-id="473a9-142">**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="473a9-142">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="473a9-143">Клиенты P1 будут `hidden` возвращены.</span><span class="sxs-lookup"><span data-stu-id="473a9-143">P1 customers will be returned `hidden`.</span></span>|
|`source`|`string`|<span data-ttu-id="473a9-144">Источник обнаружения рисков.</span><span class="sxs-lookup"><span data-stu-id="473a9-144">Source of the risk detection.</span></span> <span data-ttu-id="473a9-145">Например, "activeDirectory".</span><span class="sxs-lookup"><span data-stu-id="473a9-145">For example, "activeDirectory".</span></span> |
|`detectionTimingType`|`riskDetectionTimingType`|<span data-ttu-id="473a9-146">Сроки обнаружения риска (в режиме реального времени и в автономном режиме).</span><span class="sxs-lookup"><span data-stu-id="473a9-146">Timing of the detected risk (real-time/offline).</span></span> <span data-ttu-id="473a9-147">Возможные значения неDefined, realtime, nearRealtime, автономно, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="473a9-147">The possible values are notDefined, realtime, nearRealtime, offline, unknownFutureValue.</span></span> |
|`activity`|`activityType`|<span data-ttu-id="473a9-148">Указывает тип активности, с чем связан обнаруженный риск.</span><span class="sxs-lookup"><span data-stu-id="473a9-148">Indicates the activity type the detected risk is linked to.</span></span> <span data-ttu-id="473a9-149">Возможные значения : signin, user, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="473a9-149">The possible values are signin, user, unknownFutureValue.</span></span> |
|`tokenIssuerType`|`tokenIssuerType`|<span data-ttu-id="473a9-150">Указывает тип эмитента маркеров для обнаруженного риска входного знака.</span><span class="sxs-lookup"><span data-stu-id="473a9-150">Indicates the type of token issuer for the detected sign-in risk.</span></span> <span data-ttu-id="473a9-151">Возможные значения : AzureAD, ADFederationServices и unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="473a9-151">The possible values are AzureAD, ADFederationServices, and unknownFutureValue.</span></span> |
|`ipAddress`|`string`|<span data-ttu-id="473a9-152">Предоставляет IP-адрес клиента, откуда возник риск.</span><span class="sxs-lookup"><span data-stu-id="473a9-152">Provides the IP address of the client from where the risk occurred.</span></span> |
|`location`|[<span data-ttu-id="473a9-153">signInLocation</span><span class="sxs-lookup"><span data-stu-id="473a9-153">signInLocation</span></span>](signinlocation.md)|<span data-ttu-id="473a9-154">Расположение входного знака.</span><span class="sxs-lookup"><span data-stu-id="473a9-154">Location of the sign-in.</span></span> |
|`activityDateTime`|`datetimeoffset`|<span data-ttu-id="473a9-155">Дата и время возникновения рискованных действий.</span><span class="sxs-lookup"><span data-stu-id="473a9-155">Date and time that the risky activity occurred.</span></span> |
|`detectedDateTime`|`datetimeoffset`|<span data-ttu-id="473a9-156">Дата и время обнаружения риска.</span><span class="sxs-lookup"><span data-stu-id="473a9-156">Date and time that the risk was detected.</span></span> |
|`lastUpdatedDateTime`|`datetime`|<span data-ttu-id="473a9-157">Дата и время последнего обновления обнаружения рисков.</span><span class="sxs-lookup"><span data-stu-id="473a9-157">Date and time that the risk detection was last updated.</span></span> |
|`userId`|`string`|<span data-ttu-id="473a9-158">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="473a9-158">Unique ID of the user.</span></span> |
|`userDisplayName`|`string`|<span data-ttu-id="473a9-159">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="473a9-159">Name of the user.</span></span> |
|`userPrincipalName`|`string`|<span data-ttu-id="473a9-160">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="473a9-160">The user principal name (UPN) of the user.</span></span> |
|`additionalInfo`|`string`|<span data-ttu-id="473a9-161">Дополнительные сведения, связанные с обнаружением рисков в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="473a9-161">Additional information associated with the risk detection in JSON format.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="473a9-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="473a9-162">JSON representation</span></span>

<span data-ttu-id="473a9-163">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="473a9-163">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskDetection"
}-->

```json
{
 "id": "string",
    "requestId": "string",
    "correlationId": "string",
    "riskType": {"@odata.type": "microsoft.graph.riskEventType"},
    "riskState": {"@odata.type": "microsoft.graph.riskState"},
    "riskLevel": {"@odata.type": "microsoft.graph.riskLevel"},
    "riskDetail": {"@odata.type": "microsoft.graph.riskDetail"},
    "source": "string",
    "detectionTimingType": {"@odata.type": "microsoft.graph.riskDetectionTimingType"},
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"},
    "tokenIssuerType": {"@odata.type": "microsoft.graph.tokenIssuerType"},
    "ipAddress": "string",
    "location": {"@odata.type": "microsoft.graph.signInLocation"},
    "activityDateTime": "string (timestamp)",
    "detectedDateTime": "string (timestamp)",
    "lastUpdatedDateTime": "string (timestamp)",
    "userId": "string",
    "userDisplayName": "string",
    "userPrincipalName": "string",
    "additionalInfo": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskDetections resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
