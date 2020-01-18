---
title: Тип ресурса Токенлифетимеполици
description: Представляет политику, которая может управлять временем существования маркера доступа, выданного Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a19ec9e2b8747737895bed89b1a92ec4c5d134a
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234506"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="d1f76-103">Тип ресурса Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="d1f76-103">tokenLifetimePolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1f76-104">Представляет политику, которая может управлять жизненным циклом маркера доступа JWT, маркером ID или маркером SAML 1.1/2.0, выданным Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d1f76-104">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="d1f76-105">Вы можете задать время жизни маркеров для всех приложений в Организации, для приложения с несколькими клиентами (многоорганизации) или для определенного субъекта-службы в Организации.</span><span class="sxs-lookup"><span data-stu-id="d1f76-105">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="d1f76-106">Дополнительные сведения о сценариях см [в разделе Настраиваемые сроки жизни маркеров в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="d1f76-106">For more scenario details see [Configurable token lifetimes in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="d1f76-107">Note: Настройка этой политики для маркеров обновления и маркеров сеансов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1f76-107">Note: Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="d1f76-108">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d1f76-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d1f76-109">Методы</span><span class="sxs-lookup"><span data-stu-id="d1f76-109">Methods</span></span>

| <span data-ttu-id="d1f76-110">Метод</span><span class="sxs-lookup"><span data-stu-id="d1f76-110">Method</span></span>       | <span data-ttu-id="d1f76-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d1f76-111">Return Type</span></span> | <span data-ttu-id="d1f76-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d1f76-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d1f76-113">Создание Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="d1f76-113">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="d1f76-114">токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="d1f76-114">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="d1f76-115">Создание объекта Токенлифетимеполици.</span><span class="sxs-lookup"><span data-stu-id="d1f76-115">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="d1f76-116">Получение Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="d1f76-116">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="d1f76-117">токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="d1f76-117">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="d1f76-118">Чтение свойств и связей объекта Токенлифетимеполици.</span><span class="sxs-lookup"><span data-stu-id="d1f76-118">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="d1f76-119">Список ТокенлифетимеполиЦиес</span><span class="sxs-lookup"><span data-stu-id="d1f76-119">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="d1f76-120">токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="d1f76-120">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="d1f76-121">Чтение свойств и связей объектов ТокенлифетимеполиЦиес.</span><span class="sxs-lookup"><span data-stu-id="d1f76-121">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="d1f76-122">Обновление Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="d1f76-122">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="d1f76-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d1f76-123">None</span></span> | <span data-ttu-id="d1f76-124">Обновление объекта Токенлифетимеполици.</span><span class="sxs-lookup"><span data-stu-id="d1f76-124">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="d1f76-125">Удаление Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="d1f76-125">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="d1f76-126">Нет</span><span class="sxs-lookup"><span data-stu-id="d1f76-126">None</span></span> | <span data-ttu-id="d1f76-127">Удаление объекта Токенлифетимеполици.</span><span class="sxs-lookup"><span data-stu-id="d1f76-127">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="d1f76-128">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="d1f76-128">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="d1f76-129">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="d1f76-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="d1f76-130">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="d1f76-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="d1f76-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1f76-131">Properties</span></span>

