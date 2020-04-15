---
title: Тип ресурса Рискдетектион
description: Представляет все обнаруженные риски в клиентах AzureAD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 01d0f5c566a3c633caab8e321202e422bbad62a8
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2020
ms.locfileid: "43511003"
---
# <a name="riskdetection-resource-type"></a><span data-ttu-id="08757-103">Тип ресурса Рискдетектион</span><span class="sxs-lookup"><span data-stu-id="08757-103">riskDetection resource type</span></span>

<span data-ttu-id="08757-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08757-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08757-105">Представляет сведения об обнаруженном риске в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="08757-105">Represents information about a detected risk in an Azure AD tenant.</span></span> 

<span data-ttu-id="08757-106">Azure AD постоянно оценивает [риски пользователей](riskyuser.md) , риски, связанные с [входом](signin.md) пользователей и пользователями, на основе различных сигналов и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="08757-106">Azure AD continually evaluates [user risks](riskyuser.md) and app or user [sign-in](signin.md) risks based on various signals and machine learning.</span></span> <span data-ttu-id="08757-107">Этот API предоставляет программный доступ ко всем обнаружениям рисков в среде Azure AD.</span><span class="sxs-lookup"><span data-stu-id="08757-107">This API provides programmatic access to all risk detections in your Azure AD environment.</span></span>

<span data-ttu-id="08757-108">Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="08757-108">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span></span>

>[!NOTE]
><span data-ttu-id="08757-109">Для использования API обнаружения риска необходима лицензия Azure AD Premium P1 или P2.</span><span class="sxs-lookup"><span data-stu-id="08757-109">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="methods"></a><span data-ttu-id="08757-110">Методы</span><span class="sxs-lookup"><span data-stu-id="08757-110">Methods</span></span>

| <span data-ttu-id="08757-111">Метод</span><span class="sxs-lookup"><span data-stu-id="08757-111">Method</span></span>   | <span data-ttu-id="08757-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="08757-112">Return Type</span></span>|<span data-ttu-id="08757-113">Описание</span><span class="sxs-lookup"><span data-stu-id="08757-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="08757-114">Список Рискдетектион</span><span class="sxs-lookup"><span data-stu-id="08757-114">List riskDetection</span></span>](../api/riskdetection-list.md) | <span data-ttu-id="08757-115">Коллекция [рискдетектион](riskdetection.md)</span><span class="sxs-lookup"><span data-stu-id="08757-115">[riskDetection](riskdetection.md) collection</span></span>|<span data-ttu-id="08757-116">Перечисление обнаруженных рисков и их свойств.</span><span class="sxs-lookup"><span data-stu-id="08757-116">List risk detections and their properties.</span></span>|
|[<span data-ttu-id="08757-117">Получение Рискдетектион</span><span class="sxs-lookup"><span data-stu-id="08757-117">Get riskDetection</span></span>](../api/riskdetection-get.md) | [<span data-ttu-id="08757-118">рискдетектион</span><span class="sxs-lookup"><span data-stu-id="08757-118">riskDetection</span></span>](riskdetection.md)|<span data-ttu-id="08757-119">Получение определенного опасного обнаружения и его свойств.</span><span class="sxs-lookup"><span data-stu-id="08757-119">Get a specific risky detection and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="08757-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="08757-120">Properties</span></span>

