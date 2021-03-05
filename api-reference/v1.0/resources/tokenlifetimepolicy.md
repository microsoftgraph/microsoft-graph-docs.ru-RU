---
title: тип ресурса tokenLifetimePolicy
description: Представляет политику, которая может контролировать срок службы маркера доступа, выданного Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f950ce0c5a269aee5159349c76e9bea1c4c7a505
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442504"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="45211-103">тип ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="45211-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="45211-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45211-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="45211-105">Представляет политику, которая может контролировать срок службы маркера доступа JWT, маркера ID или маркера SAML 1.1/2.0, выданного Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="45211-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="45211-106">Жизненный цикл маркера можно задать для всех приложений в вашей организации, мультитенантного приложения (охватывающего несколько организаций) или отдельного субъекта-службы в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="45211-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="45211-107">Дополнительные сведения о сценарии см. [в материале Configurable token lifetimes in Azure Active Directory.](/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="45211-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="45211-108">**Примечание:** Настройка этой политики для маркеров обновления и маркеров сеансов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45211-108">**Note:** Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="45211-109">Наследует [от stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="45211-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="45211-110">Методы</span><span class="sxs-lookup"><span data-stu-id="45211-110">Methods</span></span>

| <span data-ttu-id="45211-111">Метод</span><span class="sxs-lookup"><span data-stu-id="45211-111">Method</span></span>       | <span data-ttu-id="45211-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="45211-112">Return Type</span></span> | <span data-ttu-id="45211-113">Описание</span><span class="sxs-lookup"><span data-stu-id="45211-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="45211-114">Перечисление типов ресурсов tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="45211-114">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="45211-115">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="45211-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="45211-116">Чтение свойств и связей объектов tokenLifetimePolicies.</span><span class="sxs-lookup"><span data-stu-id="45211-116">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="45211-117">Создание tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="45211-117">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="45211-118">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="45211-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="45211-119">Создание объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="45211-119">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="45211-120">Get tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="45211-120">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="45211-121">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="45211-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="45211-122">Чтение свойств и связей объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="45211-122">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="45211-123">Обновление tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="45211-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="45211-124">Нет</span><span class="sxs-lookup"><span data-stu-id="45211-124">None</span></span> | <span data-ttu-id="45211-125">Обновление объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="45211-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="45211-126">Удаление tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="45211-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="45211-127">Нет</span><span class="sxs-lookup"><span data-stu-id="45211-127">None</span></span> | <span data-ttu-id="45211-128">Удаление объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="45211-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="45211-129">Список применяетсяTo</span><span class="sxs-lookup"><span data-stu-id="45211-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="45211-130">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="45211-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="45211-131">Получите список directoryObjects, к которые была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="45211-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="45211-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="45211-132">Properties</span></span>

