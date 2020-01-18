---
title: Тип ресурса Хомереалмдисковериполици
description: Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 62b0735fbf7d927cf7ee417a81a54a8cb5eb2473
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234509"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="596b1-103">Тип ресурса Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="596b1-103">homeRealmDiscoveryPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="596b1-104">Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федеративных доменах.</span><span class="sxs-lookup"><span data-stu-id="596b1-104">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="596b1-105">Вы можете настроить Хомереалмдисковериполици для всех субъектов службы в организации или для определенных субъектов службы в Организации.</span><span class="sxs-lookup"><span data-stu-id="596b1-105">You can set homeRealmDiscoveryPolicy for all service principals in your organization, or for specific service principals in your organization.</span></span>  <span data-ttu-id="596b1-106">Дополнительные сведения о сценариях и политиках приведены [в статье Настройка режима входа в Azure AD для приложения с помощью политики обнаружения домашней области](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span><span class="sxs-lookup"><span data-stu-id="596b1-106">For more scenario and policy details see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span></span>

<span data-ttu-id="596b1-107">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="596b1-107">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="596b1-108">Методы</span><span class="sxs-lookup"><span data-stu-id="596b1-108">Methods</span></span>

| <span data-ttu-id="596b1-109">Метод</span><span class="sxs-lookup"><span data-stu-id="596b1-109">Method</span></span>       | <span data-ttu-id="596b1-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="596b1-110">Return Type</span></span> | <span data-ttu-id="596b1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="596b1-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="596b1-112">Создание Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="596b1-112">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="596b1-113">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="596b1-113">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="596b1-114">Создание объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="596b1-114">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="596b1-115">Получение Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="596b1-115">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="596b1-116">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="596b1-116">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="596b1-117">Чтение свойств и связей объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="596b1-117">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="596b1-118">Список ХомереалмдисковериполиЦиес</span><span class="sxs-lookup"><span data-stu-id="596b1-118">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="596b1-119">хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="596b1-119">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="596b1-120">Чтение свойств и связей объектов ХомереалмдисковериполиЦиес.</span><span class="sxs-lookup"><span data-stu-id="596b1-120">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="596b1-121">Обновление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="596b1-121">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="596b1-122">Нет</span><span class="sxs-lookup"><span data-stu-id="596b1-122">None</span></span> | <span data-ttu-id="596b1-123">Обновление объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="596b1-123">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="596b1-124">Удаление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="596b1-124">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="596b1-125">Нет</span><span class="sxs-lookup"><span data-stu-id="596b1-125">None</span></span> | <span data-ttu-id="596b1-126">Удаление объекта Хомереалмдисковериполици.</span><span class="sxs-lookup"><span data-stu-id="596b1-126">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="596b1-127">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="596b1-127">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="596b1-128">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="596b1-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="596b1-129">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="596b1-129">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="596b1-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="596b1-130">Properties</span></span>

| <span data-ttu-id="596b1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="596b1-131">Property</span></span>     | <span data-ttu-id="596b1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="596b1-132">Type</span></span>        | <span data-ttu-id="596b1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="596b1-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="596b1-134">id</span><span class="sxs-lookup"><span data-stu-id="596b1-134">id</span></span>|<span data-ttu-id="596b1-135">String</span><span class="sxs-lookup"><span data-stu-id="596b1-135">String</span></span>| <span data-ttu-id="596b1-136">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="596b1-136">Unique identifier for this policy.</span></span> <span data-ttu-id="596b1-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="596b1-137">Read-only.</span></span>|
|<span data-ttu-id="596b1-138">RDLC</span><span class="sxs-lookup"><span data-stu-id="596b1-138">definition</span></span>|<span data-ttu-id="596b1-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="596b1-139">String collection</span></span>| <span data-ttu-id="596b1-140">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="596b1-140">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="596b1-141">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="596b1-141">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="596b1-142">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="596b1-142">Required.</span></span>|
|<span data-ttu-id="596b1-143">description</span><span class="sxs-lookup"><span data-stu-id="596b1-143">description</span></span>|<span data-ttu-id="596b1-144">String</span><span class="sxs-lookup"><span data-stu-id="596b1-144">String</span></span>| <span data-ttu-id="596b1-145">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="596b1-145">Description for this policy.</span></span>|
|<span data-ttu-id="596b1-146">displayName</span><span class="sxs-lookup"><span data-stu-id="596b1-146">displayName</span></span>|<span data-ttu-id="596b1-147">Строка</span><span class="sxs-lookup"><span data-stu-id="596b1-147">String</span></span>| <span data-ttu-id="596b1-148">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="596b1-148">Display name for this policy.</span></span> <span data-ttu-id="596b1-149">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="596b1-149">Required.</span></span>|
|<span data-ttu-id="596b1-150">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="596b1-150">isOrganizationDefault</span></span>|<span data-ttu-id="596b1-151">Логический</span><span class="sxs-lookup"><span data-stu-id="596b1-151">Boolean</span></span>|<span data-ttu-id="596b1-152">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="596b1-152">If set to true, activates this policy.</span></span> <span data-ttu-id="596b1-153">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="596b1-153">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="596b1-154">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="596b1-154">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="596b1-155">Свойства определения политики обнаружения домашней области</span><span class="sxs-lookup"><span data-stu-id="596b1-155">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="596b1-156">Свойства, приведенные ниже, формируют объект JSON, представляющий политику времени существования маркеров.</span><span class="sxs-lookup"><span data-stu-id="596b1-156">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="596b1-157">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="596b1-157">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="596b1-158">Ниже показан пример в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="596b1-158">An example is shown below in JSON format:</span></span>

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

