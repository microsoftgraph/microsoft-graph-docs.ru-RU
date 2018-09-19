# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="979df-101">тип ресурса userSecurityState</span><span class="sxs-lookup"><span data-stu-id="979df-101">userSecurityState resource type</span></span>

<span data-ttu-id="979df-102">Содержит информацию о состоянии учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="979df-102">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="979df-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="979df-103">Properties</span></span>

| <span data-ttu-id="979df-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="979df-104">Property</span></span>   | <span data-ttu-id="979df-105">Тип</span><span class="sxs-lookup"><span data-stu-id="979df-105">Type</span></span> |<span data-ttu-id="979df-106">Описание</span><span class="sxs-lookup"><span data-stu-id="979df-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="979df-107">aadUserId</span><span class="sxs-lookup"><span data-stu-id="979df-107">aadUserId</span></span>|<span data-ttu-id="979df-108">Строка</span><span class="sxs-lookup"><span data-stu-id="979df-108">String</span></span>|<span data-ttu-id="979df-109">Идентификатор объекта AAD User  (GUID) — представляет физическую сущность / пользователя с несколькими учетными записями.</span><span class="sxs-lookup"><span data-stu-id="979df-109">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="979df-110">accountName</span><span class="sxs-lookup"><span data-stu-id="979df-110">accountName</span></span>|<span data-ttu-id="979df-111">Строка</span><span class="sxs-lookup"><span data-stu-id="979df-111">String</span></span>|<span data-ttu-id="979df-112">Имя учетной записи пользователя (без домена Active Directory или домена DNS) – (также называемое `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="979df-112">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="979df-113">domainName</span><span class="sxs-lookup"><span data-stu-id="979df-113">domainName</span></span>|<span data-ttu-id="979df-114">Строка</span><span class="sxs-lookup"><span data-stu-id="979df-114">String</span></span>|<span data-ttu-id="979df-115">Домен учетной записи пользователя NetBIOS/Active Directory (в формате домен\учетная запись).</span><span class="sxs-lookup"><span data-stu-id="979df-115">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="979df-116">emailRole</span><span class="sxs-lookup"><span data-stu-id="979df-116">emailRole</span></span>|<span data-ttu-id="979df-117">emailRole</span><span class="sxs-lookup"><span data-stu-id="979df-117">emailRole</span></span>|<span data-ttu-id="979df-118">Для оповещений, связанных с электронной почтой, – «роль» электронной почты пользовательской учетной записи.</span><span class="sxs-lookup"><span data-stu-id="979df-118">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="979df-119">Возможные значения: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="979df-119">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="979df-120">isVpn</span><span class="sxs-lookup"><span data-stu-id="979df-120">isVpn</span></span>|<span data-ttu-id="979df-121">Логический</span><span class="sxs-lookup"><span data-stu-id="979df-121">Boolean</span></span>|<span data-ttu-id="979df-122">Указывает, вошел ли пользователь в систему через VPN.</span><span class="sxs-lookup"><span data-stu-id="979df-122">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="979df-123">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="979df-123">logonDateTime</span></span>|<span data-ttu-id="979df-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="979df-124">DateTimeOffset</span></span>|<span data-ttu-id="979df-125">Время входа в программу.</span><span class="sxs-lookup"><span data-stu-id="979df-125">Time at which the sign-in occurred.</span></span> <span data-ttu-id="979df-126">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="979df-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="979df-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="979df-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="979df-128">logonId</span><span class="sxs-lookup"><span data-stu-id="979df-128">logonId</span></span>|<span data-ttu-id="979df-129">Строка</span><span class="sxs-lookup"><span data-stu-id="979df-129">String</span></span>|<span data-ttu-id="979df-130">Идентификатор входа пользователя в программу.</span><span class="sxs-lookup"><span data-stu-id="979df-130">User sign-in ID.</span></span>|
|<span data-ttu-id="979df-131">logonIp</span><span class="sxs-lookup"><span data-stu-id="979df-131">logonIp</span></span>|<span data-ttu-id="979df-132">Строка</span><span class="sxs-lookup"><span data-stu-id="979df-132">String</span></span>|<span data-ttu-id="979df-133">IP-адрес, с которого поступил запрос на вход в программу.</span><span class="sxs-lookup"><span data-stu-id="979df-133">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="979df-134">logonLocation</span><span class="sxs-lookup"><span data-stu-id="979df-134">logonLocation</span></span>|<span data-ttu-id="979df-135">Строка</span><span class="sxs-lookup"><span data-stu-id="979df-135">String</span></span>|<span data-ttu-id="979df-136">Местоположение (определяемое по IP-адресу), связанное с событием входа в программу этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="979df-136">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="979df-137">logonType</span><span class="sxs-lookup"><span data-stu-id="979df-137">logonType</span></span>|<span data-ttu-id="979df-138">logonType</span><span class="sxs-lookup"><span data-stu-id="979df-138">logonType</span></span>|<span data-ttu-id="979df-139">Способ входа пользователя в программу.</span><span class="sxs-lookup"><span data-stu-id="979df-139">Method of user sign in.</span></span> <span data-ttu-id="979df-140">Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="979df-140">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="979df-141">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="979df-141">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="979df-142">Строка</span><span class="sxs-lookup"><span data-stu-id="979df-142">String</span></span>|<span data-ttu-id="979df-143"> SID пользователя – локальный идентификатор безопасности в Active Directory.</span><span class="sxs-lookup"><span data-stu-id="979df-143">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="979df-144">riskScore</span><span class="sxs-lookup"><span data-stu-id="979df-144">riskScore</span></span>|<span data-ttu-id="979df-145">Строка</span><span class="sxs-lookup"><span data-stu-id="979df-145">String</span></span>|<span data-ttu-id="979df-146">Указанная поставщиком / рассчитанная оценка рисков для учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="979df-146">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="979df-147">Рекомендуемый диапазон значений: от 0 до 1, что соответствует величине в процентах.</span><span class="sxs-lookup"><span data-stu-id="979df-147">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="979df-148">userAccountType</span><span class="sxs-lookup"><span data-stu-id="979df-148">userAccountType</span></span>|<span data-ttu-id="979df-149">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="979df-149">userAccountSecurityType</span></span>|<span data-ttu-id="979df-150">Тип учетной записи (членство в группе), согласно определению, принятому в Windows.</span><span class="sxs-lookup"><span data-stu-id="979df-150">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="979df-151">Возможные значения: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="979df-151">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="979df-152">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="979df-152">userPrincipalName</span></span>|<span data-ttu-id="979df-153">Строка</span><span class="sxs-lookup"><span data-stu-id="979df-153">String</span></span>|<span data-ttu-id="979df-154">Учетное имя пользователя - формат для Интернета: (имя учетной записи пользователя)@(имя домена DNS учетной записи пользователя).</span><span class="sxs-lookup"><span data-stu-id="979df-154">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="979df-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="979df-155">JSON representation</span></span>

<span data-ttu-id="979df-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="979df-156">The following is a JSON representation of the resource.</span></span>

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
