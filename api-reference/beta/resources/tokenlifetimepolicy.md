---
title: Тип ресурса tokenLifetimePolicy
description: Представляет политику, которая может управлять сроком действия маркера доступа, выданного Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bcfe06a8a42db4b0cfd5c8dab8da2b753e195f2c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155512"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="dc7a9-103">Тип ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dc7a9-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="dc7a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc7a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc7a9-105">Представляет политику, которая может управлять сроком действия маркера доступа JWT, маркера ИД или маркера SAML 1.1/2.0, выданного Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="dc7a9-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="dc7a9-106">Жизненный цикл маркера можно задать для всех приложений в вашей организации, мультитенантного приложения (охватывающего несколько организаций) или отдельного субъекта-службы в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="dc7a9-107">Дополнительные сведения о сценарии см. в сведениях [о настраиваемых сроках действия маркеров в Azure Active Directory.](/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="dc7a9-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="dc7a9-108">Примечание. Настройка этой политики для маркеров обновления и маркеров сеансов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-108">Note: Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="dc7a9-109">Наследуется от [stsPolicy.](stsPolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dc7a9-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dc7a9-110">Методы</span><span class="sxs-lookup"><span data-stu-id="dc7a9-110">Methods</span></span>

| <span data-ttu-id="dc7a9-111">Метод</span><span class="sxs-lookup"><span data-stu-id="dc7a9-111">Method</span></span>       | <span data-ttu-id="dc7a9-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dc7a9-112">Return Type</span></span> | <span data-ttu-id="dc7a9-113">Описание</span><span class="sxs-lookup"><span data-stu-id="dc7a9-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dc7a9-114">Создание tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dc7a9-114">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="dc7a9-115">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dc7a9-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="dc7a9-116">Создание объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-116">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="dc7a9-117">Get tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dc7a9-117">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="dc7a9-118">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dc7a9-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="dc7a9-119">Чтение свойств и связей объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-119">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="dc7a9-120">Перечисление типов ресурсов tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dc7a9-120">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="dc7a9-121">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dc7a9-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="dc7a9-122">Чтение свойств и связей объектов tokenLifetimePolicies.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-122">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="dc7a9-123">Обновление tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dc7a9-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="dc7a9-124">Нет</span><span class="sxs-lookup"><span data-stu-id="dc7a9-124">None</span></span> | <span data-ttu-id="dc7a9-125">Обновление объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="dc7a9-126">Удаление tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dc7a9-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="dc7a9-127">Нет</span><span class="sxs-lookup"><span data-stu-id="dc7a9-127">None</span></span> | <span data-ttu-id="dc7a9-128">Удаление объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="dc7a9-129">List appliesTo</span><span class="sxs-lookup"><span data-stu-id="dc7a9-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="dc7a9-130">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="dc7a9-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="dc7a9-131">Получите список directoryObjects, к которые была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="dc7a9-132">Назначение типа ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dc7a9-132">Assign tokenLifetimePolicy</span></span>](../api/application-post-tokenlifetimepolicies.md) | <span data-ttu-id="dc7a9-133">Нет</span><span class="sxs-lookup"><span data-stu-id="dc7a9-133">None</span></span> | <span data-ttu-id="dc7a9-134">Назначьте объект tokenLifetimePolicy [объекту application](application.md) или [servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="dc7a9-134">Assign a tokenLifetimePolicy object to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="dc7a9-135">Список assigned tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dc7a9-135">List assigned tokenLifetimePolicy</span></span>](../api/application-list-tokenlifetimepolicies.md) | <span data-ttu-id="dc7a9-136">Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dc7a9-136">[tokenLifetimePolicy](tokenlifetimepolicy.md) collection</span></span> | <span data-ttu-id="dc7a9-137">Список объектов tokenLifetimePolicy, которые назначены объекту [application](application.md) или [servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="dc7a9-137">List the tokenLifetimePolicy objects that are assigned to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="dc7a9-138">Удаление типа ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dc7a9-138">Remove tokenLifetimePolicy</span></span>](../api/application-delete-tokenlifetimepolicies.md) | <span data-ttu-id="dc7a9-139">Нет</span><span class="sxs-lookup"><span data-stu-id="dc7a9-139">None</span></span> | <span data-ttu-id="dc7a9-140">Удаление объекта tokenLifetimePolicy из [объекта application](application.md) или [servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="dc7a9-140">Remove a tokenLifetimePolicy object from an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dc7a9-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc7a9-141">Properties</span></span>

| <span data-ttu-id="dc7a9-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc7a9-142">Property</span></span>     | <span data-ttu-id="dc7a9-143">Тип</span><span class="sxs-lookup"><span data-stu-id="dc7a9-143">Type</span></span>        | <span data-ttu-id="dc7a9-144">Описание</span><span class="sxs-lookup"><span data-stu-id="dc7a9-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dc7a9-145">id</span><span class="sxs-lookup"><span data-stu-id="dc7a9-145">id</span></span>|<span data-ttu-id="dc7a9-146">String</span><span class="sxs-lookup"><span data-stu-id="dc7a9-146">String</span></span>| <span data-ttu-id="dc7a9-147">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-147">Unique identifier for this policy.</span></span> <span data-ttu-id="dc7a9-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-148">Read-only.</span></span>|
|<span data-ttu-id="dc7a9-149">definition</span><span class="sxs-lookup"><span data-stu-id="dc7a9-149">definition</span></span>|<span data-ttu-id="dc7a9-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dc7a9-150">String collection</span></span>| <span data-ttu-id="dc7a9-151">Коллекция строк, содержащая строку JSON, которая определяет правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-151">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="dc7a9-152">Дополнительные сведения о схеме JSON для этого свойства см. ниже.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-152">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="dc7a9-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-153">Required.</span></span>|
|<span data-ttu-id="dc7a9-154">description</span><span class="sxs-lookup"><span data-stu-id="dc7a9-154">description</span></span>|<span data-ttu-id="dc7a9-155">String</span><span class="sxs-lookup"><span data-stu-id="dc7a9-155">String</span></span>| <span data-ttu-id="dc7a9-156">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-156">Description for this policy.</span></span>|
|<span data-ttu-id="dc7a9-157">displayName</span><span class="sxs-lookup"><span data-stu-id="dc7a9-157">displayName</span></span>|<span data-ttu-id="dc7a9-158">String</span><span class="sxs-lookup"><span data-stu-id="dc7a9-158">String</span></span>| <span data-ttu-id="dc7a9-159">Отображаемого имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-159">Display name for this policy.</span></span> <span data-ttu-id="dc7a9-160">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-160">Required.</span></span>|
|<span data-ttu-id="dc7a9-161">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="dc7a9-161">isOrganizationDefault</span></span>|<span data-ttu-id="dc7a9-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc7a9-162">Boolean</span></span>|<span data-ttu-id="dc7a9-163">Если установлено true, активирует эту политику.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-163">If set to true, activates this policy.</span></span> <span data-ttu-id="dc7a9-164">Для одного типа политики может быть несколько политик, но только одна может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-164">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="dc7a9-165">Необязательный, значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-165">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="dc7a9-166">Свойства определения политики жизненного срока действия маркера</span><span class="sxs-lookup"><span data-stu-id="dc7a9-166">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="dc7a9-167">Ниже properties form the JSON object that represents a token lifetime policy.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-167">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="dc7a9-168">Этот объект JSON необходимо **преобразовать** в строку с escape-кавычками, чтобы вставить его в **свойство** определения.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-168">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="dc7a9-169">Пример показан ниже в формате JSON:</span><span class="sxs-lookup"><span data-stu-id="dc7a9-169">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="dc7a9-170">Примечание. Все сроки в этих свойствах заданы в формате "дд.чч:мм:сс".</span><span class="sxs-lookup"><span data-stu-id="dc7a9-170">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="dc7a9-171">Примечание. Максимальное количество свойств, обозначаемого в "днях", составляет 1 секунду от заметимого количества дней.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-171">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="dc7a9-172">Например, максимальное значение 1 дня указывается как "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="dc7a9-172">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="dc7a9-173">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc7a9-173">Property</span></span>     | <span data-ttu-id="dc7a9-174">Тип</span><span class="sxs-lookup"><span data-stu-id="dc7a9-174">Type</span></span>   |<span data-ttu-id="dc7a9-175">Описание</span><span class="sxs-lookup"><span data-stu-id="dc7a9-175">Description</span></span>| <span data-ttu-id="dc7a9-176">Min Value</span><span class="sxs-lookup"><span data-stu-id="dc7a9-176">Min Value</span></span> | <span data-ttu-id="dc7a9-177">Максимальное значение</span><span class="sxs-lookup"><span data-stu-id="dc7a9-177">Max Value</span></span> | <span data-ttu-id="dc7a9-178">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="dc7a9-178">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="dc7a9-179">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="dc7a9-179">AccessTokenLifetime</span></span>|<span data-ttu-id="dc7a9-180">String</span><span class="sxs-lookup"><span data-stu-id="dc7a9-180">String</span></span>|<span data-ttu-id="dc7a9-181">Управляет тем, как долго маркеры доступа и маркеры ID считаются допустимым.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-181">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="dc7a9-182">10 минут</span><span class="sxs-lookup"><span data-stu-id="dc7a9-182">10 minutes</span></span>|<span data-ttu-id="dc7a9-183">1 день</span><span class="sxs-lookup"><span data-stu-id="dc7a9-183">1 day</span></span>|<span data-ttu-id="dc7a9-184">1 час</span><span class="sxs-lookup"><span data-stu-id="dc7a9-184">1 hour</span></span>|
|<span data-ttu-id="dc7a9-185">Версия</span><span class="sxs-lookup"><span data-stu-id="dc7a9-185">Version</span></span>|<span data-ttu-id="dc7a9-186">Целое число</span><span class="sxs-lookup"><span data-stu-id="dc7a9-186">Integer</span></span>|<span data-ttu-id="dc7a9-187">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-187">Set value of 1.</span></span> <span data-ttu-id="dc7a9-188">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-188">Required.</span></span>|<span data-ttu-id="dc7a9-189">Нет</span><span class="sxs-lookup"><span data-stu-id="dc7a9-189">None</span></span>|<span data-ttu-id="dc7a9-190">Нет</span><span class="sxs-lookup"><span data-stu-id="dc7a9-190">None</span></span>|<span data-ttu-id="dc7a9-191">Нет</span><span class="sxs-lookup"><span data-stu-id="dc7a9-191">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc7a9-192">Связи</span><span class="sxs-lookup"><span data-stu-id="dc7a9-192">Relationships</span></span>

| <span data-ttu-id="dc7a9-193">Связь</span><span class="sxs-lookup"><span data-stu-id="dc7a9-193">Relationship</span></span> | <span data-ttu-id="dc7a9-194">Тип</span><span class="sxs-lookup"><span data-stu-id="dc7a9-194">Type</span></span>        | <span data-ttu-id="dc7a9-195">Описание</span><span class="sxs-lookup"><span data-stu-id="dc7a9-195">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dc7a9-196">appliesTo</span><span class="sxs-lookup"><span data-stu-id="dc7a9-196">appliesTo</span></span>|<span data-ttu-id="dc7a9-197">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="dc7a9-197">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="dc7a9-198">Коллекция [directoryObject,](directoryObject.md) к которую применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-198">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="dc7a9-199">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-199">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc7a9-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc7a9-200">JSON representation</span></span>

<span data-ttu-id="dc7a9-201">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc7a9-201">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
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
  "description": "tokenLifetimePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->