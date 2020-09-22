---
title: Тип ресурса Усерсекуритистате
description: Содержит сведения о состоянии учетной записи пользователя.
localization_priority: Normal
author: krbain
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 55c7a55678f4120a7e3c1755a599fcde36ffcd5c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057817"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="b9ae4-103">Тип ресурса Усерсекуритистате</span><span class="sxs-lookup"><span data-stu-id="b9ae4-103">userSecurityState resource type</span></span>

<span data-ttu-id="b9ae4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9ae4-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9ae4-105">Содержит сведения о состоянии учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="b9ae4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9ae4-106">Properties</span></span>

| <span data-ttu-id="b9ae4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9ae4-107">Property</span></span>   | <span data-ttu-id="b9ae4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b9ae4-108">Type</span></span> |<span data-ttu-id="b9ae4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b9ae4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9ae4-110">аадусерид</span><span class="sxs-lookup"><span data-stu-id="b9ae4-110">aadUserId</span></span>|<span data-ttu-id="b9ae4-111">String</span><span class="sxs-lookup"><span data-stu-id="b9ae4-111">String</span></span>|<span data-ttu-id="b9ae4-112">Идентификатор объекта пользователя AAD (GUID) — представляет объект пользователя физической или многопользовательской учетной записи.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="b9ae4-113">accountName</span><span class="sxs-lookup"><span data-stu-id="b9ae4-113">accountName</span></span>|<span data-ttu-id="b9ae4-114">String</span><span class="sxs-lookup"><span data-stu-id="b9ae4-114">String</span></span>|<span data-ttu-id="b9ae4-115">Имя учетной записи пользователя (без домена Active Directory или DNS-домена) (также называется `mailNickName` ).</span><span class="sxs-lookup"><span data-stu-id="b9ae4-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="b9ae4-116">domainName</span><span class="sxs-lookup"><span data-stu-id="b9ae4-116">domainName</span></span>|<span data-ttu-id="b9ae4-117">String</span><span class="sxs-lookup"><span data-stu-id="b9ae4-117">String</span></span>|<span data-ttu-id="b9ae4-118">NetBIOS/Active Directory учетной записи пользователя (то есть формат домен \ пользователь).</span><span class="sxs-lookup"><span data-stu-id="b9ae4-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="b9ae4-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="b9ae4-119">emailRole</span></span>|<span data-ttu-id="b9ae4-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="b9ae4-120">emailRole</span></span>|<span data-ttu-id="b9ae4-121">Для оповещений, связанных с электронной почтой: "роль" — Электронная почта учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="b9ae4-122">Возможные значения: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="b9ae4-123">исвпн</span><span class="sxs-lookup"><span data-stu-id="b9ae4-123">isVpn</span></span>|<span data-ttu-id="b9ae4-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9ae4-124">Boolean</span></span>|<span data-ttu-id="b9ae4-125">Указывает, вошел ли пользователь в систему через VPN.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="b9ae4-126">логондатетиме</span><span class="sxs-lookup"><span data-stu-id="b9ae4-126">logonDateTime</span></span>|<span data-ttu-id="b9ae4-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9ae4-127">DateTimeOffset</span></span>|<span data-ttu-id="b9ae4-128">Время возникновения входа.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="b9ae4-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b9ae4-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b9ae4-130">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="b9ae4-131">логонид</span><span class="sxs-lookup"><span data-stu-id="b9ae4-131">logonId</span></span>|<span data-ttu-id="b9ae4-132">String</span><span class="sxs-lookup"><span data-stu-id="b9ae4-132">String</span></span>|<span data-ttu-id="b9ae4-133">Идентификатор входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-133">User sign-in ID.</span></span>|
|<span data-ttu-id="b9ae4-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="b9ae4-134">logonIp</span></span>|<span data-ttu-id="b9ae4-135">String</span><span class="sxs-lookup"><span data-stu-id="b9ae4-135">String</span></span>|<span data-ttu-id="b9ae4-136">IP-адрес, с которого поступил запрос на вход.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="b9ae4-137">логонлокатион</span><span class="sxs-lookup"><span data-stu-id="b9ae4-137">logonLocation</span></span>|<span data-ttu-id="b9ae4-138">String</span><span class="sxs-lookup"><span data-stu-id="b9ae4-138">String</span></span>|<span data-ttu-id="b9ae4-139">Расположение (по сопоставлению IP-адресов), связанное с событием входа пользователя этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="b9ae4-140">logonType</span><span class="sxs-lookup"><span data-stu-id="b9ae4-140">logonType</span></span>|<span data-ttu-id="b9ae4-141">logonType</span><span class="sxs-lookup"><span data-stu-id="b9ae4-141">logonType</span></span>|<span data-ttu-id="b9ae4-142">Способ входа пользователя в систему.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-142">Method of user sign in.</span></span> <span data-ttu-id="b9ae4-143">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="b9ae4-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="b9ae4-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="b9ae4-145">String</span><span class="sxs-lookup"><span data-stu-id="b9ae4-145">String</span></span>|<span data-ttu-id="b9ae4-146">Идентификатор безопасности (SID) Active Directory (локальный идентификатор) пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="b9ae4-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="b9ae4-147">riskScore</span></span>|<span data-ttu-id="b9ae4-148">String</span><span class="sxs-lookup"><span data-stu-id="b9ae4-148">String</span></span>|<span data-ttu-id="b9ae4-149">Рассчитанный поставщиком и вычисляемый показатель риска учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="b9ae4-150">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="b9ae4-151">усераккаунттипе</span><span class="sxs-lookup"><span data-stu-id="b9ae4-151">userAccountType</span></span>|<span data-ttu-id="b9ae4-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="b9ae4-152">userAccountSecurityType</span></span>|<span data-ttu-id="b9ae4-153">Тип учетной записи пользователя (членство в группе), определение Windows.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="b9ae4-154">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="b9ae4-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9ae4-155">userPrincipalName</span></span>|<span data-ttu-id="b9ae4-156">String</span><span class="sxs-lookup"><span data-stu-id="b9ae4-156">String</span></span>|<span data-ttu-id="b9ae4-157">Имя пользователя для входа в Интернет: (имя учетной записи пользователя) @ (DNS-имя домена учетной записи пользователя).</span><span class="sxs-lookup"><span data-stu-id="b9ae4-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9ae4-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b9ae4-158">JSON representation</span></span>

<span data-ttu-id="b9ae4-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9ae4-159">The following is a JSON representation of the resource.</span></span>

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


