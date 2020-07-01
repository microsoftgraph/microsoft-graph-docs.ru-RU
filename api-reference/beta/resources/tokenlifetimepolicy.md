---
title: Тип ресурса Токенлифетимеполици
description: Представляет политику, которая может управлять временем существования маркера доступа, выданного Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 143898e33e3e3474bd5caf0d7855ff19a15e4e13
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006970"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="a5cb1-103">Тип ресурса Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="a5cb1-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="a5cb1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5cb1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5cb1-105">Представляет политику, которая может управлять жизненным циклом маркера доступа JWT, маркером ID или маркером SAML 1.1/2.0, выданным Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a5cb1-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="a5cb1-106">Вы можете задать время жизни маркеров для всех приложений в Организации, для приложения с несколькими клиентами (многоорганизации) или для определенного субъекта-службы в Организации.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="a5cb1-107">Дополнительные сведения о сценариях см [в разделе Настраиваемые сроки жизни маркеров в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="a5cb1-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="a5cb1-108">Note: Настройка этой политики для маркеров обновления и маркеров сеансов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-108">Note: Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="a5cb1-109">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a5cb1-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a5cb1-110">Методы</span><span class="sxs-lookup"><span data-stu-id="a5cb1-110">Methods</span></span>

| <span data-ttu-id="a5cb1-111">Метод</span><span class="sxs-lookup"><span data-stu-id="a5cb1-111">Method</span></span>       | <span data-ttu-id="a5cb1-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a5cb1-112">Return Type</span></span> | <span data-ttu-id="a5cb1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a5cb1-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a5cb1-114">Создание Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="a5cb1-114">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="a5cb1-115">токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="a5cb1-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="a5cb1-116">Создание объекта Токенлифетимеполици.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-116">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="a5cb1-117">Получение Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="a5cb1-117">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="a5cb1-118">токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="a5cb1-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="a5cb1-119">Чтение свойств и связей объекта Токенлифетимеполици.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-119">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="a5cb1-120">Перечисление типов ресурсов tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="a5cb1-120">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="a5cb1-121">токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="a5cb1-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="a5cb1-122">Чтение свойств и связей объектов ТокенлифетимеполиЦиес.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-122">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="a5cb1-123">Обновление Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="a5cb1-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="a5cb1-124">Нет</span><span class="sxs-lookup"><span data-stu-id="a5cb1-124">None</span></span> | <span data-ttu-id="a5cb1-125">Обновление объекта Токенлифетимеполици.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="a5cb1-126">Удаление Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="a5cb1-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="a5cb1-127">Нет</span><span class="sxs-lookup"><span data-stu-id="a5cb1-127">None</span></span> | <span data-ttu-id="a5cb1-128">Удаление объекта Токенлифетимеполици.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="a5cb1-129">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="a5cb1-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="a5cb1-130">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a5cb1-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="a5cb1-131">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="a5cb1-132">Назначение типа ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="a5cb1-132">Assign tokenLifetimePolicy</span></span>](../api/application-post-tokenlifetimepolicies.md) | <span data-ttu-id="a5cb1-133">Нет</span><span class="sxs-lookup"><span data-stu-id="a5cb1-133">None</span></span> | <span data-ttu-id="a5cb1-134">Назначьте объект Токенлифетимеполици объекту [Application](application.md) или [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="a5cb1-134">Assign a tokenLifetimePolicy object to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="a5cb1-135">Список назначенных Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="a5cb1-135">List assigned tokenLifetimePolicy</span></span>](../api/application-list-tokenlifetimepolicies.md) | <span data-ttu-id="a5cb1-136">Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a5cb1-136">[tokenLifetimePolicy](tokenlifetimepolicy.md) collection</span></span> | <span data-ttu-id="a5cb1-137">Перечисление объектов Токенлифетимеполици, назначенных [приложению](application.md) или объекту [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="a5cb1-137">List the tokenLifetimePolicy objects that are assigned to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="a5cb1-138">Удаление типа ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="a5cb1-138">Remove tokenLifetimePolicy</span></span>](../api/application-delete-tokenlifetimepolicies.md) | <span data-ttu-id="a5cb1-139">Нет</span><span class="sxs-lookup"><span data-stu-id="a5cb1-139">None</span></span> | <span data-ttu-id="a5cb1-140">Удаление объекта Токенлифетимеполици из [приложения](application.md) или объекта [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="a5cb1-140">Remove a tokenLifetimePolicy object from an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a5cb1-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5cb1-141">Properties</span></span>

| <span data-ttu-id="a5cb1-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5cb1-142">Property</span></span>     | <span data-ttu-id="a5cb1-143">Тип</span><span class="sxs-lookup"><span data-stu-id="a5cb1-143">Type</span></span>        | <span data-ttu-id="a5cb1-144">Описание</span><span class="sxs-lookup"><span data-stu-id="a5cb1-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5cb1-145">id</span><span class="sxs-lookup"><span data-stu-id="a5cb1-145">id</span></span>|<span data-ttu-id="a5cb1-146">String</span><span class="sxs-lookup"><span data-stu-id="a5cb1-146">String</span></span>| <span data-ttu-id="a5cb1-147">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-147">Unique identifier for this policy.</span></span> <span data-ttu-id="a5cb1-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-148">Read-only.</span></span>|
|<span data-ttu-id="a5cb1-149">RDLC</span><span class="sxs-lookup"><span data-stu-id="a5cb1-149">definition</span></span>|<span data-ttu-id="a5cb1-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a5cb1-150">String collection</span></span>| <span data-ttu-id="a5cb1-151">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-151">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="a5cb1-152">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-152">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="a5cb1-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-153">Required.</span></span>|
|<span data-ttu-id="a5cb1-154">description</span><span class="sxs-lookup"><span data-stu-id="a5cb1-154">description</span></span>|<span data-ttu-id="a5cb1-155">String</span><span class="sxs-lookup"><span data-stu-id="a5cb1-155">String</span></span>| <span data-ttu-id="a5cb1-156">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-156">Description for this policy.</span></span>|
|<span data-ttu-id="a5cb1-157">displayName</span><span class="sxs-lookup"><span data-stu-id="a5cb1-157">displayName</span></span>|<span data-ttu-id="a5cb1-158">Строка</span><span class="sxs-lookup"><span data-stu-id="a5cb1-158">String</span></span>| <span data-ttu-id="a5cb1-159">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-159">Display name for this policy.</span></span> <span data-ttu-id="a5cb1-160">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-160">Required.</span></span>|
|<span data-ttu-id="a5cb1-161">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="a5cb1-161">isOrganizationDefault</span></span>|<span data-ttu-id="a5cb1-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5cb1-162">Boolean</span></span>|<span data-ttu-id="a5cb1-163">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-163">If set to true, activates this policy.</span></span> <span data-ttu-id="a5cb1-164">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-164">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="a5cb1-165">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-165">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="a5cb1-166">Свойства определения политики времени существования маркера</span><span class="sxs-lookup"><span data-stu-id="a5cb1-166">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="a5cb1-167">Свойства, приведенные ниже, формируют объект JSON, представляющий политику времени существования маркеров.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-167">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="a5cb1-168">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="a5cb1-168">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="a5cb1-169">Ниже показан пример в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-169">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="a5cb1-170">Note: все временные интервалы в этих свойствах указаны в формате "DD. чч: мм: СС".</span><span class="sxs-lookup"><span data-stu-id="a5cb1-170">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="a5cb1-171">Note: Max Values для свойств, обозначенных в "Days", — 1 секунды, обозначенное как количество дней.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-171">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="a5cb1-172">Например, максимальное значение в 1 день задается как "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="a5cb1-172">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="a5cb1-173">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5cb1-173">Property</span></span>     | <span data-ttu-id="a5cb1-174">Тип</span><span class="sxs-lookup"><span data-stu-id="a5cb1-174">Type</span></span>   |<span data-ttu-id="a5cb1-175">Описание</span><span class="sxs-lookup"><span data-stu-id="a5cb1-175">Description</span></span>| <span data-ttu-id="a5cb1-176">Минимальное значение</span><span class="sxs-lookup"><span data-stu-id="a5cb1-176">Min Value</span></span> | <span data-ttu-id="a5cb1-177">Максимальное значение</span><span class="sxs-lookup"><span data-stu-id="a5cb1-177">Max Value</span></span> | <span data-ttu-id="a5cb1-178">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="a5cb1-178">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="a5cb1-179">акцесстокенлифетиме</span><span class="sxs-lookup"><span data-stu-id="a5cb1-179">AccessTokenLifetime</span></span>|<span data-ttu-id="a5cb1-180">String</span><span class="sxs-lookup"><span data-stu-id="a5cb1-180">String</span></span>|<span data-ttu-id="a5cb1-181">Управляет тем, как долго считаются действительными маркеры доступа и ИДЕНТИФИКАТОРы.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-181">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="a5cb1-182">10 минут</span><span class="sxs-lookup"><span data-stu-id="a5cb1-182">10 minutes</span></span>|<span data-ttu-id="a5cb1-183">1 день</span><span class="sxs-lookup"><span data-stu-id="a5cb1-183">1 day</span></span>|<span data-ttu-id="a5cb1-184">1 час</span><span class="sxs-lookup"><span data-stu-id="a5cb1-184">1 hour</span></span>|
|<span data-ttu-id="a5cb1-185">Версия</span><span class="sxs-lookup"><span data-stu-id="a5cb1-185">Version</span></span>|<span data-ttu-id="a5cb1-186">Integer</span><span class="sxs-lookup"><span data-stu-id="a5cb1-186">Integer</span></span>|<span data-ttu-id="a5cb1-187">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-187">Set value of 1.</span></span> <span data-ttu-id="a5cb1-188">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-188">Required.</span></span>|<span data-ttu-id="a5cb1-189">Нет</span><span class="sxs-lookup"><span data-stu-id="a5cb1-189">None</span></span>|<span data-ttu-id="a5cb1-190">Нет</span><span class="sxs-lookup"><span data-stu-id="a5cb1-190">None</span></span>|<span data-ttu-id="a5cb1-191">Нет</span><span class="sxs-lookup"><span data-stu-id="a5cb1-191">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5cb1-192">Связи</span><span class="sxs-lookup"><span data-stu-id="a5cb1-192">Relationships</span></span>

| <span data-ttu-id="a5cb1-193">Связь</span><span class="sxs-lookup"><span data-stu-id="a5cb1-193">Relationship</span></span> | <span data-ttu-id="a5cb1-194">Тип</span><span class="sxs-lookup"><span data-stu-id="a5cb1-194">Type</span></span>        | <span data-ttu-id="a5cb1-195">Описание</span><span class="sxs-lookup"><span data-stu-id="a5cb1-195">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5cb1-196">Тег</span><span class="sxs-lookup"><span data-stu-id="a5cb1-196">appliesTo</span></span>|<span data-ttu-id="a5cb1-197">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a5cb1-197">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="a5cb1-198">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-198">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="a5cb1-199">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-199">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5cb1-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5cb1-200">JSON representation</span></span>

<span data-ttu-id="a5cb1-201">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5cb1-201">The following is a JSON representation of the resource.</span></span>

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