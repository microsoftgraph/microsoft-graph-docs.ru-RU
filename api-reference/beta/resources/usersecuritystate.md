---
title: Тип ресурса Усерсекуритистате
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 67e5c7d2feb76346d754f582e34b5afe39af3d32
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519514"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="7e1a7-104">Тип ресурса Усерсекуритистате</span><span class="sxs-lookup"><span data-stu-id="7e1a7-104">userSecurityState resource type</span></span>

<span data-ttu-id="7e1a7-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7e1a7-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e1a7-106">Содержит сведения о состоянии учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-106">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="7e1a7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e1a7-107">Properties</span></span>

| <span data-ttu-id="7e1a7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e1a7-108">Property</span></span>   | <span data-ttu-id="7e1a7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7e1a7-109">Type</span></span> |<span data-ttu-id="7e1a7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7e1a7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e1a7-111">аадусерид</span><span class="sxs-lookup"><span data-stu-id="7e1a7-111">aadUserId</span></span>|<span data-ttu-id="7e1a7-112">String</span><span class="sxs-lookup"><span data-stu-id="7e1a7-112">String</span></span>|<span data-ttu-id="7e1a7-113">Идентификатор объекта пользователя AAD (GUID) — представляет объект пользователя физической или многопользовательской учетной записи.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-113">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="7e1a7-114">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="7e1a7-114">accountName</span></span>|<span data-ttu-id="7e1a7-115">String</span><span class="sxs-lookup"><span data-stu-id="7e1a7-115">String</span></span>|<span data-ttu-id="7e1a7-116">Имя учетной записи пользователя (без домена Active Directory или DNS-домена) (также называется `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="7e1a7-116">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="7e1a7-117">domainName</span><span class="sxs-lookup"><span data-stu-id="7e1a7-117">domainName</span></span>|<span data-ttu-id="7e1a7-118">String</span><span class="sxs-lookup"><span data-stu-id="7e1a7-118">String</span></span>|<span data-ttu-id="7e1a7-119">NetBIOS/Active Directory учетной записи пользователя (то есть формат домен \ пользователь).</span><span class="sxs-lookup"><span data-stu-id="7e1a7-119">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="7e1a7-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="7e1a7-120">emailRole</span></span>|<span data-ttu-id="7e1a7-121">emailRole</span><span class="sxs-lookup"><span data-stu-id="7e1a7-121">emailRole</span></span>|<span data-ttu-id="7e1a7-122">Для оповещений, связанных с электронной почтой: "роль" — Электронная почта учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-122">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="7e1a7-123">Возможные значения: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-123">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="7e1a7-124">исвпн</span><span class="sxs-lookup"><span data-stu-id="7e1a7-124">isVpn</span></span>|<span data-ttu-id="7e1a7-125">Логический</span><span class="sxs-lookup"><span data-stu-id="7e1a7-125">Boolean</span></span>|<span data-ttu-id="7e1a7-126">Указывает, вошел ли пользователь в систему через VPN.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-126">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="7e1a7-127">логондатетиме</span><span class="sxs-lookup"><span data-stu-id="7e1a7-127">logonDateTime</span></span>|<span data-ttu-id="7e1a7-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e1a7-128">DateTimeOffset</span></span>|<span data-ttu-id="7e1a7-129">Время возникновения входа.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-129">Time at which the sign-in occurred.</span></span> <span data-ttu-id="7e1a7-130">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="7e1a7-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7e1a7-131">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7e1a7-132">логонид</span><span class="sxs-lookup"><span data-stu-id="7e1a7-132">logonId</span></span>|<span data-ttu-id="7e1a7-133">String</span><span class="sxs-lookup"><span data-stu-id="7e1a7-133">String</span></span>|<span data-ttu-id="7e1a7-134">Идентификатор входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-134">User sign-in ID.</span></span>|
|<span data-ttu-id="7e1a7-135">logonIp</span><span class="sxs-lookup"><span data-stu-id="7e1a7-135">logonIp</span></span>|<span data-ttu-id="7e1a7-136">String</span><span class="sxs-lookup"><span data-stu-id="7e1a7-136">String</span></span>|<span data-ttu-id="7e1a7-137">IP-адрес, с которого поступил запрос на вход.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-137">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="7e1a7-138">логонлокатион</span><span class="sxs-lookup"><span data-stu-id="7e1a7-138">logonLocation</span></span>|<span data-ttu-id="7e1a7-139">String</span><span class="sxs-lookup"><span data-stu-id="7e1a7-139">String</span></span>|<span data-ttu-id="7e1a7-140">Расположение (по сопоставлению IP-адресов), связанное с событием входа пользователя этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-140">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="7e1a7-141">logonType</span><span class="sxs-lookup"><span data-stu-id="7e1a7-141">logonType</span></span>|<span data-ttu-id="7e1a7-142">logonType</span><span class="sxs-lookup"><span data-stu-id="7e1a7-142">logonType</span></span>|<span data-ttu-id="7e1a7-143">Способ входа пользователя в систему.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-143">Method of user sign in.</span></span> <span data-ttu-id="7e1a7-144">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-144">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="7e1a7-145">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="7e1a7-145">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="7e1a7-146">String</span><span class="sxs-lookup"><span data-stu-id="7e1a7-146">String</span></span>|<span data-ttu-id="7e1a7-147">Идентификатор безопасности (SID) Active Directory (локальный идентификатор) пользователя.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-147">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="7e1a7-148">riskScore</span><span class="sxs-lookup"><span data-stu-id="7e1a7-148">riskScore</span></span>|<span data-ttu-id="7e1a7-149">String</span><span class="sxs-lookup"><span data-stu-id="7e1a7-149">String</span></span>|<span data-ttu-id="7e1a7-150">Рассчитанный поставщиком и вычисляемый показатель риска учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-150">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="7e1a7-151">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-151">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="7e1a7-152">усераккаунттипе</span><span class="sxs-lookup"><span data-stu-id="7e1a7-152">userAccountType</span></span>|<span data-ttu-id="7e1a7-153">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="7e1a7-153">userAccountSecurityType</span></span>|<span data-ttu-id="7e1a7-154">Тип учетной записи пользователя (членство в группе), определение Windows.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-154">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="7e1a7-155">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-155">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="7e1a7-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7e1a7-156">userPrincipalName</span></span>|<span data-ttu-id="7e1a7-157">String</span><span class="sxs-lookup"><span data-stu-id="7e1a7-157">String</span></span>|<span data-ttu-id="7e1a7-158">Имя пользователя для входа в Интернет: (имя учетной записи пользователя) @ (DNS-имя домена учетной записи пользователя).</span><span class="sxs-lookup"><span data-stu-id="7e1a7-158">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e1a7-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e1a7-159">JSON representation</span></span>

<span data-ttu-id="7e1a7-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e1a7-160">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
