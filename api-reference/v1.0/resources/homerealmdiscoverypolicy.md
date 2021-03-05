---
title: тип ресурса homeRealmDiscoveryPolicy
description: Представляет политику управления поведением проверки подлинности Azure Active Directory для федерационных пользователей.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 78fee8908291619a819b1d62108d149c39b0ae68
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444415"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="b22b8-103">тип ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b22b8-103">homeRealmDiscoveryPolicy resource type</span></span>

<span data-ttu-id="b22b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b22b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b22b8-105">Представляет политику управления поведением проверки подлинности Azure Active Directory для федерационных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федерадных доменах.</span><span class="sxs-lookup"><span data-stu-id="b22b8-105">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="b22b8-106">Вы можете установить **homeRealmDiscoveryPolicy** для всех директоров служб в вашей организации или для определенных директоров служб в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="b22b8-106">You can set **homeRealmDiscoveryPolicy** for all service principals in your organization, or for specific service principals in your organization.</span></span> <span data-ttu-id="b22b8-107">Дополнительные сведения о сценарии и политике см. в материале Настройка входа [Azure AD](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) в поведение приложения с помощью политики обнаружения домашней области, а также входа в [Azure Active Directory](/azure/active-directory/authentication/howto-authentication-use-email-signin)с помощью электронной почты в качестве альтернативного входа.</span><span class="sxs-lookup"><span data-stu-id="b22b8-107">For more scenario and policy details, see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) as well as [Sign-in to Azure Active Directory using email as an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span>

<span data-ttu-id="b22b8-108">Наследует [от stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b22b8-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b22b8-109">Методы</span><span class="sxs-lookup"><span data-stu-id="b22b8-109">Methods</span></span>

| <span data-ttu-id="b22b8-110">Метод</span><span class="sxs-lookup"><span data-stu-id="b22b8-110">Method</span></span>       | <span data-ttu-id="b22b8-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b22b8-111">Return Type</span></span> | <span data-ttu-id="b22b8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b22b8-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b22b8-113">Перечисление типов ресурсов homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b22b8-113">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="b22b8-114">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b22b8-114">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="b22b8-115">Чтение свойств и связей объектов homeRealmDiscoveryPolicies.</span><span class="sxs-lookup"><span data-stu-id="b22b8-115">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="b22b8-116">Создание homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b22b8-116">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="b22b8-117">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b22b8-117">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="b22b8-118">Создание объекта homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="b22b8-118">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="b22b8-119">Get homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b22b8-119">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="b22b8-120">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b22b8-120">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="b22b8-121">Чтение свойств и отношений объекта homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="b22b8-121">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="b22b8-122">Обновление homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b22b8-122">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="b22b8-123">Нет</span><span class="sxs-lookup"><span data-stu-id="b22b8-123">None</span></span> | <span data-ttu-id="b22b8-124">Обновление объекта homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="b22b8-124">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="b22b8-125">Удаление homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b22b8-125">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="b22b8-126">Нет</span><span class="sxs-lookup"><span data-stu-id="b22b8-126">None</span></span> | <span data-ttu-id="b22b8-127">Удаление объекта homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="b22b8-127">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="b22b8-128">Список применяетсяTo</span><span class="sxs-lookup"><span data-stu-id="b22b8-128">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="b22b8-129">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="b22b8-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="b22b8-130">Получите список directoryObjects, к которые была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="b22b8-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="b22b8-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="b22b8-131">Properties</span></span>

| <span data-ttu-id="b22b8-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="b22b8-132">Property</span></span>     | <span data-ttu-id="b22b8-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b22b8-133">Type</span></span>        | <span data-ttu-id="b22b8-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b22b8-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b22b8-135">id</span><span class="sxs-lookup"><span data-stu-id="b22b8-135">id</span></span>|<span data-ttu-id="b22b8-136">String</span><span class="sxs-lookup"><span data-stu-id="b22b8-136">String</span></span>| <span data-ttu-id="b22b8-137">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b22b8-137">Unique identifier for this policy.</span></span> <span data-ttu-id="b22b8-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b22b8-138">Read-only.</span></span>|
|<span data-ttu-id="b22b8-139">определение</span><span class="sxs-lookup"><span data-stu-id="b22b8-139">definition</span></span>|<span data-ttu-id="b22b8-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b22b8-140">String collection</span></span>| <span data-ttu-id="b22b8-141">Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики.</span><span class="sxs-lookup"><span data-stu-id="b22b8-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="b22b8-142">Дополнительные сведения о схеме JSON для этого свойства см. ниже.</span><span class="sxs-lookup"><span data-stu-id="b22b8-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="b22b8-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b22b8-143">Required.</span></span>|
|<span data-ttu-id="b22b8-144">description</span><span class="sxs-lookup"><span data-stu-id="b22b8-144">description</span></span>|<span data-ttu-id="b22b8-145">String</span><span class="sxs-lookup"><span data-stu-id="b22b8-145">String</span></span>| <span data-ttu-id="b22b8-146">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="b22b8-146">Description for this policy.</span></span>|
|<span data-ttu-id="b22b8-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b22b8-147">displayName</span></span>|<span data-ttu-id="b22b8-148">String</span><span class="sxs-lookup"><span data-stu-id="b22b8-148">String</span></span>| <span data-ttu-id="b22b8-149">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b22b8-149">Display name for this policy.</span></span> <span data-ttu-id="b22b8-150">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b22b8-150">Required.</span></span>|
|<span data-ttu-id="b22b8-151">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="b22b8-151">isOrganizationDefault</span></span>|<span data-ttu-id="b22b8-152">Логический</span><span class="sxs-lookup"><span data-stu-id="b22b8-152">Boolean</span></span>|<span data-ttu-id="b22b8-153">Если заданной для true, активирует эту политику.</span><span class="sxs-lookup"><span data-stu-id="b22b8-153">If set to true, activates this policy.</span></span> <span data-ttu-id="b22b8-154">Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации.</span><span class="sxs-lookup"><span data-stu-id="b22b8-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="b22b8-155">Необязательный, значение по умолчанию является ложным.</span><span class="sxs-lookup"><span data-stu-id="b22b8-155">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="b22b8-156">Свойства определения политики обнаружения домашней области</span><span class="sxs-lookup"><span data-stu-id="b22b8-156">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="b22b8-157">Свойства, представленные ниже, формируют объект JSON, который представляет политику срока службы маркера.</span><span class="sxs-lookup"><span data-stu-id="b22b8-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="b22b8-158">Этот объект JSON необходимо **преобразовать** в строку с кавычками, которые будут вставлены в **свойство определения.**</span><span class="sxs-lookup"><span data-stu-id="b22b8-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="b22b8-159">Пример показан ниже в формате JSON:</span><span class="sxs-lookup"><span data-stu-id="b22b8-159">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"HomeRealmDiscoveryPolicy\":
     {\"AccelerateToFederatedDomain\":true,
      \"PreferredDomain\":\"federated.example.edu\",
      \"AlternateIdLogin\":{\"Enabled\":true}}}"
  ]
```

| <span data-ttu-id="b22b8-160">Свойство</span><span class="sxs-lookup"><span data-stu-id="b22b8-160">Property</span></span>     | <span data-ttu-id="b22b8-161">Тип</span><span class="sxs-lookup"><span data-stu-id="b22b8-161">Type</span></span>   |<span data-ttu-id="b22b8-162">Описание</span><span class="sxs-lookup"><span data-stu-id="b22b8-162">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="b22b8-163">AccelerateToFederatedDomain</span><span class="sxs-lookup"><span data-stu-id="b22b8-163">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="b22b8-164">Логический</span><span class="sxs-lookup"><span data-stu-id="b22b8-164">Boolean</span></span>| <span data-ttu-id="b22b8-165">Настройка для `true` автоматического ускорения (обход обнаружения домашней области).</span><span class="sxs-lookup"><span data-stu-id="b22b8-165">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="b22b8-166">Если в клиенте есть только один проверенный и федераированный домен, пользователи будут доставлены непосредственно к федератированному поставщику удостоверений `true` (например, ADFS) для регистрации.</span><span class="sxs-lookup"><span data-stu-id="b22b8-166">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="b22b8-167">Если в клиенте имеется несколько проверенных `true` доменов, необходимо укаменеть **PreferredDomain.**</span><span class="sxs-lookup"><span data-stu-id="b22b8-167">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="b22b8-168">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b22b8-168">Optional.</span></span>|
|<span data-ttu-id="b22b8-169">PreferredDomain</span><span class="sxs-lookup"><span data-stu-id="b22b8-169">PreferredDomain</span></span>|<span data-ttu-id="b22b8-170">String</span><span class="sxs-lookup"><span data-stu-id="b22b8-170">String</span></span>| <span data-ttu-id="b22b8-171">Указывает домен, чтобы ускорить вход в.</span><span class="sxs-lookup"><span data-stu-id="b22b8-171">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="b22b8-172">Он может быть опущен, если у клиента есть только один федераированный домен.</span><span class="sxs-lookup"><span data-stu-id="b22b8-172">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="b22b8-173">Если он опущен и существует несколько проверенных федераированных доменов, эта политика не влияет.</span><span class="sxs-lookup"><span data-stu-id="b22b8-173">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="b22b8-174">Обязательно, **если accelerateToFederatedDomain** `true` является .</span><span class="sxs-lookup"><span data-stu-id="b22b8-174">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="b22b8-175">AllowCloudPasswordValidation</span><span class="sxs-lookup"><span data-stu-id="b22b8-175">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="b22b8-176">Логический</span><span class="sxs-lookup"><span data-stu-id="b22b8-176">Boolean</span></span>| <span data-ttu-id="b22b8-177">Установите, чтобы разрешить приложению проверку подлинности федерарно настроенного пользователя путем вручения учетных данных пользователя или пароля непосредственно в конечной точке маркера `true` Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b22b8-177">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="b22b8-178">Работает только в том случае, если включена синхронизация паролей.</span><span class="sxs-lookup"><span data-stu-id="b22b8-178">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="b22b8-179">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b22b8-179">Optional.</span></span>|
|<span data-ttu-id="b22b8-180">AlternateIdLogin</span><span class="sxs-lookup"><span data-stu-id="b22b8-180">AlternateIdLogin</span></span>| <span data-ttu-id="b22b8-181">Json</span><span class="sxs-lookup"><span data-stu-id="b22b8-181">Json</span></span> |<span data-ttu-id="b22b8-182">Установите {"Включено": true} чтобы разрешить вход в Azure AD с помощью электронной почты в качестве [альтернативного входа.](/azure/active-directory/authentication/howto-authentication-use-email-signin)</span><span class="sxs-lookup"><span data-stu-id="b22b8-182">Set to {"Enabled": true} to allow Azure AD sign-in using email as [an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span> <span data-ttu-id="b22b8-183">Работает только при **наборе IsOrganizationDefault** `true` .</span><span class="sxs-lookup"><span data-stu-id="b22b8-183">Only works when **IsOrganizationDefault** is set to `true`.</span></span> <span data-ttu-id="b22b8-184">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b22b8-184">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b22b8-185">Связи</span><span class="sxs-lookup"><span data-stu-id="b22b8-185">Relationships</span></span>

| <span data-ttu-id="b22b8-186">Связь</span><span class="sxs-lookup"><span data-stu-id="b22b8-186">Relationship</span></span> | <span data-ttu-id="b22b8-187">Тип</span><span class="sxs-lookup"><span data-stu-id="b22b8-187">Type</span></span>        | <span data-ttu-id="b22b8-188">Описание</span><span class="sxs-lookup"><span data-stu-id="b22b8-188">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b22b8-189">appliesTo</span><span class="sxs-lookup"><span data-stu-id="b22b8-189">appliesTo</span></span>|<span data-ttu-id="b22b8-190">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="b22b8-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="b22b8-191">Коллекция [directoryObject,](directoryObject.md) к которую была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="b22b8-191">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="b22b8-192">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b22b8-192">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b22b8-193">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b22b8-193">JSON representation</span></span>

<span data-ttu-id="b22b8-194">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b22b8-194">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "homeRealmDiscoveryPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
