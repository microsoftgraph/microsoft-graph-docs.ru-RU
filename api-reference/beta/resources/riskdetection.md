---
title: Тип ресурса Рискдетектион
description: Представляет все обнаруженные риски в клиентах AzureAD.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: de889892e023d5d6036ab1886534d94c4362d641
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448593"
---
# <a name="riskdetection-resource-type"></a><span data-ttu-id="bf52f-103">Тип ресурса Рискдетектион</span><span class="sxs-lookup"><span data-stu-id="bf52f-103">riskDetection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf52f-104">Представляет сведения об обнаруженном риске в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bf52f-104">Represents information about a detected risk in an Azure AD tenant.</span></span> 

<span data-ttu-id="bf52f-105">Azure AD постоянно оценивает риск для пользователей и входа в зависимости от различных сигналов и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="bf52f-105">Azure AD continually evaluates user and sign-in risk based on various signals and machine learning.</span></span> <span data-ttu-id="bf52f-106">Этот API предоставляет программный доступ ко всем обнаружениям рисков в среде Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bf52f-106">This API provides programmatic access to all risk detections in your Azure AD environment.</span></span>

<span data-ttu-id="bf52f-107">Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверений Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="bf52f-107">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

>[!NOTE]
><span data-ttu-id="bf52f-108">Для использования API обнаружения рисков необходима лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="bf52f-108">You must have an Azure AD Premium P2 license to use the risk detection API.</span></span>

## <a name="methods"></a><span data-ttu-id="bf52f-109">Методы</span><span class="sxs-lookup"><span data-stu-id="bf52f-109">Methods</span></span>

| <span data-ttu-id="bf52f-110">Метод</span><span class="sxs-lookup"><span data-stu-id="bf52f-110">Method</span></span>   | <span data-ttu-id="bf52f-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bf52f-111">Return Type</span></span>|<span data-ttu-id="bf52f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bf52f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf52f-113">Список Рискдетектион</span><span class="sxs-lookup"><span data-stu-id="bf52f-113">List riskDetection</span></span>](../api/riskdetection-list.md) | <span data-ttu-id="bf52f-114">Коллекция [рискдетектион](riskdetection.md)</span><span class="sxs-lookup"><span data-stu-id="bf52f-114">[riskDetection](riskdetection.md) collection</span></span>|<span data-ttu-id="bf52f-115">Перечисление обнаруженных рисков и их свойств.</span><span class="sxs-lookup"><span data-stu-id="bf52f-115">List risk detections and their properties.</span></span>|
|[<span data-ttu-id="bf52f-116">Получение Рискдетектион</span><span class="sxs-lookup"><span data-stu-id="bf52f-116">Get riskDetection</span></span>](../api/riskdetection-get.md) | [<span data-ttu-id="bf52f-117">Рискдетектион</span><span class="sxs-lookup"><span data-stu-id="bf52f-117">riskDetection</span></span>](riskdetection.md)|<span data-ttu-id="bf52f-118">Получение определенного опасного обнаружения и его свойств.</span><span class="sxs-lookup"><span data-stu-id="bf52f-118">Get a specific risky detection and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="bf52f-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf52f-119">Properties</span></span>

