---
title: Тип ресурса Хомереалмдисковериполици
description: Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c29134a0c6d35e5dd5eff72f133938c3366912f5
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917266"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="dd2ad-103">Тип ресурса Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="dd2ad-103">homeRealmDiscoveryPolicy resource type</span></span>

<span data-ttu-id="dd2ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd2ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd2ad-105">Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федеративных доменах.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-105">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="dd2ad-106">Вы можете настроить Хомереалмдисковериполици для всех субъектов службы в организации или для определенных субъектов службы в Организации.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-106">You can set homeRealmDiscoveryPolicy for all service principals in your organization, or for specific service principals in your organization.</span></span>  <span data-ttu-id="dd2ad-107">Дополнительные сведения о сценариях и политиках приведены [в статье Настройка режима входа в Azure AD для приложения с помощью политики обнаружения домашней области](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span><span class="sxs-lookup"><span data-stu-id="dd2ad-107">For more scenario and policy details see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span></span>

<span data-ttu-id="dd2ad-108">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd2ad-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dd2ad-109">Методы</span><span class="sxs-lookup"><span data-stu-id="dd2ad-109">Methods</span></span>

| <span data-ttu-id="dd2ad-110">Метод</span><span class="sxs-lookup"><span data-stu-id="dd2ad-110">Method</span></span>       | <span data-ttu-id="dd2ad-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dd2ad-111">Return Type</span></span> | <span data-ttu-id="dd2ad-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dd2ad-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dd2ad-113">Создание Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="dd2ad-113">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="dd2ad-114">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="dd2ad-114">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="dd2ad-115">Создание объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-115">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="dd2ad-116">Получение Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="dd2ad-116">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="dd2ad-117">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="dd2ad-117">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="dd2ad-118">Чтение свойств и связей объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-118">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="dd2ad-119">Перечисление типов ресурсов homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="dd2ad-119">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="dd2ad-120">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="dd2ad-120">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="dd2ad-121">Чтение свойств и связей объектов ХомереалмдисковериполиЦиес.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-121">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="dd2ad-122">Обновление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="dd2ad-122">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="dd2ad-123">Нет</span><span class="sxs-lookup"><span data-stu-id="dd2ad-123">None</span></span> | <span data-ttu-id="dd2ad-124">Обновление объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-124">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="dd2ad-125">Удаление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="dd2ad-125">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="dd2ad-126">Нет</span><span class="sxs-lookup"><span data-stu-id="dd2ad-126">None</span></span> | <span data-ttu-id="dd2ad-127">Удаление объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-127">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="dd2ad-128">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="dd2ad-128">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="dd2ad-129">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="dd2ad-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="dd2ad-130">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="dd2ad-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd2ad-131">Properties</span></span>

| <span data-ttu-id="dd2ad-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd2ad-132">Property</span></span>     | <span data-ttu-id="dd2ad-133">Тип</span><span class="sxs-lookup"><span data-stu-id="dd2ad-133">Type</span></span>        | <span data-ttu-id="dd2ad-134">Описание</span><span class="sxs-lookup"><span data-stu-id="dd2ad-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd2ad-135">id</span><span class="sxs-lookup"><span data-stu-id="dd2ad-135">id</span></span>|<span data-ttu-id="dd2ad-136">String</span><span class="sxs-lookup"><span data-stu-id="dd2ad-136">String</span></span>| <span data-ttu-id="dd2ad-137">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-137">Unique identifier for this policy.</span></span> <span data-ttu-id="dd2ad-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-138">Read-only.</span></span>|
|<span data-ttu-id="dd2ad-139">RDLC</span><span class="sxs-lookup"><span data-stu-id="dd2ad-139">definition</span></span>|<span data-ttu-id="dd2ad-140">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="dd2ad-140">String collection</span></span>| <span data-ttu-id="dd2ad-141">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="dd2ad-142">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="dd2ad-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-143">Required.</span></span>|
|<span data-ttu-id="dd2ad-144">description</span><span class="sxs-lookup"><span data-stu-id="dd2ad-144">description</span></span>|<span data-ttu-id="dd2ad-145">String</span><span class="sxs-lookup"><span data-stu-id="dd2ad-145">String</span></span>| <span data-ttu-id="dd2ad-146">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-146">Description for this policy.</span></span>|
|<span data-ttu-id="dd2ad-147">displayName</span><span class="sxs-lookup"><span data-stu-id="dd2ad-147">displayName</span></span>|<span data-ttu-id="dd2ad-148">Строка</span><span class="sxs-lookup"><span data-stu-id="dd2ad-148">String</span></span>| <span data-ttu-id="dd2ad-149">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-149">Display name for this policy.</span></span> <span data-ttu-id="dd2ad-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-150">Required.</span></span>|
|<span data-ttu-id="dd2ad-151">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="dd2ad-151">isOrganizationDefault</span></span>|<span data-ttu-id="dd2ad-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd2ad-152">Boolean</span></span>|<span data-ttu-id="dd2ad-153">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-153">If set to true, activates this policy.</span></span> <span data-ttu-id="dd2ad-154">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="dd2ad-155">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-155">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="dd2ad-156">Свойства определения политики обнаружения домашней области</span><span class="sxs-lookup"><span data-stu-id="dd2ad-156">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="dd2ad-157">Свойства, приведенные ниже, формируют объект JSON, представляющий политику времени существования маркеров.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="dd2ad-158">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="dd2ad-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="dd2ad-159">Ниже показан пример в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-159">An example is shown below in JSON format:</span></span>

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

| <span data-ttu-id="dd2ad-160">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd2ad-160">Property</span></span>     | <span data-ttu-id="dd2ad-161">Тип</span><span class="sxs-lookup"><span data-stu-id="dd2ad-161">Type</span></span>   |<span data-ttu-id="dd2ad-162">Описание</span><span class="sxs-lookup"><span data-stu-id="dd2ad-162">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="dd2ad-163">акцелератетофедератеддомаин</span><span class="sxs-lookup"><span data-stu-id="dd2ad-163">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="dd2ad-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd2ad-164">Boolean</span></span>| <span data-ttu-id="dd2ad-165">Задано `true` значение для автоускорения (обход поиска домашних областей).</span><span class="sxs-lookup"><span data-stu-id="dd2ad-165">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="dd2ad-166">Если `true` в клиенте есть только один проверенный и федеративный домен, то пользователи будут передаваться непосредственно поставщику федеративного удостоверения (например, ADFS) для входа.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-166">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="dd2ad-167">Если `true` в клиенте имеется несколько проверенных доменов, необходимо указать **преферреддомаин** .</span><span class="sxs-lookup"><span data-stu-id="dd2ad-167">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="dd2ad-168">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-168">Optional.</span></span>|
|<span data-ttu-id="dd2ad-169">преферреддомаин</span><span class="sxs-lookup"><span data-stu-id="dd2ad-169">PreferredDomain</span></span>|<span data-ttu-id="dd2ad-170">String</span><span class="sxs-lookup"><span data-stu-id="dd2ad-170">String</span></span>| <span data-ttu-id="dd2ad-171">Указывает домен для ускорения входа в систему.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-171">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="dd2ad-172">Его можно опустить, если у клиента только один федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-172">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="dd2ad-173">Если он не указан и существует несколько проверенных федеративных доменов, эта политика не оказывает никакого действия.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-173">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="dd2ad-174">Обязательный **AccelerateToFederatedDomain** , если `true`акцелератетофедератеддомаин —.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-174">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="dd2ad-175">алловклаудпассвордвалидатион</span><span class="sxs-lookup"><span data-stu-id="dd2ad-175">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="dd2ad-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd2ad-176">Boolean</span></span>| <span data-ttu-id="dd2ad-177">`true` Чтобы разрешить приложению выполнять проверку подлинности федеративного пользователя, указав учетные данные имени пользователя и пароля непосредственно в конечной точке маркера Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-177">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="dd2ad-178">Работает, только если включена синхронизация хэша паролей.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-178">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="dd2ad-179">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-179">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd2ad-180">Связи</span><span class="sxs-lookup"><span data-stu-id="dd2ad-180">Relationships</span></span>

| <span data-ttu-id="dd2ad-181">Связь</span><span class="sxs-lookup"><span data-stu-id="dd2ad-181">Relationship</span></span> | <span data-ttu-id="dd2ad-182">Тип</span><span class="sxs-lookup"><span data-stu-id="dd2ad-182">Type</span></span>        | <span data-ttu-id="dd2ad-183">Описание</span><span class="sxs-lookup"><span data-stu-id="dd2ad-183">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd2ad-184">Тег</span><span class="sxs-lookup"><span data-stu-id="dd2ad-184">appliesTo</span></span>|<span data-ttu-id="dd2ad-185">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="dd2ad-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="dd2ad-186">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-186">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="dd2ad-187">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-187">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd2ad-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd2ad-188">JSON representation</span></span>

<span data-ttu-id="dd2ad-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd2ad-189">The following is a JSON representation of the resource.</span></span>

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