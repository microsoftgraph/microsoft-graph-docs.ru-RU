---
title: Тип ресурса userSecurityState
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62a54a996d7fe9c892da797cee352a57d0782035
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517241"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="25cc6-104">Тип ресурса userSecurityState</span><span class="sxs-lookup"><span data-stu-id="25cc6-104">userSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25cc6-105">Содержит информацию о состояниях об учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="25cc6-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="25cc6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="25cc6-106">Properties</span></span>

| <span data-ttu-id="25cc6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="25cc6-107">Property</span></span>   | <span data-ttu-id="25cc6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="25cc6-108">Type</span></span> |<span data-ttu-id="25cc6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="25cc6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25cc6-110">aadUserId</span><span class="sxs-lookup"><span data-stu-id="25cc6-110">aadUserId</span></span>|<span data-ttu-id="25cc6-111">String</span><span class="sxs-lookup"><span data-stu-id="25cc6-111">String</span></span>|<span data-ttu-id="25cc6-112">AAD пользователя объекта идентификатор (GUID) — представляет удостоверение пользователя физических/несколькими-account.</span><span class="sxs-lookup"><span data-stu-id="25cc6-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="25cc6-113">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="25cc6-113">accountName</span></span>|<span data-ttu-id="25cc6-114">String</span><span class="sxs-lookup"><span data-stu-id="25cc6-114">String</span></span>|<span data-ttu-id="25cc6-115">Имя учетной записи для учетной записи пользователя (без домена Active Directory и DNS домена) - (также называемая `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="25cc6-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="25cc6-116">domainName</span><span class="sxs-lookup"><span data-stu-id="25cc6-116">domainName</span></span>|<span data-ttu-id="25cc6-117">String</span><span class="sxs-lookup"><span data-stu-id="25cc6-117">String</span></span>|<span data-ttu-id="25cc6-118">NetBIOS/Active Directory в домен учетной записи пользователя (то есть, в формате домен\учетная запись).</span><span class="sxs-lookup"><span data-stu-id="25cc6-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="25cc6-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="25cc6-119">emailRole</span></span>|<span data-ttu-id="25cc6-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="25cc6-120">emailRole</span></span>|<span data-ttu-id="25cc6-121">Связанные с электронной почты оповещений,-электронной почты для учетной записи пользователя «роли».</span><span class="sxs-lookup"><span data-stu-id="25cc6-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="25cc6-122">Возможные значения: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="25cc6-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="25cc6-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="25cc6-123">isVpn</span></span>|<span data-ttu-id="25cc6-124">Логическое</span><span class="sxs-lookup"><span data-stu-id="25cc6-124">Boolean</span></span>|<span data-ttu-id="25cc6-125">Указывает, вошел ли пользователь через VPN.</span><span class="sxs-lookup"><span data-stu-id="25cc6-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="25cc6-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="25cc6-126">logonDateTime</span></span>|<span data-ttu-id="25cc6-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25cc6-127">DateTimeOffset</span></span>|<span data-ttu-id="25cc6-128">Время входа в программу.</span><span class="sxs-lookup"><span data-stu-id="25cc6-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="25cc6-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="25cc6-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="25cc6-130">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="25cc6-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="25cc6-131">logonId</span><span class="sxs-lookup"><span data-stu-id="25cc6-131">logonId</span></span>|<span data-ttu-id="25cc6-132">String</span><span class="sxs-lookup"><span data-stu-id="25cc6-132">String</span></span>|<span data-ttu-id="25cc6-133">Идентификатор пользователя входа.</span><span class="sxs-lookup"><span data-stu-id="25cc6-133">User sign-in ID.</span></span>|
|<span data-ttu-id="25cc6-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="25cc6-134">logonIp</span></span>|<span data-ttu-id="25cc6-135">String</span><span class="sxs-lookup"><span data-stu-id="25cc6-135">String</span></span>|<span data-ttu-id="25cc6-136">IP-адрес, запрос на вход исходит от.</span><span class="sxs-lookup"><span data-stu-id="25cc6-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="25cc6-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="25cc6-137">logonLocation</span></span>|<span data-ttu-id="25cc6-138">String</span><span class="sxs-lookup"><span data-stu-id="25cc6-138">String</span></span>|<span data-ttu-id="25cc6-139">Расположение (по сопоставления IP-адреса), связанных с событие вход пользователя с этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="25cc6-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="25cc6-140">logonType</span><span class="sxs-lookup"><span data-stu-id="25cc6-140">logonType</span></span>|<span data-ttu-id="25cc6-141">logonType</span><span class="sxs-lookup"><span data-stu-id="25cc6-141">logonType</span></span>|<span data-ttu-id="25cc6-142">Метод входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="25cc6-142">Method of user sign in.</span></span> <span data-ttu-id="25cc6-143">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="25cc6-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="25cc6-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="25cc6-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="25cc6-145">String</span><span class="sxs-lookup"><span data-stu-id="25cc6-145">String</span></span>|<span data-ttu-id="25cc6-146">Active Directory (локально) идентификатор безопасности (SID) пользователя.</span><span class="sxs-lookup"><span data-stu-id="25cc6-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="25cc6-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="25cc6-147">riskScore</span></span>|<span data-ttu-id="25cc6-148">String</span><span class="sxs-lookup"><span data-stu-id="25cc6-148">String</span></span>|<span data-ttu-id="25cc6-149">Оценка риска поставщика создается/вычисляемые учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="25cc6-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="25cc6-150">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="25cc6-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="25cc6-151">userAccountType</span><span class="sxs-lookup"><span data-stu-id="25cc6-151">userAccountType</span></span>|<span data-ttu-id="25cc6-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="25cc6-152">userAccountSecurityType</span></span>|<span data-ttu-id="25cc6-153">Тип учетной записи (членство в группе) для определения Windows.</span><span class="sxs-lookup"><span data-stu-id="25cc6-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="25cc6-154">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="25cc6-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="25cc6-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="25cc6-155">userPrincipalName</span></span>|<span data-ttu-id="25cc6-156">Строка</span><span class="sxs-lookup"><span data-stu-id="25cc6-156">String</span></span>|<span data-ttu-id="25cc6-157">Учетное имя пользователя - формат для Интернета: (имя учетной записи пользователя) @(имя домена DNS учетной записи пользователя).</span><span class="sxs-lookup"><span data-stu-id="25cc6-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25cc6-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25cc6-158">JSON representation</span></span>

<span data-ttu-id="25cc6-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25cc6-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/usersecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
