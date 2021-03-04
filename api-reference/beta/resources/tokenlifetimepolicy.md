---
title: тип ресурса tokenLifetimePolicy
description: Представляет политику, которая может контролировать срок службы маркера доступа, выданного Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: dfe225a5d79551d7312a7ef22daa976d5d75e38b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442777"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="aa2b8-103">тип ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="aa2b8-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="aa2b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa2b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa2b8-105">Представляет политику, которая может контролировать срок службы маркера доступа JWT, маркера ID или маркера SAML 1.1/2.0, выданного Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="aa2b8-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="aa2b8-106">Жизненный цикл маркера можно задать для всех приложений в вашей организации, мультитенантного приложения (охватывающего несколько организаций) или отдельного субъекта-службы в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="aa2b8-107">Дополнительные сведения о сценарии см. [в материале Configurable token lifetimes in Azure Active Directory.](/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="aa2b8-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="aa2b8-108">Примечание. Настройка этой политики для маркеров обновления и маркеров сеансов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-108">Note: Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="aa2b8-109">Наследует [от stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aa2b8-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="aa2b8-110">Методы</span><span class="sxs-lookup"><span data-stu-id="aa2b8-110">Methods</span></span>

| <span data-ttu-id="aa2b8-111">Метод</span><span class="sxs-lookup"><span data-stu-id="aa2b8-111">Method</span></span>       | <span data-ttu-id="aa2b8-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aa2b8-112">Return Type</span></span> | <span data-ttu-id="aa2b8-113">Описание</span><span class="sxs-lookup"><span data-stu-id="aa2b8-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="aa2b8-114">Создание tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="aa2b8-114">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="aa2b8-115">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="aa2b8-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="aa2b8-116">Создание объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-116">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="aa2b8-117">Get tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="aa2b8-117">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="aa2b8-118">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="aa2b8-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="aa2b8-119">Чтение свойств и связей объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-119">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="aa2b8-120">Перечисление типов ресурсов tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="aa2b8-120">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="aa2b8-121">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="aa2b8-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="aa2b8-122">Чтение свойств и связей объектов tokenLifetimePolicies.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-122">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="aa2b8-123">Обновление tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="aa2b8-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="aa2b8-124">Нет</span><span class="sxs-lookup"><span data-stu-id="aa2b8-124">None</span></span> | <span data-ttu-id="aa2b8-125">Обновление объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="aa2b8-126">Удаление tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="aa2b8-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="aa2b8-127">Нет</span><span class="sxs-lookup"><span data-stu-id="aa2b8-127">None</span></span> | <span data-ttu-id="aa2b8-128">Удаление объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="aa2b8-129">Список применяетсяTo</span><span class="sxs-lookup"><span data-stu-id="aa2b8-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="aa2b8-130">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="aa2b8-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="aa2b8-131">Получите список directoryObjects, к которые была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="aa2b8-132">Назначение типа ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="aa2b8-132">Assign tokenLifetimePolicy</span></span>](../api/application-post-tokenlifetimepolicies.md) | <span data-ttu-id="aa2b8-133">Нет</span><span class="sxs-lookup"><span data-stu-id="aa2b8-133">None</span></span> | <span data-ttu-id="aa2b8-134">Назначьте объект tokenLifetimePolicy [приложению](application.md) или [объекту servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="aa2b8-134">Assign a tokenLifetimePolicy object to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="aa2b8-135">Список назначенного tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="aa2b8-135">List assigned tokenLifetimePolicy</span></span>](../api/application-list-tokenlifetimepolicies.md) | <span data-ttu-id="aa2b8-136">Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aa2b8-136">[tokenLifetimePolicy](tokenlifetimepolicy.md) collection</span></span> | <span data-ttu-id="aa2b8-137">Список объектов tokenLifetimePolicy, которые назначены объекту [приложения](application.md) или [servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="aa2b8-137">List the tokenLifetimePolicy objects that are assigned to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="aa2b8-138">Удаление типа ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="aa2b8-138">Remove tokenLifetimePolicy</span></span>](../api/application-delete-tokenlifetimepolicies.md) | <span data-ttu-id="aa2b8-139">Нет</span><span class="sxs-lookup"><span data-stu-id="aa2b8-139">None</span></span> | <span data-ttu-id="aa2b8-140">Удалите объект tokenLifetimePolicy из [приложения](application.md) или [объекта servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="aa2b8-140">Remove a tokenLifetimePolicy object from an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="aa2b8-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa2b8-141">Properties</span></span>

| <span data-ttu-id="aa2b8-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa2b8-142">Property</span></span>     | <span data-ttu-id="aa2b8-143">Тип</span><span class="sxs-lookup"><span data-stu-id="aa2b8-143">Type</span></span>        | <span data-ttu-id="aa2b8-144">Описание</span><span class="sxs-lookup"><span data-stu-id="aa2b8-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aa2b8-145">id</span><span class="sxs-lookup"><span data-stu-id="aa2b8-145">id</span></span>|<span data-ttu-id="aa2b8-146">String</span><span class="sxs-lookup"><span data-stu-id="aa2b8-146">String</span></span>| <span data-ttu-id="aa2b8-147">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-147">Unique identifier for this policy.</span></span> <span data-ttu-id="aa2b8-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-148">Read-only.</span></span>|
|<span data-ttu-id="aa2b8-149">определение</span><span class="sxs-lookup"><span data-stu-id="aa2b8-149">definition</span></span>|<span data-ttu-id="aa2b8-150">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="aa2b8-150">String collection</span></span>| <span data-ttu-id="aa2b8-151">Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-151">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="aa2b8-152">Дополнительные сведения о схеме JSON для этого свойства см. ниже.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-152">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="aa2b8-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-153">Required.</span></span>|
|<span data-ttu-id="aa2b8-154">description</span><span class="sxs-lookup"><span data-stu-id="aa2b8-154">description</span></span>|<span data-ttu-id="aa2b8-155">String</span><span class="sxs-lookup"><span data-stu-id="aa2b8-155">String</span></span>| <span data-ttu-id="aa2b8-156">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-156">Description for this policy.</span></span>|
|<span data-ttu-id="aa2b8-157">displayName</span><span class="sxs-lookup"><span data-stu-id="aa2b8-157">displayName</span></span>|<span data-ttu-id="aa2b8-158">String</span><span class="sxs-lookup"><span data-stu-id="aa2b8-158">String</span></span>| <span data-ttu-id="aa2b8-159">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-159">Display name for this policy.</span></span> <span data-ttu-id="aa2b8-160">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-160">Required.</span></span>|
|<span data-ttu-id="aa2b8-161">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="aa2b8-161">isOrganizationDefault</span></span>|<span data-ttu-id="aa2b8-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa2b8-162">Boolean</span></span>|<span data-ttu-id="aa2b8-163">Если заданной для true, активирует эту политику.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-163">If set to true, activates this policy.</span></span> <span data-ttu-id="aa2b8-164">Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-164">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="aa2b8-165">Необязательный, значение по умолчанию является ложным.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-165">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="aa2b8-166">Свойства определения политики жизни маркера</span><span class="sxs-lookup"><span data-stu-id="aa2b8-166">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="aa2b8-167">Свойства, представленные ниже, формируют объект JSON, который представляет политику срока службы маркера.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-167">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="aa2b8-168">Этот объект JSON необходимо **преобразовать** в строку с кавычками, которые будут вставлены в **свойство определения.**</span><span class="sxs-lookup"><span data-stu-id="aa2b8-168">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="aa2b8-169">Пример показан ниже в формате JSON:</span><span class="sxs-lookup"><span data-stu-id="aa2b8-169">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="aa2b8-170">Примечание. Все периоды времени в этих свойствах указаны в формате "dd.hh:mm:ss".</span><span class="sxs-lookup"><span data-stu-id="aa2b8-170">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="aa2b8-171">Примечание. Максимальные значения для свойств, обозначаемого в "днях", на 1 секунду меньше замечаемого числа дней.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-171">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="aa2b8-172">Например, максимальное значение 1 дня указывается как "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="aa2b8-172">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="aa2b8-173">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa2b8-173">Property</span></span>     | <span data-ttu-id="aa2b8-174">Тип</span><span class="sxs-lookup"><span data-stu-id="aa2b8-174">Type</span></span>   |<span data-ttu-id="aa2b8-175">Описание</span><span class="sxs-lookup"><span data-stu-id="aa2b8-175">Description</span></span>| <span data-ttu-id="aa2b8-176">Значение Min</span><span class="sxs-lookup"><span data-stu-id="aa2b8-176">Min Value</span></span> | <span data-ttu-id="aa2b8-177">Максимальное значение</span><span class="sxs-lookup"><span data-stu-id="aa2b8-177">Max Value</span></span> | <span data-ttu-id="aa2b8-178">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="aa2b8-178">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="aa2b8-179">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="aa2b8-179">AccessTokenLifetime</span></span>|<span data-ttu-id="aa2b8-180">String</span><span class="sxs-lookup"><span data-stu-id="aa2b8-180">String</span></span>|<span data-ttu-id="aa2b8-181">Контролирует, как долго и доступ, и маркеры ID считаются допустимыми.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-181">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="aa2b8-182">10 минут</span><span class="sxs-lookup"><span data-stu-id="aa2b8-182">10 minutes</span></span>|<span data-ttu-id="aa2b8-183">1 день</span><span class="sxs-lookup"><span data-stu-id="aa2b8-183">1 day</span></span>|<span data-ttu-id="aa2b8-184">1 час</span><span class="sxs-lookup"><span data-stu-id="aa2b8-184">1 hour</span></span>|
|<span data-ttu-id="aa2b8-185">Версия</span><span class="sxs-lookup"><span data-stu-id="aa2b8-185">Version</span></span>|<span data-ttu-id="aa2b8-186">Целое число</span><span class="sxs-lookup"><span data-stu-id="aa2b8-186">Integer</span></span>|<span data-ttu-id="aa2b8-187">Значение 1.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-187">Set value of 1.</span></span> <span data-ttu-id="aa2b8-188">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-188">Required.</span></span>|<span data-ttu-id="aa2b8-189">Нет</span><span class="sxs-lookup"><span data-stu-id="aa2b8-189">None</span></span>|<span data-ttu-id="aa2b8-190">Нет</span><span class="sxs-lookup"><span data-stu-id="aa2b8-190">None</span></span>|<span data-ttu-id="aa2b8-191">Нет</span><span class="sxs-lookup"><span data-stu-id="aa2b8-191">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa2b8-192">Связи</span><span class="sxs-lookup"><span data-stu-id="aa2b8-192">Relationships</span></span>

| <span data-ttu-id="aa2b8-193">Связь</span><span class="sxs-lookup"><span data-stu-id="aa2b8-193">Relationship</span></span> | <span data-ttu-id="aa2b8-194">Тип</span><span class="sxs-lookup"><span data-stu-id="aa2b8-194">Type</span></span>        | <span data-ttu-id="aa2b8-195">Описание</span><span class="sxs-lookup"><span data-stu-id="aa2b8-195">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aa2b8-196">appliesTo</span><span class="sxs-lookup"><span data-stu-id="aa2b8-196">appliesTo</span></span>|<span data-ttu-id="aa2b8-197">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="aa2b8-197">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="aa2b8-198">Коллекция [directoryObject,](directoryObject.md) к которую была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-198">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="aa2b8-199">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-199">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa2b8-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa2b8-200">JSON representation</span></span>

<span data-ttu-id="aa2b8-201">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa2b8-201">The following is a JSON representation of the resource.</span></span>

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
