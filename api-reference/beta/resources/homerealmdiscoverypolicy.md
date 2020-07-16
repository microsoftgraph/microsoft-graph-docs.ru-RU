---
title: Тип ресурса Хомереалмдисковериполици
description: Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7a1a214553bca62438078a02834565338fc0e163
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007094"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="2a1ef-103">Тип ресурса Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="2a1ef-103">homeRealmDiscoveryPolicy resource type</span></span>

<span data-ttu-id="2a1ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a1ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a1ef-105">Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федеративных доменах.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-105">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="2a1ef-106">Вы можете настроить Хомереалмдисковериполици для всех субъектов службы в организации или для определенных субъектов службы в Организации.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-106">You can set homeRealmDiscoveryPolicy for all service principals in your organization, or for specific service principals in your organization.</span></span>  <span data-ttu-id="2a1ef-107">Дополнительные сведения о сценариях и политиках приведены [в статье Настройка режима входа в Azure AD для приложения с помощью политики обнаружения домашней области](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span><span class="sxs-lookup"><span data-stu-id="2a1ef-107">For more scenario and policy details see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span></span>

<span data-ttu-id="2a1ef-108">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2a1ef-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2a1ef-109">Методы</span><span class="sxs-lookup"><span data-stu-id="2a1ef-109">Methods</span></span>

| <span data-ttu-id="2a1ef-110">Метод</span><span class="sxs-lookup"><span data-stu-id="2a1ef-110">Method</span></span>       | <span data-ttu-id="2a1ef-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2a1ef-111">Return Type</span></span> | <span data-ttu-id="2a1ef-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2a1ef-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2a1ef-113">Создание Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="2a1ef-113">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="2a1ef-114">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="2a1ef-114">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="2a1ef-115">Создание объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-115">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="2a1ef-116">Получение Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="2a1ef-116">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="2a1ef-117">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="2a1ef-117">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="2a1ef-118">Чтение свойств и связей объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-118">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="2a1ef-119">Перечисление типов ресурсов homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="2a1ef-119">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="2a1ef-120">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="2a1ef-120">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="2a1ef-121">Чтение свойств и связей объектов ХомереалмдисковериполиЦиес.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-121">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="2a1ef-122">Обновление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="2a1ef-122">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="2a1ef-123">Нет</span><span class="sxs-lookup"><span data-stu-id="2a1ef-123">None</span></span> | <span data-ttu-id="2a1ef-124">Обновление объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-124">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="2a1ef-125">Удаление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="2a1ef-125">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="2a1ef-126">Нет</span><span class="sxs-lookup"><span data-stu-id="2a1ef-126">None</span></span> | <span data-ttu-id="2a1ef-127">Удаление объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-127">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="2a1ef-128">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="2a1ef-128">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="2a1ef-129">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="2a1ef-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="2a1ef-130">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="2a1ef-131">Назначение типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="2a1ef-131">Assign homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-post-homerealmdiscoverypolicies.md) | <span data-ttu-id="2a1ef-132">Нет</span><span class="sxs-lookup"><span data-stu-id="2a1ef-132">None</span></span> | <span data-ttu-id="2a1ef-133">Назначьте объект Хомереалмдисковериполици объекту [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="2a1ef-133">Assign a homeRealmDiscoveryPolicy object to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="2a1ef-134">Список назначенных Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="2a1ef-134">List assigned homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-list-homerealmdiscoverypolicies.md) | <span data-ttu-id="2a1ef-135">Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2a1ef-135">[homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) collection</span></span> | <span data-ttu-id="2a1ef-136">Перечисление объектов Хомереалмдисковериполици, назначенных объекту [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="2a1ef-136">List the homeRealmDiscoveryPolicy objects that are assigned to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="2a1ef-137">Удаление типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="2a1ef-137">Remove homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md) | <span data-ttu-id="2a1ef-138">Нет</span><span class="sxs-lookup"><span data-stu-id="2a1ef-138">None</span></span> | <span data-ttu-id="2a1ef-139">Удаление объекта Хомереалмдисковериполици из объекта [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="2a1ef-139">Remove a homeRealmDiscoveryPolicy object from a [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2a1ef-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a1ef-140">Properties</span></span>