| <span data-ttu-id="45211-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="45211-133">Property</span></span>     | <span data-ttu-id="45211-134">Тип</span><span class="sxs-lookup"><span data-stu-id="45211-134">Type</span></span>        | <span data-ttu-id="45211-135">Описание</span><span class="sxs-lookup"><span data-stu-id="45211-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="45211-136">id</span><span class="sxs-lookup"><span data-stu-id="45211-136">id</span></span>|<span data-ttu-id="45211-137">String</span><span class="sxs-lookup"><span data-stu-id="45211-137">String</span></span>| <span data-ttu-id="45211-138">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="45211-138">Unique identifier for this policy.</span></span> <span data-ttu-id="45211-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="45211-139">Read-only.</span></span>|
|<span data-ttu-id="45211-140">определение</span><span class="sxs-lookup"><span data-stu-id="45211-140">definition</span></span>|<span data-ttu-id="45211-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="45211-141">String collection</span></span>| <span data-ttu-id="45211-142">Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики.</span><span class="sxs-lookup"><span data-stu-id="45211-142">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="45211-143">Дополнительные сведения о схеме JSON для этого свойства см. ниже.</span><span class="sxs-lookup"><span data-stu-id="45211-143">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="45211-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45211-144">Required.</span></span>|
|<span data-ttu-id="45211-145">description</span><span class="sxs-lookup"><span data-stu-id="45211-145">description</span></span>|<span data-ttu-id="45211-146">String</span><span class="sxs-lookup"><span data-stu-id="45211-146">String</span></span>| <span data-ttu-id="45211-147">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="45211-147">Description for this policy.</span></span>|
|<span data-ttu-id="45211-148">displayName</span><span class="sxs-lookup"><span data-stu-id="45211-148">displayName</span></span>|<span data-ttu-id="45211-149">String</span><span class="sxs-lookup"><span data-stu-id="45211-149">String</span></span>| <span data-ttu-id="45211-150">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="45211-150">Display name for this policy.</span></span> <span data-ttu-id="45211-151">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="45211-151">Required.</span></span>|
|<span data-ttu-id="45211-152">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="45211-152">isOrganizationDefault</span></span>|<span data-ttu-id="45211-153">Логический</span><span class="sxs-lookup"><span data-stu-id="45211-153">Boolean</span></span>|<span data-ttu-id="45211-154">Если заданной для true, активирует эту политику.</span><span class="sxs-lookup"><span data-stu-id="45211-154">If set to true, activates this policy.</span></span> <span data-ttu-id="45211-155">Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации.</span><span class="sxs-lookup"><span data-stu-id="45211-155">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="45211-156">Необязательный, значение по умолчанию является ложным.</span><span class="sxs-lookup"><span data-stu-id="45211-156">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="45211-157">Свойства определения политики жизни маркера</span><span class="sxs-lookup"><span data-stu-id="45211-157">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="45211-158">Свойства, представленные ниже, формируют объект JSON, который представляет политику срока службы маркера.</span><span class="sxs-lookup"><span data-stu-id="45211-158">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="45211-159">Этот объект JSON необходимо **преобразовать** в строку с кавычками, которые будут вставлены в **свойство определения.**</span><span class="sxs-lookup"><span data-stu-id="45211-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="45211-160">Пример показан ниже в формате JSON:</span><span class="sxs-lookup"><span data-stu-id="45211-160">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="45211-161">**Примечание:** Все периоды времени в этих свойствах указаны в формате "dd.hh:mm:ss".</span><span class="sxs-lookup"><span data-stu-id="45211-161">**Note:** All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="45211-162">**Примечание:** Максимальные значения свойств, обозначаемого в "днях", на 1 секунду меньше замечаемого числа дней.</span><span class="sxs-lookup"><span data-stu-id="45211-162">**Note:** Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="45211-163">Например, максимальное значение 1 дня указывается как "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="45211-163">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="45211-164">Свойство</span><span class="sxs-lookup"><span data-stu-id="45211-164">Property</span></span>     | <span data-ttu-id="45211-165">Тип</span><span class="sxs-lookup"><span data-stu-id="45211-165">Type</span></span>   |<span data-ttu-id="45211-166">Описание</span><span class="sxs-lookup"><span data-stu-id="45211-166">Description</span></span>| <span data-ttu-id="45211-167">Значение Min</span><span class="sxs-lookup"><span data-stu-id="45211-167">Min Value</span></span> | <span data-ttu-id="45211-168">Максимальное значение</span><span class="sxs-lookup"><span data-stu-id="45211-168">Max Value</span></span> | <span data-ttu-id="45211-169">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="45211-169">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="45211-170">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="45211-170">AccessTokenLifetime</span></span>|<span data-ttu-id="45211-171">String</span><span class="sxs-lookup"><span data-stu-id="45211-171">String</span></span>|<span data-ttu-id="45211-172">Контролирует, как долго и доступ, и маркеры ID считаются допустимыми.</span><span class="sxs-lookup"><span data-stu-id="45211-172">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="45211-173">10 минут</span><span class="sxs-lookup"><span data-stu-id="45211-173">10 minutes</span></span>|<span data-ttu-id="45211-174">1 день</span><span class="sxs-lookup"><span data-stu-id="45211-174">1 day</span></span>|<span data-ttu-id="45211-175">1 час</span><span class="sxs-lookup"><span data-stu-id="45211-175">1 hour</span></span>|
|<span data-ttu-id="45211-176">Версия</span><span class="sxs-lookup"><span data-stu-id="45211-176">Version</span></span>|<span data-ttu-id="45211-177">Целое число</span><span class="sxs-lookup"><span data-stu-id="45211-177">Integer</span></span>|<span data-ttu-id="45211-178">Значение 1.</span><span class="sxs-lookup"><span data-stu-id="45211-178">Set value of 1.</span></span> <span data-ttu-id="45211-179">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="45211-179">Required.</span></span>|<span data-ttu-id="45211-180">Нет</span><span class="sxs-lookup"><span data-stu-id="45211-180">None</span></span>|<span data-ttu-id="45211-181">Нет</span><span class="sxs-lookup"><span data-stu-id="45211-181">None</span></span>|<span data-ttu-id="45211-182">Нет</span><span class="sxs-lookup"><span data-stu-id="45211-182">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="45211-183">Связи</span><span class="sxs-lookup"><span data-stu-id="45211-183">Relationships</span></span>

| <span data-ttu-id="45211-184">Связь</span><span class="sxs-lookup"><span data-stu-id="45211-184">Relationship</span></span> | <span data-ttu-id="45211-185">Тип</span><span class="sxs-lookup"><span data-stu-id="45211-185">Type</span></span>        | <span data-ttu-id="45211-186">Описание</span><span class="sxs-lookup"><span data-stu-id="45211-186">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="45211-187">appliesTo</span><span class="sxs-lookup"><span data-stu-id="45211-187">appliesTo</span></span>|<span data-ttu-id="45211-188">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="45211-188">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="45211-189">Коллекция [directoryObject,](directoryObject.md) к которую была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="45211-189">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="45211-190">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="45211-190">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45211-191">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45211-191">JSON representation</span></span>

<span data-ttu-id="45211-192">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45211-192">The following is a JSON representation of the resource.</span></span>

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
