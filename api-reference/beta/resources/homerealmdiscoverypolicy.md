---
title: Тип ресурса Хомереалмдисковериполици
description: Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5e9c5d9933c2b98a1012291f02fa7e248bd403dd
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401441"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="66f17-103">Тип ресурса Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="66f17-103">homeRealmDiscoveryPolicy resource type</span></span>

<span data-ttu-id="66f17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66f17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66f17-105">Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федеративных доменах.</span><span class="sxs-lookup"><span data-stu-id="66f17-105">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="66f17-106">Вы можете настроить Хомереалмдисковериполици для всех субъектов службы в организации или для определенных субъектов службы в Организации.</span><span class="sxs-lookup"><span data-stu-id="66f17-106">You can set homeRealmDiscoveryPolicy for all service principals in your organization, or for specific service principals in your organization.</span></span>  <span data-ttu-id="66f17-107">Дополнительные сведения о сценариях и политиках приведены [в статье Настройка режима входа в Azure AD для приложения с помощью политики обнаружения домашней области](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span><span class="sxs-lookup"><span data-stu-id="66f17-107">For more scenario and policy details see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span></span>

<span data-ttu-id="66f17-108">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="66f17-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="66f17-109">Методы</span><span class="sxs-lookup"><span data-stu-id="66f17-109">Methods</span></span>

| <span data-ttu-id="66f17-110">Метод</span><span class="sxs-lookup"><span data-stu-id="66f17-110">Method</span></span>       | <span data-ttu-id="66f17-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="66f17-111">Return Type</span></span> | <span data-ttu-id="66f17-112">Описание</span><span class="sxs-lookup"><span data-stu-id="66f17-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="66f17-113">Создание Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="66f17-113">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="66f17-114">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="66f17-114">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="66f17-115">Создание объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="66f17-115">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="66f17-116">Получение Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="66f17-116">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="66f17-117">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="66f17-117">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="66f17-118">Чтение свойств и связей объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="66f17-118">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="66f17-119">Перечисление типов ресурсов homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="66f17-119">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="66f17-120">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="66f17-120">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="66f17-121">Чтение свойств и связей объектов ХомереалмдисковериполиЦиес.</span><span class="sxs-lookup"><span data-stu-id="66f17-121">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="66f17-122">Обновление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="66f17-122">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="66f17-123">Нет</span><span class="sxs-lookup"><span data-stu-id="66f17-123">None</span></span> | <span data-ttu-id="66f17-124">Обновление объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="66f17-124">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="66f17-125">Удаление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="66f17-125">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="66f17-126">Нет</span><span class="sxs-lookup"><span data-stu-id="66f17-126">None</span></span> | <span data-ttu-id="66f17-127">Удаление объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="66f17-127">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="66f17-128">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="66f17-128">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="66f17-129">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="66f17-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="66f17-130">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="66f17-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="66f17-131">Назначение типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="66f17-131">Assign homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-post-homerealmdiscoverypolicies.md) | <span data-ttu-id="66f17-132">Нет</span><span class="sxs-lookup"><span data-stu-id="66f17-132">None</span></span> | <span data-ttu-id="66f17-133">Назначьте объект Хомереалмдисковериполици объекту [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="66f17-133">Assign a homeRealmDiscoveryPolicy object to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="66f17-134">Список назначенных Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="66f17-134">List assigned homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-list-homerealmdiscoverypolicies.md) | <span data-ttu-id="66f17-135">Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="66f17-135">[homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) collection</span></span> | <span data-ttu-id="66f17-136">Перечисление объектов Хомереалмдисковериполици, назначенных объекту [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="66f17-136">List the homeRealmDiscoveryPolicy objects that are assigned to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="66f17-137">Удаление типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="66f17-137">Remove homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md) | <span data-ttu-id="66f17-138">Нет</span><span class="sxs-lookup"><span data-stu-id="66f17-138">None</span></span> | <span data-ttu-id="66f17-139">Удаление объекта Хомереалмдисковериполици из объекта [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="66f17-139">Remove a homeRealmDiscoveryPolicy object from a [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="66f17-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="66f17-140">Properties</span></span>

| <span data-ttu-id="66f17-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="66f17-141">Property</span></span>     | <span data-ttu-id="66f17-142">Тип</span><span class="sxs-lookup"><span data-stu-id="66f17-142">Type</span></span>        | <span data-ttu-id="66f17-143">Описание</span><span class="sxs-lookup"><span data-stu-id="66f17-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="66f17-144">id</span><span class="sxs-lookup"><span data-stu-id="66f17-144">id</span></span>|<span data-ttu-id="66f17-145">String</span><span class="sxs-lookup"><span data-stu-id="66f17-145">String</span></span>| <span data-ttu-id="66f17-146">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="66f17-146">Unique identifier for this policy.</span></span> <span data-ttu-id="66f17-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66f17-147">Read-only.</span></span>|
|<span data-ttu-id="66f17-148">RDLC</span><span class="sxs-lookup"><span data-stu-id="66f17-148">definition</span></span>|<span data-ttu-id="66f17-149">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="66f17-149">String collection</span></span>| <span data-ttu-id="66f17-150">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="66f17-150">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="66f17-151">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="66f17-151">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="66f17-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66f17-152">Required.</span></span>|
|<span data-ttu-id="66f17-153">description</span><span class="sxs-lookup"><span data-stu-id="66f17-153">description</span></span>|<span data-ttu-id="66f17-154">String</span><span class="sxs-lookup"><span data-stu-id="66f17-154">String</span></span>| <span data-ttu-id="66f17-155">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="66f17-155">Description for this policy.</span></span>|
|<span data-ttu-id="66f17-156">displayName</span><span class="sxs-lookup"><span data-stu-id="66f17-156">displayName</span></span>|<span data-ttu-id="66f17-157">String</span><span class="sxs-lookup"><span data-stu-id="66f17-157">String</span></span>| <span data-ttu-id="66f17-158">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="66f17-158">Display name for this policy.</span></span> <span data-ttu-id="66f17-159">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="66f17-159">Required.</span></span>|
|<span data-ttu-id="66f17-160">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="66f17-160">isOrganizationDefault</span></span>|<span data-ttu-id="66f17-161">Логический</span><span class="sxs-lookup"><span data-stu-id="66f17-161">Boolean</span></span>|<span data-ttu-id="66f17-162">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="66f17-162">If set to true, activates this policy.</span></span> <span data-ttu-id="66f17-163">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="66f17-163">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="66f17-164">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="66f17-164">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="66f17-165">Свойства определения политики обнаружения домашней области</span><span class="sxs-lookup"><span data-stu-id="66f17-165">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="66f17-166">Свойства, приведенные ниже, формируют объект JSON, представляющий политику времени существования маркеров.</span><span class="sxs-lookup"><span data-stu-id="66f17-166">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="66f17-167">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="66f17-167">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="66f17-168">Ниже показан пример в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66f17-168">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"HomeRealmDiscoveryPolicy\":
     {\"AccelerateToFederatedDomain\":true,
      \"PreferredDomain\":\"federated.example.edu\"}}"
  ]
```

| <span data-ttu-id="66f17-169">Свойство</span><span class="sxs-lookup"><span data-stu-id="66f17-169">Property</span></span>     | <span data-ttu-id="66f17-170">Тип</span><span class="sxs-lookup"><span data-stu-id="66f17-170">Type</span></span>   |<span data-ttu-id="66f17-171">Описание</span><span class="sxs-lookup"><span data-stu-id="66f17-171">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="66f17-172">акцелератетофедератеддомаин</span><span class="sxs-lookup"><span data-stu-id="66f17-172">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="66f17-173">Логический</span><span class="sxs-lookup"><span data-stu-id="66f17-173">Boolean</span></span>| <span data-ttu-id="66f17-174">Задано значение `true` для автоускорения (обход поиска домашних областей).</span><span class="sxs-lookup"><span data-stu-id="66f17-174">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="66f17-175">Если `true` в клиенте есть только один проверенный и федеративный домен, то пользователи будут передаваться непосредственно поставщику федеративного удостоверения (например, ADFS) для входа.</span><span class="sxs-lookup"><span data-stu-id="66f17-175">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="66f17-176">Если `true` в клиенте имеется несколько проверенных доменов, необходимо указать **преферреддомаин** .</span><span class="sxs-lookup"><span data-stu-id="66f17-176">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="66f17-177">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="66f17-177">Optional.</span></span>|
|<span data-ttu-id="66f17-178">преферреддомаин</span><span class="sxs-lookup"><span data-stu-id="66f17-178">PreferredDomain</span></span>|<span data-ttu-id="66f17-179">String</span><span class="sxs-lookup"><span data-stu-id="66f17-179">String</span></span>| <span data-ttu-id="66f17-180">Указывает домен для ускорения входа в систему.</span><span class="sxs-lookup"><span data-stu-id="66f17-180">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="66f17-181">Его можно опустить, если у клиента только один федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="66f17-181">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="66f17-182">Если он не указан и существует несколько проверенных федеративных доменов, эта политика не оказывает никакого действия.</span><span class="sxs-lookup"><span data-stu-id="66f17-182">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="66f17-183">Обязательный, если **акцелератетофедератеддомаин** — `true` .</span><span class="sxs-lookup"><span data-stu-id="66f17-183">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="66f17-184">алловклаудпассвордвалидатион</span><span class="sxs-lookup"><span data-stu-id="66f17-184">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="66f17-185">Логический</span><span class="sxs-lookup"><span data-stu-id="66f17-185">Boolean</span></span>| <span data-ttu-id="66f17-186">Чтобы `true` разрешить приложению выполнять проверку подлинности федеративного пользователя, указав учетные данные имени пользователя и пароля непосредственно в конечной точке маркера Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="66f17-186">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="66f17-187">Работает, только если включена синхронизация хэша паролей.</span><span class="sxs-lookup"><span data-stu-id="66f17-187">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="66f17-188">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="66f17-188">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66f17-189">Связи</span><span class="sxs-lookup"><span data-stu-id="66f17-189">Relationships</span></span>

| <span data-ttu-id="66f17-190">Связь</span><span class="sxs-lookup"><span data-stu-id="66f17-190">Relationship</span></span> | <span data-ttu-id="66f17-191">Тип</span><span class="sxs-lookup"><span data-stu-id="66f17-191">Type</span></span>        | <span data-ttu-id="66f17-192">Описание</span><span class="sxs-lookup"><span data-stu-id="66f17-192">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="66f17-193">Тег</span><span class="sxs-lookup"><span data-stu-id="66f17-193">appliesTo</span></span>|<span data-ttu-id="66f17-194">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="66f17-194">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="66f17-195">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="66f17-195">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="66f17-196">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66f17-196">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66f17-197">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66f17-197">JSON representation</span></span>

<span data-ttu-id="66f17-198">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66f17-198">The following is a JSON representation of the resource.</span></span>

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