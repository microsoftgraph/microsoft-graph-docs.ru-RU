---
title: Тип ресурса userSecurityState
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: f530ac1a657b4049c17bdcdd40f1dd5ea734f278
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078499"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="adac0-104">Тип ресурса userSecurityState</span><span class="sxs-lookup"><span data-stu-id="adac0-104">userSecurityState resource type</span></span>

 > <span data-ttu-id="adac0-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="adac0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adac0-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adac0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="adac0-107">Содержит информацию о состояниях об учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="adac0-107">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="adac0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="adac0-108">Properties</span></span>

| <span data-ttu-id="adac0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="adac0-109">Property</span></span>   | <span data-ttu-id="adac0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="adac0-110">Type</span></span> |<span data-ttu-id="adac0-111">Description</span><span class="sxs-lookup"><span data-stu-id="adac0-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adac0-112">aadUserId</span><span class="sxs-lookup"><span data-stu-id="adac0-112">aadUserId</span></span>|<span data-ttu-id="adac0-113">String</span><span class="sxs-lookup"><span data-stu-id="adac0-113">String</span></span>|<span data-ttu-id="adac0-114">AAD пользователя объекта идентификатор (GUID) — представляет удостоверение пользователя физических/несколькими-account.</span><span class="sxs-lookup"><span data-stu-id="adac0-114">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="adac0-115">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="adac0-115">accountName</span></span>|<span data-ttu-id="adac0-116">String</span><span class="sxs-lookup"><span data-stu-id="adac0-116">String</span></span>|<span data-ttu-id="adac0-117">Имя учетной записи для учетной записи пользователя (без домена Active Directory и DNS домена) - (также называемая `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="adac0-117">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="adac0-118">domainName</span><span class="sxs-lookup"><span data-stu-id="adac0-118">domainName</span></span>|<span data-ttu-id="adac0-119">String</span><span class="sxs-lookup"><span data-stu-id="adac0-119">String</span></span>|<span data-ttu-id="adac0-120">NetBIOS/Active Directory в домен учетной записи пользователя (то есть, в формате домен\учетная запись).</span><span class="sxs-lookup"><span data-stu-id="adac0-120">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="adac0-121">emailRole</span><span class="sxs-lookup"><span data-stu-id="adac0-121">emailRole</span></span>|<span data-ttu-id="adac0-122">emailRole</span><span class="sxs-lookup"><span data-stu-id="adac0-122">emailRole</span></span>|<span data-ttu-id="adac0-123">Связанные с электронной почты оповещений,-электронной почты для учетной записи пользователя «роли».</span><span class="sxs-lookup"><span data-stu-id="adac0-123">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="adac0-124">Возможные значения: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="adac0-124">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="adac0-125">isVpn</span><span class="sxs-lookup"><span data-stu-id="adac0-125">isVpn</span></span>|<span data-ttu-id="adac0-126">Логический</span><span class="sxs-lookup"><span data-stu-id="adac0-126">Boolean</span></span>|<span data-ttu-id="adac0-127">Указывает, вошел ли пользователь через VPN.</span><span class="sxs-lookup"><span data-stu-id="adac0-127">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="adac0-128">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="adac0-128">logonDateTime</span></span>|<span data-ttu-id="adac0-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adac0-129">DateTimeOffset</span></span>|<span data-ttu-id="adac0-130">Время входа в программу.</span><span class="sxs-lookup"><span data-stu-id="adac0-130">Time at which the sign-in occurred.</span></span> <span data-ttu-id="adac0-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="adac0-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="adac0-132">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="adac0-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="adac0-133">logonId</span><span class="sxs-lookup"><span data-stu-id="adac0-133">logonId</span></span>|<span data-ttu-id="adac0-134">String</span><span class="sxs-lookup"><span data-stu-id="adac0-134">String</span></span>|<span data-ttu-id="adac0-135">Идентификатор пользователя входа.</span><span class="sxs-lookup"><span data-stu-id="adac0-135">User sign-in ID.</span></span>|
|<span data-ttu-id="adac0-136">logonIp</span><span class="sxs-lookup"><span data-stu-id="adac0-136">logonIp</span></span>|<span data-ttu-id="adac0-137">String</span><span class="sxs-lookup"><span data-stu-id="adac0-137">String</span></span>|<span data-ttu-id="adac0-138">IP-адрес, запрос на вход исходит от.</span><span class="sxs-lookup"><span data-stu-id="adac0-138">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="adac0-139">logonLocation</span><span class="sxs-lookup"><span data-stu-id="adac0-139">logonLocation</span></span>|<span data-ttu-id="adac0-140">String</span><span class="sxs-lookup"><span data-stu-id="adac0-140">String</span></span>|<span data-ttu-id="adac0-141">Расположение (по сопоставления IP-адреса), связанных с событие вход пользователя с этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="adac0-141">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="adac0-142">logonType</span><span class="sxs-lookup"><span data-stu-id="adac0-142">logonType</span></span>|<span data-ttu-id="adac0-143">logonType</span><span class="sxs-lookup"><span data-stu-id="adac0-143">logonType</span></span>|<span data-ttu-id="adac0-144">Метод входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="adac0-144">Method of user sign in.</span></span> <span data-ttu-id="adac0-145">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="adac0-145">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="adac0-146">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="adac0-146">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="adac0-147">String</span><span class="sxs-lookup"><span data-stu-id="adac0-147">String</span></span>|<span data-ttu-id="adac0-148">Active Directory (локально) идентификатор безопасности (SID) пользователя.</span><span class="sxs-lookup"><span data-stu-id="adac0-148">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="adac0-149">riskScore</span><span class="sxs-lookup"><span data-stu-id="adac0-149">riskScore</span></span>|<span data-ttu-id="adac0-150">String</span><span class="sxs-lookup"><span data-stu-id="adac0-150">String</span></span>|<span data-ttu-id="adac0-151">Оценка риска поставщика создается/вычисляемые учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="adac0-151">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="adac0-152">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="adac0-152">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="adac0-153">userAccountType</span><span class="sxs-lookup"><span data-stu-id="adac0-153">userAccountType</span></span>|<span data-ttu-id="adac0-154">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="adac0-154">userAccountSecurityType</span></span>|<span data-ttu-id="adac0-155">Тип учетной записи (членство в группе) для определения Windows.</span><span class="sxs-lookup"><span data-stu-id="adac0-155">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="adac0-156">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="adac0-156">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="adac0-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="adac0-157">userPrincipalName</span></span>|<span data-ttu-id="adac0-158">String</span><span class="sxs-lookup"><span data-stu-id="adac0-158">String</span></span>|<span data-ttu-id="adac0-159">Учетное имя пользователя - формат для Интернета: (имя учетной записи пользователя) @(имя домена DNS учетной записи пользователя).</span><span class="sxs-lookup"><span data-stu-id="adac0-159">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="adac0-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="adac0-160">JSON representation</span></span>

<span data-ttu-id="adac0-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adac0-161">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