| <span data-ttu-id="d1f76-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1f76-132">Property</span></span>     | <span data-ttu-id="d1f76-133">Тип</span><span class="sxs-lookup"><span data-stu-id="d1f76-133">Type</span></span>        | <span data-ttu-id="d1f76-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d1f76-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d1f76-135">id</span><span class="sxs-lookup"><span data-stu-id="d1f76-135">id</span></span>|<span data-ttu-id="d1f76-136">String</span><span class="sxs-lookup"><span data-stu-id="d1f76-136">String</span></span>| <span data-ttu-id="d1f76-137">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d1f76-137">Unique identifier for this policy.</span></span> <span data-ttu-id="d1f76-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1f76-138">Read-only.</span></span>|
|<span data-ttu-id="d1f76-139">RDLC</span><span class="sxs-lookup"><span data-stu-id="d1f76-139">definition</span></span>|<span data-ttu-id="d1f76-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d1f76-140">String collection</span></span>| <span data-ttu-id="d1f76-141">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d1f76-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="d1f76-142">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="d1f76-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="d1f76-143">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="d1f76-143">Required.</span></span>|
|<span data-ttu-id="d1f76-144">description</span><span class="sxs-lookup"><span data-stu-id="d1f76-144">description</span></span>|<span data-ttu-id="d1f76-145">String</span><span class="sxs-lookup"><span data-stu-id="d1f76-145">String</span></span>| <span data-ttu-id="d1f76-146">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d1f76-146">Description for this policy.</span></span>|
|<span data-ttu-id="d1f76-147">displayName</span><span class="sxs-lookup"><span data-stu-id="d1f76-147">displayName</span></span>|<span data-ttu-id="d1f76-148">Строка</span><span class="sxs-lookup"><span data-stu-id="d1f76-148">String</span></span>| <span data-ttu-id="d1f76-149">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d1f76-149">Display name for this policy.</span></span> <span data-ttu-id="d1f76-150">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d1f76-150">Required.</span></span>|
|<span data-ttu-id="d1f76-151">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="d1f76-151">isOrganizationDefault</span></span>|<span data-ttu-id="d1f76-152">Логический</span><span class="sxs-lookup"><span data-stu-id="d1f76-152">Boolean</span></span>|<span data-ttu-id="d1f76-153">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="d1f76-153">If set to true, activates this policy.</span></span> <span data-ttu-id="d1f76-154">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d1f76-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="d1f76-155">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="d1f76-155">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="d1f76-156">Свойства определения политики времени существования маркера</span><span class="sxs-lookup"><span data-stu-id="d1f76-156">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="d1f76-157">Свойства, приведенные ниже, формируют объект JSON, представляющий политику времени существования маркеров.</span><span class="sxs-lookup"><span data-stu-id="d1f76-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="d1f76-158">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="d1f76-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="d1f76-159">Ниже показан пример в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1f76-159">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="d1f76-160">Note: все временные интервалы в этих свойствах указаны в формате "DD. чч: мм: СС".</span><span class="sxs-lookup"><span data-stu-id="d1f76-160">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="d1f76-161">Note: Max Values для свойств, обозначенных в "Days", — 1 секунды, обозначенное как количество дней.</span><span class="sxs-lookup"><span data-stu-id="d1f76-161">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="d1f76-162">Например, максимальное значение в 1 день задается как "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="d1f76-162">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="d1f76-163">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1f76-163">Property</span></span>     | <span data-ttu-id="d1f76-164">Тип</span><span class="sxs-lookup"><span data-stu-id="d1f76-164">Type</span></span>   |<span data-ttu-id="d1f76-165">Описание</span><span class="sxs-lookup"><span data-stu-id="d1f76-165">Description</span></span>| <span data-ttu-id="d1f76-166">Минимальное значение</span><span class="sxs-lookup"><span data-stu-id="d1f76-166">Min Value</span></span> | <span data-ttu-id="d1f76-167">Максимальное значение</span><span class="sxs-lookup"><span data-stu-id="d1f76-167">Max Value</span></span> | <span data-ttu-id="d1f76-168">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="d1f76-168">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="d1f76-169">акцесстокенлифетиме</span><span class="sxs-lookup"><span data-stu-id="d1f76-169">AccessTokenLifetime</span></span>|<span data-ttu-id="d1f76-170">String</span><span class="sxs-lookup"><span data-stu-id="d1f76-170">String</span></span>|<span data-ttu-id="d1f76-171">Управляет тем, как долго считаются действительными маркеры доступа и ИДЕНТИФИКАТОРы.</span><span class="sxs-lookup"><span data-stu-id="d1f76-171">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="d1f76-172">10 минут</span><span class="sxs-lookup"><span data-stu-id="d1f76-172">10 minutes</span></span>|<span data-ttu-id="d1f76-173">1 день</span><span class="sxs-lookup"><span data-stu-id="d1f76-173">1 day</span></span>|<span data-ttu-id="d1f76-174">1 hour</span><span class="sxs-lookup"><span data-stu-id="d1f76-174">1 hour</span></span>|
|<span data-ttu-id="d1f76-175">Версия</span><span class="sxs-lookup"><span data-stu-id="d1f76-175">Version</span></span>|<span data-ttu-id="d1f76-176">Целое число</span><span class="sxs-lookup"><span data-stu-id="d1f76-176">Integer</span></span>|<span data-ttu-id="d1f76-177">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="d1f76-177">Set value of 1.</span></span> <span data-ttu-id="d1f76-178">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d1f76-178">Required.</span></span>|<span data-ttu-id="d1f76-179">Нет</span><span class="sxs-lookup"><span data-stu-id="d1f76-179">None</span></span>|<span data-ttu-id="d1f76-180">Нет</span><span class="sxs-lookup"><span data-stu-id="d1f76-180">None</span></span>|<span data-ttu-id="d1f76-181">Нет</span><span class="sxs-lookup"><span data-stu-id="d1f76-181">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1f76-182">Связи</span><span class="sxs-lookup"><span data-stu-id="d1f76-182">Relationships</span></span>

| <span data-ttu-id="d1f76-183">Связь</span><span class="sxs-lookup"><span data-stu-id="d1f76-183">Relationship</span></span> | <span data-ttu-id="d1f76-184">Тип</span><span class="sxs-lookup"><span data-stu-id="d1f76-184">Type</span></span>        | <span data-ttu-id="d1f76-185">Описание</span><span class="sxs-lookup"><span data-stu-id="d1f76-185">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d1f76-186">Тег</span><span class="sxs-lookup"><span data-stu-id="d1f76-186">appliesTo</span></span>|<span data-ttu-id="d1f76-187">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="d1f76-187">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="d1f76-188">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="d1f76-188">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="d1f76-189">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1f76-189">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1f76-190">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1f76-190">JSON representation</span></span>

<span data-ttu-id="d1f76-191">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1f76-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
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
  "description": "tokenLifetimePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->