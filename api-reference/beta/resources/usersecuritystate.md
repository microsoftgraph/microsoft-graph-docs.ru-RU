---
title: тип ресурсов userSecurityState
description: Содержит сведения о учетной записи пользователя.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: c95f898a729138a7af88eaf25fa4cbc0c5fc9bb9
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761783"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="ae8f7-103">тип ресурсов userSecurityState</span><span class="sxs-lookup"><span data-stu-id="ae8f7-103">userSecurityState resource type</span></span>

<span data-ttu-id="ae8f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae8f7-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae8f7-105">Содержит сведения о учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="ae8f7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae8f7-106">Properties</span></span>

| <span data-ttu-id="ae8f7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae8f7-107">Property</span></span>   | <span data-ttu-id="ae8f7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ae8f7-108">Type</span></span> |<span data-ttu-id="ae8f7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ae8f7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae8f7-110">aadUserId</span><span class="sxs-lookup"><span data-stu-id="ae8f7-110">aadUserId</span></span>|<span data-ttu-id="ae8f7-111">String</span><span class="sxs-lookup"><span data-stu-id="ae8f7-111">String</span></span>|<span data-ttu-id="ae8f7-112">Идентификатор объекта пользователя AAD (GUID) — представляет физическое/многосчетное пользовательское лицо.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="ae8f7-113">accountName</span><span class="sxs-lookup"><span data-stu-id="ae8f7-113">accountName</span></span>|<span data-ttu-id="ae8f7-114">String</span><span class="sxs-lookup"><span data-stu-id="ae8f7-114">String</span></span>|<span data-ttu-id="ae8f7-115">Имя учетной записи пользователя (без домена Active Directory или домена DNS) — (также `mailNickName` называемого).</span><span class="sxs-lookup"><span data-stu-id="ae8f7-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="ae8f7-116">domainName</span><span class="sxs-lookup"><span data-stu-id="ae8f7-116">domainName</span></span>|<span data-ttu-id="ae8f7-117">String</span><span class="sxs-lookup"><span data-stu-id="ae8f7-117">String</span></span>|<span data-ttu-id="ae8f7-118">Домен учетной записи пользователя NetBIOS/Active Directory (то есть формат домена\учетной записи).</span><span class="sxs-lookup"><span data-stu-id="ae8f7-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="ae8f7-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="ae8f7-119">emailRole</span></span>|<span data-ttu-id="ae8f7-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="ae8f7-120">emailRole</span></span>|<span data-ttu-id="ae8f7-121">Для оповещений, связанных с электронной почтой, — "роль" учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="ae8f7-122">Возможные значения: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="ae8f7-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="ae8f7-123">isVpn</span></span>|<span data-ttu-id="ae8f7-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae8f7-124">Boolean</span></span>|<span data-ttu-id="ae8f7-125">Указывает, вошел ли пользователь в систему через VPN.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="ae8f7-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="ae8f7-126">logonDateTime</span></span>|<span data-ttu-id="ae8f7-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae8f7-127">DateTimeOffset</span></span>|<span data-ttu-id="ae8f7-128">Время, в которое произошел вход.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="ae8f7-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ae8f7-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ae8f7-130">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-130">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="ae8f7-131">logonId</span><span class="sxs-lookup"><span data-stu-id="ae8f7-131">logonId</span></span>|<span data-ttu-id="ae8f7-132">String</span><span class="sxs-lookup"><span data-stu-id="ae8f7-132">String</span></span>|<span data-ttu-id="ae8f7-133">ID для регистрации пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-133">User sign-in ID.</span></span>|
|<span data-ttu-id="ae8f7-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="ae8f7-134">logonIp</span></span>|<span data-ttu-id="ae8f7-135">String</span><span class="sxs-lookup"><span data-stu-id="ae8f7-135">String</span></span>|<span data-ttu-id="ae8f7-136">IP-адрес запроса на вход возник из.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="ae8f7-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="ae8f7-137">logonLocation</span></span>|<span data-ttu-id="ae8f7-138">String</span><span class="sxs-lookup"><span data-stu-id="ae8f7-138">String</span></span>|<span data-ttu-id="ae8f7-139">Расположение (по сопоставлению IP-адресов), связанное с событием регистрации пользователя этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="ae8f7-140">logonType</span><span class="sxs-lookup"><span data-stu-id="ae8f7-140">logonType</span></span>|<span data-ttu-id="ae8f7-141">logonType</span><span class="sxs-lookup"><span data-stu-id="ae8f7-141">logonType</span></span>|<span data-ttu-id="ae8f7-142">Метод входной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-142">Method of user sign in.</span></span> <span data-ttu-id="ae8f7-143">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="ae8f7-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="ae8f7-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="ae8f7-145">String</span><span class="sxs-lookup"><span data-stu-id="ae8f7-145">String</span></span>|<span data-ttu-id="ae8f7-146">Идентификатор безопасности Active Directory (локально) пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="ae8f7-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="ae8f7-147">riskScore</span></span>|<span data-ttu-id="ae8f7-148">String</span><span class="sxs-lookup"><span data-stu-id="ae8f7-148">String</span></span>|<span data-ttu-id="ae8f7-149">Оценка риска учетной записи пользователя сгенерирована/рассчитана с учетной записью поставщика.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="ae8f7-150">Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="ae8f7-151">userAccountType</span><span class="sxs-lookup"><span data-stu-id="ae8f7-151">userAccountType</span></span>|<span data-ttu-id="ae8f7-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="ae8f7-152">userAccountSecurityType</span></span>|<span data-ttu-id="ae8f7-153">Тип учетной записи пользователя (членство в группе) в определении Windows.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="ae8f7-154">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="ae8f7-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ae8f7-155">userPrincipalName</span></span>|<span data-ttu-id="ae8f7-156">String</span><span class="sxs-lookup"><span data-stu-id="ae8f7-156">String</span></span>|<span data-ttu-id="ae8f7-157">Имя регистрации пользователя — интернет-формат: (имя учетной записи пользователя)@(имя доменного имени учетной записи пользователя DNS).</span><span class="sxs-lookup"><span data-stu-id="ae8f7-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae8f7-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae8f7-158">JSON representation</span></span>

<span data-ttu-id="ae8f7-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae8f7-159">The following is a JSON representation of the resource.</span></span>

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


