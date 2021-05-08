---
title: тип ресурса tokenLifetimePolicy
description: Представляет политику, которая может контролировать срок службы маркера доступа, выданного Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d143faa87af81fbaae73973510bafe3fd3ee4fcb
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241046"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="f78ac-103">тип ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="f78ac-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="f78ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f78ac-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="f78ac-105">Представляет политику, которая может контролировать срок службы маркера доступа JWT, маркера ID или маркера SAML 1.1/2.0, выданного Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f78ac-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="f78ac-106">Жизненный цикл маркера можно задать для всех приложений в вашей организации, мультитенантного приложения (охватывающего несколько организаций) или отдельного субъекта-службы в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="f78ac-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> 

><span data-ttu-id="f78ac-107">**Примечание:** Настройка этой политики для маркеров обновления и маркеров сеансов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f78ac-107">**Note:** Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="f78ac-108">Наследует [от stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f78ac-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f78ac-109">Методы</span><span class="sxs-lookup"><span data-stu-id="f78ac-109">Methods</span></span>

| <span data-ttu-id="f78ac-110">Метод</span><span class="sxs-lookup"><span data-stu-id="f78ac-110">Method</span></span>       | <span data-ttu-id="f78ac-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f78ac-111">Return Type</span></span> | <span data-ttu-id="f78ac-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f78ac-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f78ac-113">Перечисление типов ресурсов tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="f78ac-113">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="f78ac-114">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="f78ac-114">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="f78ac-115">Чтение свойств и связей объектов tokenLifetimePolicies.</span><span class="sxs-lookup"><span data-stu-id="f78ac-115">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="f78ac-116">Создание tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="f78ac-116">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="f78ac-117">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="f78ac-117">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="f78ac-118">Создание объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="f78ac-118">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="f78ac-119">Get tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="f78ac-119">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="f78ac-120">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="f78ac-120">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="f78ac-121">Чтение свойств и связей объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="f78ac-121">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="f78ac-122">Обновление tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="f78ac-122">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="f78ac-123">Нет</span><span class="sxs-lookup"><span data-stu-id="f78ac-123">None</span></span> | <span data-ttu-id="f78ac-124">Обновление объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="f78ac-124">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="f78ac-125">Удаление tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="f78ac-125">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="f78ac-126">Нет</span><span class="sxs-lookup"><span data-stu-id="f78ac-126">None</span></span> | <span data-ttu-id="f78ac-127">Удаление объекта tokenLifetimePolicy.</span><span class="sxs-lookup"><span data-stu-id="f78ac-127">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="f78ac-128">Список применяетсяTo</span><span class="sxs-lookup"><span data-stu-id="f78ac-128">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="f78ac-129">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="f78ac-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="f78ac-130">Получите список directoryObjects, к которые была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="f78ac-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="f78ac-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="f78ac-131">Properties</span></span>

