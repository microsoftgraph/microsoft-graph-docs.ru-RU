---
title: Тип ресурса userSecurityState
description: Содержит информацию о состояниях об учетной записи пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9f451f2bc42500eee15bd59809c124a79186916f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27992058"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="22bf9-103">Тип ресурса userSecurityState</span><span class="sxs-lookup"><span data-stu-id="22bf9-103">userSecurityState resource type</span></span>

<span data-ttu-id="22bf9-104">Содержит информацию о состояниях об учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="22bf9-104">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="22bf9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="22bf9-105">Properties</span></span>

| <span data-ttu-id="22bf9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="22bf9-106">Property</span></span>   | <span data-ttu-id="22bf9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="22bf9-107">Type</span></span> |<span data-ttu-id="22bf9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="22bf9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22bf9-109">aadUserId</span><span class="sxs-lookup"><span data-stu-id="22bf9-109">aadUserId</span></span>|<span data-ttu-id="22bf9-110">String</span><span class="sxs-lookup"><span data-stu-id="22bf9-110">String</span></span>|<span data-ttu-id="22bf9-111">AAD пользователя объекта идентификатор (GUID) — представляет удостоверение пользователя физических/несколькими-account.</span><span class="sxs-lookup"><span data-stu-id="22bf9-111">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="22bf9-112">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="22bf9-112">accountName</span></span>|<span data-ttu-id="22bf9-113">String</span><span class="sxs-lookup"><span data-stu-id="22bf9-113">String</span></span>|<span data-ttu-id="22bf9-114">Имя учетной записи для учетной записи пользователя (без домена Active Directory и DNS домена) - (также называемая `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="22bf9-114">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="22bf9-115">domainName</span><span class="sxs-lookup"><span data-stu-id="22bf9-115">domainName</span></span>|<span data-ttu-id="22bf9-116">String</span><span class="sxs-lookup"><span data-stu-id="22bf9-116">String</span></span>|<span data-ttu-id="22bf9-117">NetBIOS/Active Directory в домен учетной записи пользователя (то есть, в формате домен\учетная запись).</span><span class="sxs-lookup"><span data-stu-id="22bf9-117">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="22bf9-118">emailRole</span><span class="sxs-lookup"><span data-stu-id="22bf9-118">emailRole</span></span>|<span data-ttu-id="22bf9-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="22bf9-119">emailRole</span></span>|<span data-ttu-id="22bf9-120">Связанные с электронной почты оповещений,-электронной почты для учетной записи пользователя «роли».</span><span class="sxs-lookup"><span data-stu-id="22bf9-120">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="22bf9-121">Возможные значения: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="22bf9-121">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="22bf9-122">isVpn</span><span class="sxs-lookup"><span data-stu-id="22bf9-122">isVpn</span></span>|<span data-ttu-id="22bf9-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="22bf9-123">Boolean</span></span>|<span data-ttu-id="22bf9-124">Указывает, вошел ли пользователь через VPN.</span><span class="sxs-lookup"><span data-stu-id="22bf9-124">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="22bf9-125">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="22bf9-125">logonDateTime</span></span>|<span data-ttu-id="22bf9-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22bf9-126">DateTimeOffset</span></span>|<span data-ttu-id="22bf9-127">Время входа в программу.</span><span class="sxs-lookup"><span data-stu-id="22bf9-127">Time at which the sign-in occurred.</span></span> <span data-ttu-id="22bf9-128">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="22bf9-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="22bf9-129">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="22bf9-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="22bf9-130">logonId</span><span class="sxs-lookup"><span data-stu-id="22bf9-130">logonId</span></span>|<span data-ttu-id="22bf9-131">String</span><span class="sxs-lookup"><span data-stu-id="22bf9-131">String</span></span>|<span data-ttu-id="22bf9-132">Идентификатор пользователя входа.</span><span class="sxs-lookup"><span data-stu-id="22bf9-132">User sign-in ID.</span></span>|
|<span data-ttu-id="22bf9-133">logonIp</span><span class="sxs-lookup"><span data-stu-id="22bf9-133">logonIp</span></span>|<span data-ttu-id="22bf9-134">String</span><span class="sxs-lookup"><span data-stu-id="22bf9-134">String</span></span>|<span data-ttu-id="22bf9-135">IP-адрес, запрос на вход исходит от.</span><span class="sxs-lookup"><span data-stu-id="22bf9-135">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="22bf9-136">logonLocation</span><span class="sxs-lookup"><span data-stu-id="22bf9-136">logonLocation</span></span>|<span data-ttu-id="22bf9-137">String</span><span class="sxs-lookup"><span data-stu-id="22bf9-137">String</span></span>|<span data-ttu-id="22bf9-138">Расположение (по сопоставления IP-адреса), связанных с событие вход пользователя с этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="22bf9-138">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="22bf9-139">logonType</span><span class="sxs-lookup"><span data-stu-id="22bf9-139">logonType</span></span>|<span data-ttu-id="22bf9-140">logonType</span><span class="sxs-lookup"><span data-stu-id="22bf9-140">logonType</span></span>|<span data-ttu-id="22bf9-141">Метод входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="22bf9-141">Method of user sign in.</span></span> <span data-ttu-id="22bf9-142">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="22bf9-142">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="22bf9-143">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="22bf9-143">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="22bf9-144">String</span><span class="sxs-lookup"><span data-stu-id="22bf9-144">String</span></span>|<span data-ttu-id="22bf9-145">Active Directory (локально) идентификатор безопасности (SID) пользователя.</span><span class="sxs-lookup"><span data-stu-id="22bf9-145">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="22bf9-146">riskScore</span><span class="sxs-lookup"><span data-stu-id="22bf9-146">riskScore</span></span>|<span data-ttu-id="22bf9-147">String</span><span class="sxs-lookup"><span data-stu-id="22bf9-147">String</span></span>|<span data-ttu-id="22bf9-148">Оценка риска поставщика создается/вычисляемые учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="22bf9-148">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="22bf9-149">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="22bf9-149">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="22bf9-150">userAccountType</span><span class="sxs-lookup"><span data-stu-id="22bf9-150">userAccountType</span></span>|<span data-ttu-id="22bf9-151">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="22bf9-151">userAccountSecurityType</span></span>|<span data-ttu-id="22bf9-152">Тип учетной записи (членство в группе) для определения Windows.</span><span class="sxs-lookup"><span data-stu-id="22bf9-152">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="22bf9-153">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="22bf9-153">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="22bf9-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="22bf9-154">userPrincipalName</span></span>|<span data-ttu-id="22bf9-155">String</span><span class="sxs-lookup"><span data-stu-id="22bf9-155">String</span></span>|<span data-ttu-id="22bf9-156">Учетное имя пользователя - формат для Интернета: (имя учетной записи пользователя) @(имя домена DNS учетной записи пользователя).</span><span class="sxs-lookup"><span data-stu-id="22bf9-156">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22bf9-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22bf9-157">JSON representation</span></span>

<span data-ttu-id="22bf9-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22bf9-158">The following is a JSON representation of the resource.</span></span>

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