| <span data-ttu-id="2a1ef-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a1ef-141">Property</span></span>     | <span data-ttu-id="2a1ef-142">Тип</span><span class="sxs-lookup"><span data-stu-id="2a1ef-142">Type</span></span>        | <span data-ttu-id="2a1ef-143">Описание</span><span class="sxs-lookup"><span data-stu-id="2a1ef-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2a1ef-144">id</span><span class="sxs-lookup"><span data-stu-id="2a1ef-144">id</span></span>|<span data-ttu-id="2a1ef-145">String</span><span class="sxs-lookup"><span data-stu-id="2a1ef-145">String</span></span>| <span data-ttu-id="2a1ef-146">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-146">Unique identifier for this policy.</span></span> <span data-ttu-id="2a1ef-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-147">Read-only.</span></span>|
|<span data-ttu-id="2a1ef-148">RDLC</span><span class="sxs-lookup"><span data-stu-id="2a1ef-148">definition</span></span>|<span data-ttu-id="2a1ef-149">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2a1ef-149">String collection</span></span>| <span data-ttu-id="2a1ef-150">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-150">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="2a1ef-151">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-151">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="2a1ef-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-152">Required.</span></span>|
|<span data-ttu-id="2a1ef-153">description</span><span class="sxs-lookup"><span data-stu-id="2a1ef-153">description</span></span>|<span data-ttu-id="2a1ef-154">String</span><span class="sxs-lookup"><span data-stu-id="2a1ef-154">String</span></span>| <span data-ttu-id="2a1ef-155">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-155">Description for this policy.</span></span>|
|<span data-ttu-id="2a1ef-156">displayName</span><span class="sxs-lookup"><span data-stu-id="2a1ef-156">displayName</span></span>|<span data-ttu-id="2a1ef-157">Строка</span><span class="sxs-lookup"><span data-stu-id="2a1ef-157">String</span></span>| <span data-ttu-id="2a1ef-158">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-158">Display name for this policy.</span></span> <span data-ttu-id="2a1ef-159">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-159">Required.</span></span>|
|<span data-ttu-id="2a1ef-160">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="2a1ef-160">isOrganizationDefault</span></span>|<span data-ttu-id="2a1ef-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a1ef-161">Boolean</span></span>|<span data-ttu-id="2a1ef-162">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-162">If set to true, activates this policy.</span></span> <span data-ttu-id="2a1ef-163">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-163">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="2a1ef-164">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-164">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="2a1ef-165">Свойства определения политики обнаружения домашней области</span><span class="sxs-lookup"><span data-stu-id="2a1ef-165">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="2a1ef-166">Свойства, приведенные ниже, формируют объект JSON, представляющий политику времени существования маркеров.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-166">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="2a1ef-167">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="2a1ef-167">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="2a1ef-168">Ниже показан пример в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-168">An example is shown below in JSON format:</span></span>

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

| <span data-ttu-id="2a1ef-169">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a1ef-169">Property</span></span>     | <span data-ttu-id="2a1ef-170">Тип</span><span class="sxs-lookup"><span data-stu-id="2a1ef-170">Type</span></span>   |<span data-ttu-id="2a1ef-171">Описание</span><span class="sxs-lookup"><span data-stu-id="2a1ef-171">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="2a1ef-172">акцелератетофедератеддомаин</span><span class="sxs-lookup"><span data-stu-id="2a1ef-172">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="2a1ef-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a1ef-173">Boolean</span></span>| <span data-ttu-id="2a1ef-174">Задано значение `true` для автоускорения (обход поиска домашних областей).</span><span class="sxs-lookup"><span data-stu-id="2a1ef-174">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="2a1ef-175">Если `true` в клиенте есть только один проверенный и федеративный домен, то пользователи будут передаваться непосредственно поставщику федеративного удостоверения (например, ADFS) для входа.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-175">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="2a1ef-176">Если `true` в клиенте имеется несколько проверенных доменов, необходимо указать **преферреддомаин** .</span><span class="sxs-lookup"><span data-stu-id="2a1ef-176">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="2a1ef-177">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-177">Optional.</span></span>|
|<span data-ttu-id="2a1ef-178">преферреддомаин</span><span class="sxs-lookup"><span data-stu-id="2a1ef-178">PreferredDomain</span></span>|<span data-ttu-id="2a1ef-179">String</span><span class="sxs-lookup"><span data-stu-id="2a1ef-179">String</span></span>| <span data-ttu-id="2a1ef-180">Указывает домен для ускорения входа в систему.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-180">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="2a1ef-181">Его можно опустить, если у клиента только один федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-181">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="2a1ef-182">Если он не указан и существует несколько проверенных федеративных доменов, эта политика не оказывает никакого действия.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-182">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="2a1ef-183">Обязательный, если **акцелератетофедератеддомаин** — `true` .</span><span class="sxs-lookup"><span data-stu-id="2a1ef-183">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="2a1ef-184">алловклаудпассвордвалидатион</span><span class="sxs-lookup"><span data-stu-id="2a1ef-184">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="2a1ef-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a1ef-185">Boolean</span></span>| <span data-ttu-id="2a1ef-186">Чтобы `true` разрешить приложению выполнять проверку подлинности федеративного пользователя, указав учетные данные имени пользователя и пароля непосредственно в конечной точке маркера Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-186">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="2a1ef-187">Работает, только если включена синхронизация хэша паролей.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-187">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="2a1ef-188">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-188">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a1ef-189">Связи</span><span class="sxs-lookup"><span data-stu-id="2a1ef-189">Relationships</span></span>

| <span data-ttu-id="2a1ef-190">Связь</span><span class="sxs-lookup"><span data-stu-id="2a1ef-190">Relationship</span></span> | <span data-ttu-id="2a1ef-191">Тип</span><span class="sxs-lookup"><span data-stu-id="2a1ef-191">Type</span></span>        | <span data-ttu-id="2a1ef-192">Описание</span><span class="sxs-lookup"><span data-stu-id="2a1ef-192">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2a1ef-193">Тег</span><span class="sxs-lookup"><span data-stu-id="2a1ef-193">appliesTo</span></span>|<span data-ttu-id="2a1ef-194">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="2a1ef-194">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="2a1ef-195">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-195">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="2a1ef-196">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-196">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a1ef-197">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a1ef-197">JSON representation</span></span>

<span data-ttu-id="2a1ef-198">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a1ef-198">The following is a JSON representation of the resource.</span></span>

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