| <span data-ttu-id="f78ac-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="f78ac-132">Property</span></span>     | <span data-ttu-id="f78ac-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f78ac-133">Type</span></span>        | <span data-ttu-id="f78ac-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f78ac-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f78ac-135">id</span><span class="sxs-lookup"><span data-stu-id="f78ac-135">id</span></span>|<span data-ttu-id="f78ac-136">Строка</span><span class="sxs-lookup"><span data-stu-id="f78ac-136">String</span></span>| <span data-ttu-id="f78ac-137">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f78ac-137">Unique identifier for this policy.</span></span> <span data-ttu-id="f78ac-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f78ac-138">Read-only.</span></span>|
|<span data-ttu-id="f78ac-139">определение</span><span class="sxs-lookup"><span data-stu-id="f78ac-139">definition</span></span>|<span data-ttu-id="f78ac-140">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="f78ac-140">String collection</span></span>| <span data-ttu-id="f78ac-141">Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики.</span><span class="sxs-lookup"><span data-stu-id="f78ac-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="f78ac-142">Дополнительные сведения о схеме JSON для этого свойства см. ниже.</span><span class="sxs-lookup"><span data-stu-id="f78ac-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="f78ac-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f78ac-143">Required.</span></span>|
|<span data-ttu-id="f78ac-144">description</span><span class="sxs-lookup"><span data-stu-id="f78ac-144">description</span></span>|<span data-ttu-id="f78ac-145">Строка</span><span class="sxs-lookup"><span data-stu-id="f78ac-145">String</span></span>| <span data-ttu-id="f78ac-146">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="f78ac-146">Description for this policy.</span></span>|
|<span data-ttu-id="f78ac-147">displayName</span><span class="sxs-lookup"><span data-stu-id="f78ac-147">displayName</span></span>|<span data-ttu-id="f78ac-148">Строка</span><span class="sxs-lookup"><span data-stu-id="f78ac-148">String</span></span>| <span data-ttu-id="f78ac-149">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f78ac-149">Display name for this policy.</span></span> <span data-ttu-id="f78ac-150">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f78ac-150">Required.</span></span>|
|<span data-ttu-id="f78ac-151">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="f78ac-151">isOrganizationDefault</span></span>|<span data-ttu-id="f78ac-152">Логический</span><span class="sxs-lookup"><span data-stu-id="f78ac-152">Boolean</span></span>|<span data-ttu-id="f78ac-153">Если `true` установлено, активирует эту политику.</span><span class="sxs-lookup"><span data-stu-id="f78ac-153">If set to `true`, activates this policy.</span></span> <span data-ttu-id="f78ac-154">Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации.</span><span class="sxs-lookup"><span data-stu-id="f78ac-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="f78ac-155">Необязательный, значение по умолчанию `false` .</span><span class="sxs-lookup"><span data-stu-id="f78ac-155">Optional, default value is `false`.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="f78ac-156">Свойства определения политики жизни маркера</span><span class="sxs-lookup"><span data-stu-id="f78ac-156">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="f78ac-157">Свойства, представленные ниже, формируют объект JSON, который представляет политику срока службы маркера.</span><span class="sxs-lookup"><span data-stu-id="f78ac-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="f78ac-158">Этот объект JSON необходимо **преобразовать** в строку с кавычками, которые будут вставлены в **свойство определения.**</span><span class="sxs-lookup"><span data-stu-id="f78ac-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="f78ac-159">Пример показан ниже в формате JSON:</span><span class="sxs-lookup"><span data-stu-id="f78ac-159">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="f78ac-160">**Примечание:** Все периоды времени в этих свойствах указаны в формате "dd.hh:mm:ss".</span><span class="sxs-lookup"><span data-stu-id="f78ac-160">**Note:** All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="f78ac-161">**Примечание:** Максимальные значения свойств, обозначаемого в "днях", на 1 секунду меньше замечаемого числа дней.</span><span class="sxs-lookup"><span data-stu-id="f78ac-161">**Note:** Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="f78ac-162">Например, максимальное значение 1 дня указывается как "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="f78ac-162">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="f78ac-163">Свойство</span><span class="sxs-lookup"><span data-stu-id="f78ac-163">Property</span></span>     | <span data-ttu-id="f78ac-164">Тип</span><span class="sxs-lookup"><span data-stu-id="f78ac-164">Type</span></span>   |<span data-ttu-id="f78ac-165">Описание</span><span class="sxs-lookup"><span data-stu-id="f78ac-165">Description</span></span>| <span data-ttu-id="f78ac-166">Значение Min</span><span class="sxs-lookup"><span data-stu-id="f78ac-166">Min Value</span></span> | <span data-ttu-id="f78ac-167">Максимальное значение</span><span class="sxs-lookup"><span data-stu-id="f78ac-167">Max Value</span></span> | <span data-ttu-id="f78ac-168">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="f78ac-168">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="f78ac-169">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="f78ac-169">AccessTokenLifetime</span></span>|<span data-ttu-id="f78ac-170">Строка</span><span class="sxs-lookup"><span data-stu-id="f78ac-170">String</span></span>|<span data-ttu-id="f78ac-171">Контролирует, как долго и доступ, и маркеры ID считаются допустимыми.</span><span class="sxs-lookup"><span data-stu-id="f78ac-171">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="f78ac-172">10 минут</span><span class="sxs-lookup"><span data-stu-id="f78ac-172">10 minutes</span></span>|<span data-ttu-id="f78ac-173">1 день</span><span class="sxs-lookup"><span data-stu-id="f78ac-173">1 day</span></span>|<span data-ttu-id="f78ac-174">1 час</span><span class="sxs-lookup"><span data-stu-id="f78ac-174">1 hour</span></span>|
|<span data-ttu-id="f78ac-175">Версия</span><span class="sxs-lookup"><span data-stu-id="f78ac-175">Version</span></span>|<span data-ttu-id="f78ac-176">Целое число</span><span class="sxs-lookup"><span data-stu-id="f78ac-176">Integer</span></span>|<span data-ttu-id="f78ac-177">Значение 1.</span><span class="sxs-lookup"><span data-stu-id="f78ac-177">Set value of 1.</span></span> <span data-ttu-id="f78ac-178">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f78ac-178">Required.</span></span>|<span data-ttu-id="f78ac-179">Нет</span><span class="sxs-lookup"><span data-stu-id="f78ac-179">None</span></span>|<span data-ttu-id="f78ac-180">Нет</span><span class="sxs-lookup"><span data-stu-id="f78ac-180">None</span></span>|<span data-ttu-id="f78ac-181">Нет</span><span class="sxs-lookup"><span data-stu-id="f78ac-181">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="f78ac-182">Связи</span><span class="sxs-lookup"><span data-stu-id="f78ac-182">Relationships</span></span>

| <span data-ttu-id="f78ac-183">Связь</span><span class="sxs-lookup"><span data-stu-id="f78ac-183">Relationship</span></span> | <span data-ttu-id="f78ac-184">Тип</span><span class="sxs-lookup"><span data-stu-id="f78ac-184">Type</span></span>        | <span data-ttu-id="f78ac-185">Описание</span><span class="sxs-lookup"><span data-stu-id="f78ac-185">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f78ac-186">appliesTo</span><span class="sxs-lookup"><span data-stu-id="f78ac-186">appliesTo</span></span>|<span data-ttu-id="f78ac-187">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="f78ac-187">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="f78ac-188">Коллекция [directoryObject,](directoryObject.md) к которую была применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="f78ac-188">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="f78ac-189">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f78ac-189">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f78ac-190">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f78ac-190">JSON representation</span></span>

<span data-ttu-id="f78ac-191">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f78ac-191">The following is a JSON representation of the resource.</span></span>

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