| <span data-ttu-id="596b1-159">Свойство</span><span class="sxs-lookup"><span data-stu-id="596b1-159">Property</span></span>     | <span data-ttu-id="596b1-160">Тип</span><span class="sxs-lookup"><span data-stu-id="596b1-160">Type</span></span>   |<span data-ttu-id="596b1-161">Описание</span><span class="sxs-lookup"><span data-stu-id="596b1-161">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="596b1-162">акцелератетофедератеддомаин</span><span class="sxs-lookup"><span data-stu-id="596b1-162">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="596b1-163">Логический</span><span class="sxs-lookup"><span data-stu-id="596b1-163">Boolean</span></span>| <span data-ttu-id="596b1-164">Задано `true` значение для автоускорения (обход поиска домашних областей).</span><span class="sxs-lookup"><span data-stu-id="596b1-164">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="596b1-165">Если `true` в клиенте есть только один проверенный и федеративный домен, то пользователи будут передаваться непосредственно поставщику федеративного удостоверения (например, ADFS) для входа.</span><span class="sxs-lookup"><span data-stu-id="596b1-165">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="596b1-166">Если `true` в клиенте имеется несколько проверенных доменов, необходимо указать **преферреддомаин** .</span><span class="sxs-lookup"><span data-stu-id="596b1-166">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="596b1-167">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="596b1-167">Optional.</span></span>|
|<span data-ttu-id="596b1-168">преферреддомаин</span><span class="sxs-lookup"><span data-stu-id="596b1-168">PreferredDomain</span></span>|<span data-ttu-id="596b1-169">String</span><span class="sxs-lookup"><span data-stu-id="596b1-169">String</span></span>| <span data-ttu-id="596b1-170">Указывает домен для ускорения входа в систему.</span><span class="sxs-lookup"><span data-stu-id="596b1-170">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="596b1-171">Его можно опустить, если у клиента только один федеративный домен.</span><span class="sxs-lookup"><span data-stu-id="596b1-171">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="596b1-172">Если он не указан и существует несколько проверенных федеративных доменов, эта политика не оказывает никакого действия.</span><span class="sxs-lookup"><span data-stu-id="596b1-172">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="596b1-173">Обязательный \*\*\*\* , если `true`акцелератетофедератеддомаин —.</span><span class="sxs-lookup"><span data-stu-id="596b1-173">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="596b1-174">алловклаудпассвордвалидатион</span><span class="sxs-lookup"><span data-stu-id="596b1-174">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="596b1-175">Логический</span><span class="sxs-lookup"><span data-stu-id="596b1-175">Boolean</span></span>| <span data-ttu-id="596b1-176">`true` Чтобы разрешить приложению выполнять проверку подлинности федеративного пользователя, указав учетные данные имени пользователя и пароля непосредственно в конечной точке маркера Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="596b1-176">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="596b1-177">Работает, только если включена синхронизация хэша паролей.</span><span class="sxs-lookup"><span data-stu-id="596b1-177">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="596b1-178">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="596b1-178">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="596b1-179">Связи</span><span class="sxs-lookup"><span data-stu-id="596b1-179">Relationships</span></span>

| <span data-ttu-id="596b1-180">Связь</span><span class="sxs-lookup"><span data-stu-id="596b1-180">Relationship</span></span> | <span data-ttu-id="596b1-181">Тип</span><span class="sxs-lookup"><span data-stu-id="596b1-181">Type</span></span>        | <span data-ttu-id="596b1-182">Описание</span><span class="sxs-lookup"><span data-stu-id="596b1-182">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="596b1-183">Тег</span><span class="sxs-lookup"><span data-stu-id="596b1-183">appliesTo</span></span>|<span data-ttu-id="596b1-184">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="596b1-184">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="596b1-185">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="596b1-185">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="596b1-186">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="596b1-186">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="596b1-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="596b1-187">JSON representation</span></span>

<span data-ttu-id="596b1-188">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="596b1-188">The following is a JSON representation of the resource.</span></span>

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