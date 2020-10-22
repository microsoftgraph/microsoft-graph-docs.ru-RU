---
title: Тип ресурса Хомереалмдисковериполици
description: Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 94e39375648824819edb74a9707a5f1286f33087
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635189"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="85ac2-103">Тип ресурса Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="85ac2-103">homeRealmDiscoveryPolicy resource type</span></span>

<span data-ttu-id="85ac2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85ac2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85ac2-105">Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федеративных доменах.</span><span class="sxs-lookup"><span data-stu-id="85ac2-105">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="85ac2-106">Вы можете настроить **хомереалмдисковериполици** для всех субъектов службы в организации или для определенных субъектов службы в Организации.</span><span class="sxs-lookup"><span data-stu-id="85ac2-106">You can set **homeRealmDiscoveryPolicy** for all service principals in your organization, or for specific service principals in your organization.</span></span> <span data-ttu-id="85ac2-107">Дополнительные сведения о сценариях и политиках приведены [в статье Настройка входа в систему Azure AD для приложения с помощью политики обнаружения домашней области](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) и [Вход в Azure Active Directory с использованием электронной почты в качестве альтернативного идентификатора входа](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span><span class="sxs-lookup"><span data-stu-id="85ac2-107">For more scenario and policy details, see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) as well as [Sign-in to Azure Active Directory using email as an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span>

<span data-ttu-id="85ac2-108">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="85ac2-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="85ac2-109">Методы</span><span class="sxs-lookup"><span data-stu-id="85ac2-109">Methods</span></span>

| <span data-ttu-id="85ac2-110">Метод</span><span class="sxs-lookup"><span data-stu-id="85ac2-110">Method</span></span>       | <span data-ttu-id="85ac2-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="85ac2-111">Return Type</span></span> | <span data-ttu-id="85ac2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="85ac2-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="85ac2-113">Перечисление типов ресурсов homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="85ac2-113">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="85ac2-114">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="85ac2-114">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="85ac2-115">Чтение свойств и связей объектов ХомереалмдисковериполиЦиес.</span><span class="sxs-lookup"><span data-stu-id="85ac2-115">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="85ac2-116">Создание Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="85ac2-116">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="85ac2-117">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="85ac2-117">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="85ac2-118">Создание объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="85ac2-118">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="85ac2-119">Получение Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="85ac2-119">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="85ac2-120">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="85ac2-120">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="85ac2-121">Чтение свойств и связей объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="85ac2-121">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="85ac2-122">Обновление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="85ac2-122">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="85ac2-123">Нет</span><span class="sxs-lookup"><span data-stu-id="85ac2-123">None</span></span> | <span data-ttu-id="85ac2-124">Обновление объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="85ac2-124">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="85ac2-125">Удаление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="85ac2-125">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="85ac2-126">Нет</span><span class="sxs-lookup"><span data-stu-id="85ac2-126">None</span></span> | <span data-ttu-id="85ac2-127">Удаление объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="85ac2-127">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="85ac2-128">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="85ac2-128">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="85ac2-129">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="85ac2-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="85ac2-130">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="85ac2-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="85ac2-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="85ac2-131">Properties</span></span>

| <span data-ttu-id="85ac2-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="85ac2-132">Property</span></span>     | <span data-ttu-id="85ac2-133">Тип</span><span class="sxs-lookup"><span data-stu-id="85ac2-133">Type</span></span>        | <span data-ttu-id="85ac2-134">Описание</span><span class="sxs-lookup"><span data-stu-id="85ac2-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="85ac2-135">id</span><span class="sxs-lookup"><span data-stu-id="85ac2-135">id</span></span>|<span data-ttu-id="85ac2-136">String</span><span class="sxs-lookup"><span data-stu-id="85ac2-136">String</span></span>| <span data-ttu-id="85ac2-137">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="85ac2-137">Unique identifier for this policy.</span></span> <span data-ttu-id="85ac2-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85ac2-138">Read-only.</span></span>|
|<span data-ttu-id="85ac2-139">RDLC</span><span class="sxs-lookup"><span data-stu-id="85ac2-139">definition</span></span>|<span data-ttu-id="85ac2-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="85ac2-140">String collection</span></span>| <span data-ttu-id="85ac2-141">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="85ac2-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="85ac2-142">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="85ac2-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="85ac2-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85ac2-143">Required.</span></span>|
|<span data-ttu-id="85ac2-144">description</span><span class="sxs-lookup"><span data-stu-id="85ac2-144">description</span></span>|<span data-ttu-id="85ac2-145">String</span><span class="sxs-lookup"><span data-stu-id="85ac2-145">String</span></span>| <span data-ttu-id="85ac2-146">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="85ac2-146">Description for this policy.</span></span>|
|<span data-ttu-id="85ac2-147">displayName</span><span class="sxs-lookup"><span data-stu-id="85ac2-147">displayName</span></span>|<span data-ttu-id="85ac2-148">String</span><span class="sxs-lookup"><span data-stu-id="85ac2-148">String</span></span>| <span data-ttu-id="85ac2-149">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="85ac2-149">Display name for this policy.</span></span> <span data-ttu-id="85ac2-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85ac2-150">Required.</span></span>|
|<span data-ttu-id="85ac2-151">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="85ac2-151">isOrganizationDefault</span></span>|<span data-ttu-id="85ac2-152">Логический</span><span class="sxs-lookup"><span data-stu-id="85ac2-152">Boolean</span></span>|<span data-ttu-id="85ac2-153">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="85ac2-153">If set to true, activates this policy.</span></span> <span data-ttu-id="85ac2-154">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="85ac2-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="85ac2-155">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="85ac2-155">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="85ac2-156">Свойства определения политики обнаружения домашней области</span><span class="sxs-lookup"><span data-stu-id="85ac2-156">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="85ac2-157">Свойства, приведенные ниже, формируют объект JSON, представляющий политику времени существования маркеров.</span><span class="sxs-lookup"><span data-stu-id="85ac2-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="85ac2-158">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="85ac2-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="85ac2-159">Ниже показан пример в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85ac2-159">An example is shown below in JSON format:</span></span>

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

| <span data-ttu-id="85ac2-160">Свойство</span><span class="sxs-lookup"><span data-stu-id="85ac2-160">Property</span></span>     | <span data-ttu-id="85ac2-161">Тип</span><span class="sxs-lookup"><span data-stu-id="85ac2-161">Type</span></span>   |<span data-ttu-id="85ac2-162">Описание</span><span class="sxs-lookup"><span data-stu-id="85ac2-162">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="85ac2-163">акцелератетофедератеддомаин</span><span class="sxs-lookup"><span data-stu-id="85ac2-163">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="85ac2-164">Логический</span><span class="sxs-lookup"><span data-stu-id="85ac2-164">Boolean</span></span>| <span data-ttu-id="85ac2-165">Задано значение `true` для автоускорения (обход поиска домашних областей).</span><span class="sxs-lookup"><span data-stu-id="85ac2-165">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="85ac2-166">Если `true` в клиенте есть только один проверенный и федеративный домен, то пользователи будут передаваться непосредственно поставщику федеративного удостоверения (например, ADFS) для входа.</span><span class="sxs-lookup"><span data-stu-id="85ac2-166">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="85ac2-167">Если `true` в клиенте имеется несколько проверенных доменов, необходимо указать **преферреддомаин** .</span><span class="sxs-lookup"><span data-stu-id="85ac2-167">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="85ac2-168">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="85ac2-168">Optional.</span></span>|
|<span data-ttu-id="85ac2-169">преферреддомаин</span><span class="sxs-lookup"><span data-stu-id="85ac2-169">PreferredDomain</span></span>|<span data-ttu-id="85ac2-170">String</span><span class="sxs-lookup"><span data-stu-id="85ac2-170">String</span></span>| <span data-ttu-id="85ac2-171">Указывает домен для ускорения входа в систему.</span><span class="sxs-lookup"><span data-stu-id="85ac2-171">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="85ac2-172">Его можно опустить, если у клиента только один федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="85ac2-172">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="85ac2-173">Если он не указан и существует несколько проверенных федеративных доменов, эта политика не оказывает никакого действия.</span><span class="sxs-lookup"><span data-stu-id="85ac2-173">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="85ac2-174">Обязательный, если **акцелератетофедератеддомаин** — `true` .</span><span class="sxs-lookup"><span data-stu-id="85ac2-174">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="85ac2-175">алловклаудпассвордвалидатион</span><span class="sxs-lookup"><span data-stu-id="85ac2-175">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="85ac2-176">Логический</span><span class="sxs-lookup"><span data-stu-id="85ac2-176">Boolean</span></span>| <span data-ttu-id="85ac2-177">Чтобы `true` разрешить приложению выполнять проверку подлинности федеративного пользователя, указав учетные данные имени пользователя и пароля непосредственно в конечной точке маркера Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="85ac2-177">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="85ac2-178">Работает, только если включена синхронизация хэша паролей.</span><span class="sxs-lookup"><span data-stu-id="85ac2-178">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="85ac2-179">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="85ac2-179">Optional.</span></span>|
|<span data-ttu-id="85ac2-180">алтернатеидлогин</span><span class="sxs-lookup"><span data-stu-id="85ac2-180">AlternateIdLogin</span></span>| <span data-ttu-id="85ac2-181">Json</span><span class="sxs-lookup"><span data-stu-id="85ac2-181">Json</span></span> |<span data-ttu-id="85ac2-182">Задайте значение {"Enabled": true}, чтобы разрешить вход Azure AD с использованием электронной почты в качестве [альтернативного идентификатора входа](https://docs.microsoft.com/azure/active-directory/authentication/howto-authentication-use-email-signin).</span><span class="sxs-lookup"><span data-stu-id="85ac2-182">Set to {"Enabled": true} to allow Azure AD sign-in using email as [an alternate login ID](https://docs.microsoft.com/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span> <span data-ttu-id="85ac2-183">Работает, только если для **исорганизатиондефаулт** задано значение `true` .</span><span class="sxs-lookup"><span data-stu-id="85ac2-183">Only works when **IsOrganizationDefault** is set to `true`.</span></span> <span data-ttu-id="85ac2-184">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="85ac2-184">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85ac2-185">Связи</span><span class="sxs-lookup"><span data-stu-id="85ac2-185">Relationships</span></span>

| <span data-ttu-id="85ac2-186">Связь</span><span class="sxs-lookup"><span data-stu-id="85ac2-186">Relationship</span></span> | <span data-ttu-id="85ac2-187">Тип</span><span class="sxs-lookup"><span data-stu-id="85ac2-187">Type</span></span>        | <span data-ttu-id="85ac2-188">Описание</span><span class="sxs-lookup"><span data-stu-id="85ac2-188">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="85ac2-189">Тег</span><span class="sxs-lookup"><span data-stu-id="85ac2-189">appliesTo</span></span>|<span data-ttu-id="85ac2-190">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="85ac2-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="85ac2-191">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="85ac2-191">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="85ac2-192">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85ac2-192">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85ac2-193">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85ac2-193">JSON representation</span></span>

<span data-ttu-id="85ac2-194">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85ac2-194">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true,
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