| <span data-ttu-id="bf52f-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf52f-120">Property</span></span>   | <span data-ttu-id="bf52f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="bf52f-121">Type</span></span>|<span data-ttu-id="bf52f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bf52f-122">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="bf52f-123">Уникальный идентификатор обнаружения риска.</span><span class="sxs-lookup"><span data-stu-id="bf52f-123">Unique ID of the risk detection.</span></span> |
|`requestId`|`string`|<span data-ttu-id="bf52f-124">Идентификатор запроса, связанный с обнаружением риска.</span><span class="sxs-lookup"><span data-stu-id="bf52f-124">Request ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="bf52f-125">Это свойство имеет значение null, если обнаружение риска не связано с входом.</span><span class="sxs-lookup"><span data-stu-id="bf52f-125">This property is null if the risk detection is not associated with a sign-in.</span></span>|
|`correlationId`|`string`|<span data-ttu-id="bf52f-126">Корреляционный идентификатор входа, связанный с обнаружением риска.</span><span class="sxs-lookup"><span data-stu-id="bf52f-126">Correlation ID of the sign-in associated with the risk detection.</span></span> <span data-ttu-id="bf52f-127">Это свойство имеет значение null, если обнаружение риска не связано с входом.</span><span class="sxs-lookup"><span data-stu-id="bf52f-127">This property is null if the risk detection is not associated with a sign-in.</span></span> |
|`riskType`|`riskEventType`|<span data-ttu-id="bf52f-128">Тип обнаруженного события риска.</span><span class="sxs-lookup"><span data-stu-id="bf52f-128">The type of risk event detected.</span></span> <span data-ttu-id="bf52f-129">Возможные значения: Унликелитравел, Анонимизедипаддресс, МалиЦиаусипаддресс, Унфамилиарфеатурес, Малвареинфектедипаддресс, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, genericadminConfirmedUserCompromised , Мкасимпоссиблетравел, МкассуспиЦиаусинбоксманипулатионрулес, Инвестигатионссреатинтеллиженцесигнинлинкед, maliciousIPAddressValidCredentialsBlockedIP и unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="bf52f-129">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, genericadminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, and unknownFutureValue.</span></span> |
|`riskState`|`riskState`|<span data-ttu-id="bf52f-130">Состояние обнаруженного опасного пользователя или входа.</span><span class="sxs-lookup"><span data-stu-id="bf52f-130">The state of a detected risky user or sign-in.</span></span> <span data-ttu-id="bf52f-131">Возможные значения: None, Конфирмедсафе, remediateо, Атриск, Конфирмедкомпромисед и unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="bf52f-131">The possible values are none, confirmedSafe, remediated, dismissed, atRisk, confirmedCompromised, and unknownFutureValue.</span></span> |
|`riskLevel`|`riskLevel`|<span data-ttu-id="bf52f-132">Уровень обнаруженного риска.</span><span class="sxs-lookup"><span data-stu-id="bf52f-132">Level of the detected risk.</span></span> <span data-ttu-id="bf52f-133">Возможные значения: "минимум", "средний", "высокий", "скрытый", "нет", unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="bf52f-133">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span> |
|`riskDetail`|`riskDetail`|<span data-ttu-id="bf52f-134">Сведения об обнаруженном риске.</span><span class="sxs-lookup"><span data-stu-id="bf52f-134">Details of the detected risk.</span></span> <span data-ttu-id="bf52f-135">Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, Админдисмисседаллрискфорусер, Админконфирмедсигнинкомпромисед, Hidden, Админконфирмедусеркомпромисед, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="bf52f-135">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span> |
|`source`|`string`|<span data-ttu-id="bf52f-136">Источник обнаружения риска.</span><span class="sxs-lookup"><span data-stu-id="bf52f-136">Source of the risk detection.</span></span> <span data-ttu-id="bf52f-137">Например, "activeDirectory".</span><span class="sxs-lookup"><span data-stu-id="bf52f-137">For example, "activeDirectory".</span></span> |
|`detectionTimingType`|`riskDetectionTimingType`|<span data-ttu-id="bf52f-138">Время обнаружения риска в режиме реального времени (режим реального времени/автономный режим).</span><span class="sxs-lookup"><span data-stu-id="bf52f-138">Timing of the detected risk (real-time/offline).</span></span> <span data-ttu-id="bf52f-139">Возможные значения: Нотдефинед, реального времени, Неарреалтиме, offline, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="bf52f-139">The possible values are notDefined, realtime, nearRealtime, offline, unknownFutureValue.</span></span> |
|`activity`|`activityType`|<span data-ttu-id="bf52f-140">Указывает тип действия, с которым связан обнаруженный риск.</span><span class="sxs-lookup"><span data-stu-id="bf52f-140">Indicates the activity type the detected risk is linked to.</span></span> <span data-ttu-id="bf52f-141">Возможные значения: Signing, User, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="bf52f-141">The possible values are signin, user, unknownFutureValue.</span></span> |
|`tokenIssuerType`|`tokenIssuerType`|<span data-ttu-id="bf52f-142">Указывает тип поставщика маркеров для обнаруженного риска при входе.</span><span class="sxs-lookup"><span data-stu-id="bf52f-142">Indicates the type of token issuer for the detected sign-in risk.</span></span> <span data-ttu-id="bf52f-143">Возможные значения: AzureAD, Адфедератионсервицес и unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="bf52f-143">The possible values are AzureAD, ADFederationServices, and unknownFutureValue.</span></span> |
|`ipAddress`|`string`|<span data-ttu-id="bf52f-144">Предоставляет IP-адрес клиента, с которого произошел риск.</span><span class="sxs-lookup"><span data-stu-id="bf52f-144">Provides the IP address of the client from where the risk occurred.</span></span> |
|`location`|[`signInLocation`](signinlocation.md)|<span data-ttu-id="bf52f-145">Расположение входа в систему.</span><span class="sxs-lookup"><span data-stu-id="bf52f-145">Location of the sign-in.</span></span> |
|`activityDateTime`|`datetimeoffset`|<span data-ttu-id="bf52f-146">Дата и время, когда возникло опасное действие.</span><span class="sxs-lookup"><span data-stu-id="bf52f-146">Date and time that the risky activity occurred.</span></span> |
|`detectedDateTime`|`datetimeoffset`|<span data-ttu-id="bf52f-147">Дата и время обнаружения риска.</span><span class="sxs-lookup"><span data-stu-id="bf52f-147">Date and time that the risk was detected.</span></span> |
|`lastUpdatedDateTime`|`datetime`|<span data-ttu-id="bf52f-148">Дата и время последнего обновления обнаружения риска.</span><span class="sxs-lookup"><span data-stu-id="bf52f-148">Date and time that the risk detection was last updated.</span></span> |
|`userId`|`string`|<span data-ttu-id="bf52f-149">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf52f-149">Unique ID of the user.</span></span> |
|`userDisplayName`|`string`|<span data-ttu-id="bf52f-150">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf52f-150">Name of the user.</span></span> |
|`userPrincipalName`|`string`|<span data-ttu-id="bf52f-151">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="bf52f-151">The user principal name (UPN) of the user.</span></span> |
|`additionalInfo`|`string`|<span data-ttu-id="bf52f-152">Дополнительные сведения, связанные с определением риска в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf52f-152">Additional information associated with the risk detection in JSON format.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bf52f-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf52f-153">JSON representation</span></span>

<span data-ttu-id="bf52f-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf52f-154">Here is a JSON representation of the resource.</span></span>

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
