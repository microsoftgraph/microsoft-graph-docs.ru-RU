---
title: Тип ресурса homeRealmDiscoveryPolicy
description: Представляет политику для управления поведением проверки подлинности Azure Active Directory для федерационных пользователей.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 56e0d5b0e47c5f3ba5b37e4cbafad2138a2a7e79
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154210"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="e518c-103">Тип ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="e518c-103">homeRealmDiscoveryPolicy resource type</span></span>

<span data-ttu-id="e518c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e518c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e518c-105">Представляет политику для управления поведением проверки подлинности Azure Active Directory для федерационных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федерационных доменах.</span><span class="sxs-lookup"><span data-stu-id="e518c-105">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="e518c-106">Вы можете настроить **homeRealmDiscoveryPolicy** для всех основных служб в организации или для определенных ее основных служб.</span><span class="sxs-lookup"><span data-stu-id="e518c-106">You can set **homeRealmDiscoveryPolicy** for all service principals in your organization, or for specific service principals in your organization.</span></span> <span data-ttu-id="e518c-107">Дополнительные сведения о сценарии и политике см. в настройках поведения входа [в Azure AD](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) для приложения с помощью политики обнаружения домашней области, а также в входе в [Azure Active Directory](/azure/active-directory/authentication/howto-authentication-use-email-signin)с помощью электронной почты в качестве альтернативного ИД входа.</span><span class="sxs-lookup"><span data-stu-id="e518c-107">For more scenario and policy details, see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) as well as [Sign-in to Azure Active Directory using email as an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span>

<span data-ttu-id="e518c-108">Наследуется от [stsPolicy.](stsPolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e518c-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e518c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="e518c-109">Methods</span></span>

| <span data-ttu-id="e518c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="e518c-110">Method</span></span>       | <span data-ttu-id="e518c-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e518c-111">Return Type</span></span> | <span data-ttu-id="e518c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e518c-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e518c-113">Перечисление типов ресурсов homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="e518c-113">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="e518c-114">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="e518c-114">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="e518c-115">Чтение свойств и связей объектов homeRealmDiscoveryPolicies.</span><span class="sxs-lookup"><span data-stu-id="e518c-115">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="e518c-116">Создание homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="e518c-116">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="e518c-117">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="e518c-117">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="e518c-118">Создание объекта homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="e518c-118">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="e518c-119">Get homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="e518c-119">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="e518c-120">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="e518c-120">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="e518c-121">Чтение свойств и связей объекта homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="e518c-121">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="e518c-122">Обновление homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="e518c-122">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="e518c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="e518c-123">None</span></span> | <span data-ttu-id="e518c-124">Обновление объекта homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="e518c-124">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="e518c-125">Удаление homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="e518c-125">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="e518c-126">Нет</span><span class="sxs-lookup"><span data-stu-id="e518c-126">None</span></span> | <span data-ttu-id="e518c-127">Удаление объекта homeRealmDiscoveryPolicy.</span><span class="sxs-lookup"><span data-stu-id="e518c-127">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="e518c-128">List appliesTo</span><span class="sxs-lookup"><span data-stu-id="e518c-128">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="e518c-129">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e518c-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="e518c-130">Получите список directoryObjects, к которые была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="e518c-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="e518c-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="e518c-131">Properties</span></span>

| <span data-ttu-id="e518c-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="e518c-132">Property</span></span>     | <span data-ttu-id="e518c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="e518c-133">Type</span></span>        | <span data-ttu-id="e518c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e518c-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e518c-135">id</span><span class="sxs-lookup"><span data-stu-id="e518c-135">id</span></span>|<span data-ttu-id="e518c-136">String</span><span class="sxs-lookup"><span data-stu-id="e518c-136">String</span></span>| <span data-ttu-id="e518c-137">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e518c-137">Unique identifier for this policy.</span></span> <span data-ttu-id="e518c-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e518c-138">Read-only.</span></span>|
|<span data-ttu-id="e518c-139">definition</span><span class="sxs-lookup"><span data-stu-id="e518c-139">definition</span></span>|<span data-ttu-id="e518c-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e518c-140">String collection</span></span>| <span data-ttu-id="e518c-141">Коллекция строк, содержащая строку JSON, которая определяет правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e518c-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="e518c-142">Дополнительные сведения о схеме JSON для этого свойства см. ниже.</span><span class="sxs-lookup"><span data-stu-id="e518c-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="e518c-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e518c-143">Required.</span></span>|
|<span data-ttu-id="e518c-144">description</span><span class="sxs-lookup"><span data-stu-id="e518c-144">description</span></span>|<span data-ttu-id="e518c-145">String</span><span class="sxs-lookup"><span data-stu-id="e518c-145">String</span></span>| <span data-ttu-id="e518c-146">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="e518c-146">Description for this policy.</span></span>|
|<span data-ttu-id="e518c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="e518c-147">displayName</span></span>|<span data-ttu-id="e518c-148">String</span><span class="sxs-lookup"><span data-stu-id="e518c-148">String</span></span>| <span data-ttu-id="e518c-149">Отображаемого имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e518c-149">Display name for this policy.</span></span> <span data-ttu-id="e518c-150">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="e518c-150">Required.</span></span>|
|<span data-ttu-id="e518c-151">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="e518c-151">isOrganizationDefault</span></span>|<span data-ttu-id="e518c-152">Логическое</span><span class="sxs-lookup"><span data-stu-id="e518c-152">Boolean</span></span>|<span data-ttu-id="e518c-153">Если установлено true, активирует эту политику.</span><span class="sxs-lookup"><span data-stu-id="e518c-153">If set to true, activates this policy.</span></span> <span data-ttu-id="e518c-154">Для одного типа политики может быть несколько политик, но только одна может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e518c-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="e518c-155">Необязательный, значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="e518c-155">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="e518c-156">Свойства определения политики обнаружения домашней области</span><span class="sxs-lookup"><span data-stu-id="e518c-156">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="e518c-157">Ниже properties form the JSON object that represents a token lifetime policy.</span><span class="sxs-lookup"><span data-stu-id="e518c-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="e518c-158">Этот объект JSON необходимо **преобразовать** в строку с escape-кавычками, чтобы вставить его в **свойство** определения.</span><span class="sxs-lookup"><span data-stu-id="e518c-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="e518c-159">Пример показан ниже в формате JSON:</span><span class="sxs-lookup"><span data-stu-id="e518c-159">An example is shown below in JSON format:</span></span>

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

| <span data-ttu-id="e518c-160">Свойство</span><span class="sxs-lookup"><span data-stu-id="e518c-160">Property</span></span>     | <span data-ttu-id="e518c-161">Тип</span><span class="sxs-lookup"><span data-stu-id="e518c-161">Type</span></span>   |<span data-ttu-id="e518c-162">Описание</span><span class="sxs-lookup"><span data-stu-id="e518c-162">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="e518c-163">AccelerateToFederatedDomain</span><span class="sxs-lookup"><span data-stu-id="e518c-163">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="e518c-164">Логическое</span><span class="sxs-lookup"><span data-stu-id="e518c-164">Boolean</span></span>| <span data-ttu-id="e518c-165">Установите для `true` автоматического ускорения (обход обнаружения домашней области).</span><span class="sxs-lookup"><span data-stu-id="e518c-165">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="e518c-166">Если в клиенте имеется только один проверенный и федераированный домен, пользователи будут перенаправлены непосредственно к федератированному поставщику удостоверений `true` (например, ADFS) для входов.</span><span class="sxs-lookup"><span data-stu-id="e518c-166">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="e518c-167">Если в клиенте имеется несколько проверенных доменов, необходимо `true` у указано **имя PreferredDomain.**</span><span class="sxs-lookup"><span data-stu-id="e518c-167">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="e518c-168">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e518c-168">Optional.</span></span>|
|<span data-ttu-id="e518c-169">PreferredDomain</span><span class="sxs-lookup"><span data-stu-id="e518c-169">PreferredDomain</span></span>|<span data-ttu-id="e518c-170">String</span><span class="sxs-lookup"><span data-stu-id="e518c-170">String</span></span>| <span data-ttu-id="e518c-171">Указывает домен, в который необходимо ускорить вход.</span><span class="sxs-lookup"><span data-stu-id="e518c-171">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="e518c-172">Его можно о пропущено, если у клиента есть только один федераированный домен.</span><span class="sxs-lookup"><span data-stu-id="e518c-172">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="e518c-173">Если он опущен и существует несколько проверенных федераированных доменов, эта политика не действует.</span><span class="sxs-lookup"><span data-stu-id="e518c-173">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="e518c-174">Обязательно, если **accelerateToFederatedDomain** `true` имеет .</span><span class="sxs-lookup"><span data-stu-id="e518c-174">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="e518c-175">AllowCloudPasswordValidation</span><span class="sxs-lookup"><span data-stu-id="e518c-175">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="e518c-176">Логическое</span><span class="sxs-lookup"><span data-stu-id="e518c-176">Boolean</span></span>| <span data-ttu-id="e518c-177">Установите, чтобы разрешить приложению проверку подлинности федератора, предостановив учетные данные пользователя или пароля непосредственно в конечной точке маркера `true` Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e518c-177">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="e518c-178">Работает, только если включена синхронизация паролей.</span><span class="sxs-lookup"><span data-stu-id="e518c-178">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="e518c-179">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e518c-179">Optional.</span></span>|
|<span data-ttu-id="e518c-180">AlternateIdLogin</span><span class="sxs-lookup"><span data-stu-id="e518c-180">AlternateIdLogin</span></span>| <span data-ttu-id="e518c-181">Json</span><span class="sxs-lookup"><span data-stu-id="e518c-181">Json</span></span> |<span data-ttu-id="e518c-182">Установите {"Enabled": true}, чтобы разрешить вход в Azure AD с помощью электронной почты в качестве [альтернативного ИД входа.](/azure/active-directory/authentication/howto-authentication-use-email-signin)</span><span class="sxs-lookup"><span data-stu-id="e518c-182">Set to {"Enabled": true} to allow Azure AD sign-in using email as [an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span> <span data-ttu-id="e518c-183">Работает только в **том случае, если для IsOrganizationDefault** установлено такое же `true` время.</span><span class="sxs-lookup"><span data-stu-id="e518c-183">Only works when **IsOrganizationDefault** is set to `true`.</span></span> <span data-ttu-id="e518c-184">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e518c-184">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e518c-185">Связи</span><span class="sxs-lookup"><span data-stu-id="e518c-185">Relationships</span></span>

| <span data-ttu-id="e518c-186">Связь</span><span class="sxs-lookup"><span data-stu-id="e518c-186">Relationship</span></span> | <span data-ttu-id="e518c-187">Тип</span><span class="sxs-lookup"><span data-stu-id="e518c-187">Type</span></span>        | <span data-ttu-id="e518c-188">Описание</span><span class="sxs-lookup"><span data-stu-id="e518c-188">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e518c-189">appliesTo</span><span class="sxs-lookup"><span data-stu-id="e518c-189">appliesTo</span></span>|<span data-ttu-id="e518c-190">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e518c-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="e518c-191">Коллекция [directoryObject,](directoryObject.md) к которую применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="e518c-191">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="e518c-192">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e518c-192">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e518c-193">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e518c-193">JSON representation</span></span>

<span data-ttu-id="e518c-194">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e518c-194">The following is a JSON representation of the resource.</span></span>

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