| <span data-ttu-id="08757-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="08757-121">Property</span></span>   | <span data-ttu-id="08757-122">Тип</span><span class="sxs-lookup"><span data-stu-id="08757-122">Type</span></span>|<span data-ttu-id="08757-123">Описание</span><span class="sxs-lookup"><span data-stu-id="08757-123">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="08757-124">Уникальный идентификатор обнаружения риска.</span><span class="sxs-lookup"><span data-stu-id="08757-124">Unique ID of the risk detection.</span></span> |
|`requestId`|`string`|<span data-ttu-id="08757-125">Идентификатор запроса, связанный с обнаружением риска.</span><span class="sxs-lookup"><span data-stu-id="08757-125">Request ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="08757-126">Это свойство имеет значение null, если обнаружение риска не связано с входом.</span><span class="sxs-lookup"><span data-stu-id="08757-126">This property is null if the risk detection is not associated with a sign-in.</span></span>|
|`correlationId`|`string`|<span data-ttu-id="08757-127">Корреляционный идентификатор входа, связанный с обнаружением риска.</span><span class="sxs-lookup"><span data-stu-id="08757-127">Correlation ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="08757-128">Это свойство имеет значение null, если обнаружение риска не связано с входом.</span><span class="sxs-lookup"><span data-stu-id="08757-128">This property is null if the risk detection is not associated with a sign-in.</span></span> |
|`riskEventType`|`string`|<span data-ttu-id="08757-129">Тип обнаруженного события риска.</span><span class="sxs-lookup"><span data-stu-id="08757-129">The type of risk event detected.</span></span> <span data-ttu-id="08757-130">Возможные значения: `unlikelyTravel` `anonymizedIPAddress`,, `maliciousIPAddress`, `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials`,,,, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `unknownFutureValue`,,,, и. `maliciousIPAddressValidCredentialsBlockedIP`</span><span class="sxs-lookup"><span data-stu-id="08757-130">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
|`riskType`|`riskEventType`|<span data-ttu-id="08757-131">Список типов событий риска.</span><span class="sxs-lookup"><span data-stu-id="08757-131">List of risk event types.</span></span><br/><span data-ttu-id="08757-132">**Примечание:** Это свойство является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="08757-132">**Note:** This property is deprecated.</span></span> <span data-ttu-id="08757-133">Вместо этого используйте **рискевенттипес** .</span><span class="sxs-lookup"><span data-stu-id="08757-133">Use **riskEventTypes** instead.</span></span> |
|`riskState`|`riskState`|<span data-ttu-id="08757-134">Состояние обнаруженного опасного пользователя или входа.</span><span class="sxs-lookup"><span data-stu-id="08757-134">The state of a detected risky user or sign-in.</span></span> <span data-ttu-id="08757-135">Возможные значения: None, Конфирмедсафе, remediateо, Атриск, Конфирмедкомпромисед и unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="08757-135">The possible values are none, confirmedSafe, remediated, dismissed, atRisk, confirmedCompromised, and unknownFutureValue.</span></span> |
|`riskLevel`|`riskLevel`|<span data-ttu-id="08757-136">Уровень обнаруженного риска.</span><span class="sxs-lookup"><span data-stu-id="08757-136">Level of the detected risk.</span></span> <span data-ttu-id="08757-137">Возможные значения: "минимум", "средний", "высокий", "скрытый", "нет", unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="08757-137">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span> <span data-ttu-id="08757-138">**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="08757-138">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="08757-139">Клиенты P1 будут возвращены `hidden`.</span><span class="sxs-lookup"><span data-stu-id="08757-139">P1 customers will be returned `hidden`.</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="08757-140">Сведения об обнаруженном риске.</span><span class="sxs-lookup"><span data-stu-id="08757-140">Details of the detected risk.</span></span> <span data-ttu-id="08757-141">Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, Hidden, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="08757-141">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span> <span data-ttu-id="08757-142">**Примечание.** Сведения для этого свойства доступны только для пользователей Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="08757-142">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="08757-143">Клиенты P1 будут возвращены `hidden`.</span><span class="sxs-lookup"><span data-stu-id="08757-143">P1 customers will be returned `hidden`.</span></span>|
|`source`|`string`|<span data-ttu-id="08757-144">Источник обнаружения риска.</span><span class="sxs-lookup"><span data-stu-id="08757-144">Source of the risk detection.</span></span> <span data-ttu-id="08757-145">Например, "activeDirectory".</span><span class="sxs-lookup"><span data-stu-id="08757-145">For example, "activeDirectory".</span></span> |
|`detectionTimingType`|`riskDetectionTimingType`|<span data-ttu-id="08757-146">Время обнаружения риска в режиме реального времени (режим реального времени/автономный режим).</span><span class="sxs-lookup"><span data-stu-id="08757-146">Timing of the detected risk (real-time/offline).</span></span> <span data-ttu-id="08757-147">Возможные значения: Нотдефинед, реального времени, Неарреалтиме, offline, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="08757-147">The possible values are notDefined, realtime, nearRealtime, offline, unknownFutureValue.</span></span> |
|`activity`|`activityType`|<span data-ttu-id="08757-148">Указывает тип действия, с которым связан обнаруженный риск.</span><span class="sxs-lookup"><span data-stu-id="08757-148">Indicates the activity type the detected risk is linked to.</span></span> <span data-ttu-id="08757-149">Возможные значения: Signing, User, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="08757-149">The possible values are signin, user, unknownFutureValue.</span></span> |
|`tokenIssuerType`|`tokenIssuerType`|<span data-ttu-id="08757-150">Указывает тип поставщика маркеров для обнаруженного риска при входе.</span><span class="sxs-lookup"><span data-stu-id="08757-150">Indicates the type of token issuer for the detected sign-in risk.</span></span> <span data-ttu-id="08757-151">Возможные значения: AzureAD, Адфедератионсервицес и unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="08757-151">The possible values are AzureAD, ADFederationServices, and unknownFutureValue.</span></span> |
|`ipAddress`|`string`|<span data-ttu-id="08757-152">Предоставляет IP-адрес клиента, с которого произошел риск.</span><span class="sxs-lookup"><span data-stu-id="08757-152">Provides the IP address of the client from where the risk occurred.</span></span> |
|`location`|[`signInLocation`](signinlocation.md)|<span data-ttu-id="08757-153">Расположение входа в систему.</span><span class="sxs-lookup"><span data-stu-id="08757-153">Location of the sign-in.</span></span> |
|`activityDateTime`|`datetimeoffset`|<span data-ttu-id="08757-154">Дата и время, когда возникло опасное действие.</span><span class="sxs-lookup"><span data-stu-id="08757-154">Date and time that the risky activity occurred.</span></span> |
|`detectedDateTime`|`datetimeoffset`|<span data-ttu-id="08757-155">Дата и время обнаружения риска.</span><span class="sxs-lookup"><span data-stu-id="08757-155">Date and time that the risk was detected.</span></span> |
|`lastUpdatedDateTime`|`datetime`|<span data-ttu-id="08757-156">Дата и время последнего обновления обнаружения риска.</span><span class="sxs-lookup"><span data-stu-id="08757-156">Date and time that the risk detection was last updated.</span></span> |
|`userId`|`string`|<span data-ttu-id="08757-157">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="08757-157">Unique ID of the user.</span></span> |
|`userDisplayName`|`string`|<span data-ttu-id="08757-158">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="08757-158">Name of the user.</span></span> |
|`userPrincipalName`|`string`|<span data-ttu-id="08757-159">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="08757-159">The user principal name (UPN) of the user.</span></span> |
|`additionalInfo`|`string`|<span data-ttu-id="08757-160">Дополнительные сведения, связанные с определением риска в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08757-160">Additional information associated with the risk detection in JSON format.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="08757-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08757-161">JSON representation</span></span>

<span data-ttu-id="08757-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08757-162">The following is a JSON representation of the resource.</span></span>

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
