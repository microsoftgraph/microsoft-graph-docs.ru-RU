---
title: Тип ресурса Усерсекуритистате
description: Содержит сведения о состоянии учетной записи пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9f451f2bc42500eee15bd59809c124a79186916f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463812"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="e960a-103">Тип ресурса Усерсекуритистате</span><span class="sxs-lookup"><span data-stu-id="e960a-103">userSecurityState resource type</span></span>

<span data-ttu-id="e960a-104">Содержит сведения о состоянии учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="e960a-104">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="e960a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e960a-105">Properties</span></span>

| <span data-ttu-id="e960a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e960a-106">Property</span></span>   | <span data-ttu-id="e960a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e960a-107">Type</span></span> |<span data-ttu-id="e960a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e960a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e960a-109">Аадусерид</span><span class="sxs-lookup"><span data-stu-id="e960a-109">aadUserId</span></span>|<span data-ttu-id="e960a-110">String</span><span class="sxs-lookup"><span data-stu-id="e960a-110">String</span></span>|<span data-ttu-id="e960a-111">Идентификатор объекта пользователя AAD (GUID) — представляет объект пользователя физической или многопользовательской учетной записи.</span><span class="sxs-lookup"><span data-stu-id="e960a-111">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="e960a-112">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="e960a-112">accountName</span></span>|<span data-ttu-id="e960a-113">String</span><span class="sxs-lookup"><span data-stu-id="e960a-113">String</span></span>|<span data-ttu-id="e960a-114">Имя учетной записи пользователя (без домена Active Directory или DNS-домена) (также называется `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="e960a-114">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="e960a-115">domainName</span><span class="sxs-lookup"><span data-stu-id="e960a-115">domainName</span></span>|<span data-ttu-id="e960a-116">String</span><span class="sxs-lookup"><span data-stu-id="e960a-116">String</span></span>|<span data-ttu-id="e960a-117">NetBIOS/Active Directory учетной записи пользователя (то есть формат домен \ пользователь).</span><span class="sxs-lookup"><span data-stu-id="e960a-117">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="e960a-118">emailRole</span><span class="sxs-lookup"><span data-stu-id="e960a-118">emailRole</span></span>|<span data-ttu-id="e960a-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="e960a-119">emailRole</span></span>|<span data-ttu-id="e960a-120">Для оповещений, связанных с электронной почтой: "роль" — Электронная почта учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="e960a-120">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="e960a-121">Возможные значения: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="e960a-121">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="e960a-122">Исвпн</span><span class="sxs-lookup"><span data-stu-id="e960a-122">isVpn</span></span>|<span data-ttu-id="e960a-123">Логический</span><span class="sxs-lookup"><span data-stu-id="e960a-123">Boolean</span></span>|<span data-ttu-id="e960a-124">Указывает, вошел ли пользователь в систему через VPN.</span><span class="sxs-lookup"><span data-stu-id="e960a-124">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="e960a-125">Логондатетиме</span><span class="sxs-lookup"><span data-stu-id="e960a-125">logonDateTime</span></span>|<span data-ttu-id="e960a-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e960a-126">DateTimeOffset</span></span>|<span data-ttu-id="e960a-127">Время возникновения входа.</span><span class="sxs-lookup"><span data-stu-id="e960a-127">Time at which the sign-in occurred.</span></span> <span data-ttu-id="e960a-128">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e960a-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e960a-129">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e960a-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e960a-130">Логонид</span><span class="sxs-lookup"><span data-stu-id="e960a-130">logonId</span></span>|<span data-ttu-id="e960a-131">String</span><span class="sxs-lookup"><span data-stu-id="e960a-131">String</span></span>|<span data-ttu-id="e960a-132">Идентификатор входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="e960a-132">User sign-in ID.</span></span>|
|<span data-ttu-id="e960a-133">logonIp</span><span class="sxs-lookup"><span data-stu-id="e960a-133">logonIp</span></span>|<span data-ttu-id="e960a-134">String</span><span class="sxs-lookup"><span data-stu-id="e960a-134">String</span></span>|<span data-ttu-id="e960a-135">IP-адрес, с которого поступил запрос на вход.</span><span class="sxs-lookup"><span data-stu-id="e960a-135">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="e960a-136">Логонлокатион</span><span class="sxs-lookup"><span data-stu-id="e960a-136">logonLocation</span></span>|<span data-ttu-id="e960a-137">String</span><span class="sxs-lookup"><span data-stu-id="e960a-137">String</span></span>|<span data-ttu-id="e960a-138">Расположение (по сопоставлению IP-адресов), связанное с событием входа пользователя этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="e960a-138">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="e960a-139">logonType</span><span class="sxs-lookup"><span data-stu-id="e960a-139">logonType</span></span>|<span data-ttu-id="e960a-140">logonType</span><span class="sxs-lookup"><span data-stu-id="e960a-140">logonType</span></span>|<span data-ttu-id="e960a-141">Способ входа пользователя в систему.</span><span class="sxs-lookup"><span data-stu-id="e960a-141">Method of user sign in.</span></span> <span data-ttu-id="e960a-142">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="e960a-142">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="e960a-143">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="e960a-143">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="e960a-144">String</span><span class="sxs-lookup"><span data-stu-id="e960a-144">String</span></span>|<span data-ttu-id="e960a-145">Идентификатор безопасности (SID) Active Directory (локальный идентификатор) пользователя.</span><span class="sxs-lookup"><span data-stu-id="e960a-145">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="e960a-146">riskScore</span><span class="sxs-lookup"><span data-stu-id="e960a-146">riskScore</span></span>|<span data-ttu-id="e960a-147">String</span><span class="sxs-lookup"><span data-stu-id="e960a-147">String</span></span>|<span data-ttu-id="e960a-148">Рассчитанный поставщиком и вычисляемый показатель риска учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="e960a-148">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="e960a-149">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="e960a-149">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="e960a-150">Усераккаунттипе</span><span class="sxs-lookup"><span data-stu-id="e960a-150">userAccountType</span></span>|<span data-ttu-id="e960a-151">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="e960a-151">userAccountSecurityType</span></span>|<span data-ttu-id="e960a-152">Тип учетной записи пользователя (членство в группе), определение Windows.</span><span class="sxs-lookup"><span data-stu-id="e960a-152">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="e960a-153">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="e960a-153">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="e960a-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e960a-154">userPrincipalName</span></span>|<span data-ttu-id="e960a-155">String</span><span class="sxs-lookup"><span data-stu-id="e960a-155">String</span></span>|<span data-ttu-id="e960a-156">Имя пользователя для входа в Интернет: (имя учетной записи пользователя) @ (DNS-имя домена учетной записи пользователя).</span><span class="sxs-lookup"><span data-stu-id="e960a-156">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e960a-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e960a-157">JSON representation</span></span>

<span data-ttu-id="e960a-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e960a-158">The following is a JSON representation of the resource.</span></span>

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
