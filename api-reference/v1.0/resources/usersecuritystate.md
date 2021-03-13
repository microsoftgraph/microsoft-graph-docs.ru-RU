---
title: тип ресурсов userSecurityState
description: Содержит сведения о учетной записи пользователя.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 10b5043cdadaaa1180e232e0776c26a60f46f507
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759498"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="5bb02-103">тип ресурсов userSecurityState</span><span class="sxs-lookup"><span data-stu-id="5bb02-103">userSecurityState resource type</span></span>

<span data-ttu-id="5bb02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bb02-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5bb02-105">Содержит сведения о учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bb02-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="5bb02-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5bb02-106">Properties</span></span>

| <span data-ttu-id="5bb02-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bb02-107">Property</span></span>   | <span data-ttu-id="5bb02-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5bb02-108">Type</span></span> |<span data-ttu-id="5bb02-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5bb02-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bb02-110">aadUserId</span><span class="sxs-lookup"><span data-stu-id="5bb02-110">aadUserId</span></span>|<span data-ttu-id="5bb02-111">String</span><span class="sxs-lookup"><span data-stu-id="5bb02-111">String</span></span>|<span data-ttu-id="5bb02-112">Идентификатор объекта пользователя AAD (GUID) — представляет физическое/многосчетное пользовательское лицо.</span><span class="sxs-lookup"><span data-stu-id="5bb02-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="5bb02-113">accountName</span><span class="sxs-lookup"><span data-stu-id="5bb02-113">accountName</span></span>|<span data-ttu-id="5bb02-114">String</span><span class="sxs-lookup"><span data-stu-id="5bb02-114">String</span></span>|<span data-ttu-id="5bb02-115">Имя учетной записи пользователя (без домена Active Directory или домена DNS) — (также `mailNickName` называемого).</span><span class="sxs-lookup"><span data-stu-id="5bb02-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="5bb02-116">domainName</span><span class="sxs-lookup"><span data-stu-id="5bb02-116">domainName</span></span>|<span data-ttu-id="5bb02-117">String</span><span class="sxs-lookup"><span data-stu-id="5bb02-117">String</span></span>|<span data-ttu-id="5bb02-118">Домен учетной записи пользователя NetBIOS/Active Directory (то есть формат домена\учетной записи).</span><span class="sxs-lookup"><span data-stu-id="5bb02-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="5bb02-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="5bb02-119">emailRole</span></span>|<span data-ttu-id="5bb02-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="5bb02-120">emailRole</span></span>|<span data-ttu-id="5bb02-121">Для оповещений, связанных с электронной почтой, — "роль" учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bb02-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="5bb02-122">Возможные значения: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="5bb02-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="5bb02-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="5bb02-123">isVpn</span></span>|<span data-ttu-id="5bb02-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bb02-124">Boolean</span></span>|<span data-ttu-id="5bb02-125">Указывает, вошел ли пользователь в систему через VPN.</span><span class="sxs-lookup"><span data-stu-id="5bb02-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="5bb02-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="5bb02-126">logonDateTime</span></span>|<span data-ttu-id="5bb02-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bb02-127">DateTimeOffset</span></span>|<span data-ttu-id="5bb02-128">Время, в которое произошел вход.</span><span class="sxs-lookup"><span data-stu-id="5bb02-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="5bb02-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5bb02-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5bb02-130">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5bb02-130">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="5bb02-131">logonId</span><span class="sxs-lookup"><span data-stu-id="5bb02-131">logonId</span></span>|<span data-ttu-id="5bb02-132">String</span><span class="sxs-lookup"><span data-stu-id="5bb02-132">String</span></span>|<span data-ttu-id="5bb02-133">ID для регистрации пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bb02-133">User sign-in ID.</span></span>|
|<span data-ttu-id="5bb02-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="5bb02-134">logonIp</span></span>|<span data-ttu-id="5bb02-135">String</span><span class="sxs-lookup"><span data-stu-id="5bb02-135">String</span></span>|<span data-ttu-id="5bb02-136">IP-адрес запроса на вход возник из.</span><span class="sxs-lookup"><span data-stu-id="5bb02-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="5bb02-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="5bb02-137">logonLocation</span></span>|<span data-ttu-id="5bb02-138">String</span><span class="sxs-lookup"><span data-stu-id="5bb02-138">String</span></span>|<span data-ttu-id="5bb02-139">Расположение (по сопоставлению IP-адресов), связанное с событием регистрации пользователя этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="5bb02-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="5bb02-140">logonType</span><span class="sxs-lookup"><span data-stu-id="5bb02-140">logonType</span></span>|<span data-ttu-id="5bb02-141">logonType</span><span class="sxs-lookup"><span data-stu-id="5bb02-141">logonType</span></span>|<span data-ttu-id="5bb02-142">Метод входной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bb02-142">Method of user sign in.</span></span> <span data-ttu-id="5bb02-143">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="5bb02-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="5bb02-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="5bb02-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="5bb02-145">String</span><span class="sxs-lookup"><span data-stu-id="5bb02-145">String</span></span>|<span data-ttu-id="5bb02-146">Идентификатор безопасности Active Directory (локально) пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bb02-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="5bb02-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="5bb02-147">riskScore</span></span>|<span data-ttu-id="5bb02-148">String</span><span class="sxs-lookup"><span data-stu-id="5bb02-148">String</span></span>|<span data-ttu-id="5bb02-149">Оценка риска учетной записи пользователя сгенерирована/рассчитана с учетной записью поставщика.</span><span class="sxs-lookup"><span data-stu-id="5bb02-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="5bb02-150">Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.</span><span class="sxs-lookup"><span data-stu-id="5bb02-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="5bb02-151">userAccountType</span><span class="sxs-lookup"><span data-stu-id="5bb02-151">userAccountType</span></span>|<span data-ttu-id="5bb02-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="5bb02-152">userAccountSecurityType</span></span>|<span data-ttu-id="5bb02-153">Тип учетной записи пользователя (членство в группе) в определении Windows.</span><span class="sxs-lookup"><span data-stu-id="5bb02-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="5bb02-154">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="5bb02-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="5bb02-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5bb02-155">userPrincipalName</span></span>|<span data-ttu-id="5bb02-156">String</span><span class="sxs-lookup"><span data-stu-id="5bb02-156">String</span></span>|<span data-ttu-id="5bb02-157">Имя регистрации пользователя — интернет-формат: (имя учетной записи пользователя)@(имя доменного имени учетной записи пользователя DNS).</span><span class="sxs-lookup"><span data-stu-id="5bb02-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5bb02-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5bb02-158">JSON representation</span></span>

<span data-ttu-id="5bb02-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bb02-159">The following is a JSON representation of the resource.</span></span>

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

