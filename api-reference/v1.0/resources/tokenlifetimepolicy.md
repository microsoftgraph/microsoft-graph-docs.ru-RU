---
title: Тип ресурса Токенлифетимеполици
description: Представляет политику, которая может управлять временем существования маркера доступа, выданного Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dddc15d56f580352168dceb6c0b954194c1dbf0d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090692"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="6e112-103">Тип ресурса Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="6e112-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="6e112-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e112-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="6e112-105">Представляет политику, которая может управлять жизненным циклом маркера доступа JWT, маркером ID или маркером SAML 1.1/2.0, выданным Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="6e112-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="6e112-106">Вы можете задать время жизни маркеров для всех приложений в Организации, для приложения с несколькими клиентами (многоорганизации) или для определенного субъекта-службы в Организации.</span><span class="sxs-lookup"><span data-stu-id="6e112-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="6e112-107">Дополнительные сведения о сценариях см [в разделе Настраиваемые сроки жизни маркеров в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="6e112-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="6e112-108">**Примечание:** Настройка этой политики для маркеров обновления и маркеров сеансов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e112-108">**Note:** Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="6e112-109">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e112-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6e112-110">Методы</span><span class="sxs-lookup"><span data-stu-id="6e112-110">Methods</span></span>

| <span data-ttu-id="6e112-111">Метод</span><span class="sxs-lookup"><span data-stu-id="6e112-111">Method</span></span>       | <span data-ttu-id="6e112-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6e112-112">Return Type</span></span> | <span data-ttu-id="6e112-113">Описание</span><span class="sxs-lookup"><span data-stu-id="6e112-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6e112-114">Перечисление типов ресурсов tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="6e112-114">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="6e112-115">токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="6e112-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="6e112-116">Чтение свойств и связей объектов ТокенлифетимеполиЦиес.</span><span class="sxs-lookup"><span data-stu-id="6e112-116">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="6e112-117">Создание Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="6e112-117">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="6e112-118">токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="6e112-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="6e112-119">Создание объекта Токенлифетимеполици.</span><span class="sxs-lookup"><span data-stu-id="6e112-119">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="6e112-120">Получение Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="6e112-120">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="6e112-121">токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="6e112-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="6e112-122">Чтение свойств и связей объекта Токенлифетимеполици.</span><span class="sxs-lookup"><span data-stu-id="6e112-122">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="6e112-123">Обновление Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="6e112-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="6e112-124">Нет</span><span class="sxs-lookup"><span data-stu-id="6e112-124">None</span></span> | <span data-ttu-id="6e112-125">Обновление объекта Токенлифетимеполици.</span><span class="sxs-lookup"><span data-stu-id="6e112-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="6e112-126">Удаление Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="6e112-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="6e112-127">Нет</span><span class="sxs-lookup"><span data-stu-id="6e112-127">None</span></span> | <span data-ttu-id="6e112-128">Удаление объекта Токенлифетимеполици.</span><span class="sxs-lookup"><span data-stu-id="6e112-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="6e112-129">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="6e112-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="6e112-130">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="6e112-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="6e112-131">Получение списка Директорйобжектс, к которым применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="6e112-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="6e112-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e112-132">Properties</span></span>

| <span data-ttu-id="6e112-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e112-133">Property</span></span>     | <span data-ttu-id="6e112-134">Тип</span><span class="sxs-lookup"><span data-stu-id="6e112-134">Type</span></span>        | <span data-ttu-id="6e112-135">Описание</span><span class="sxs-lookup"><span data-stu-id="6e112-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6e112-136">id</span><span class="sxs-lookup"><span data-stu-id="6e112-136">id</span></span>|<span data-ttu-id="6e112-137">Строка</span><span class="sxs-lookup"><span data-stu-id="6e112-137">String</span></span>| <span data-ttu-id="6e112-138">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6e112-138">Unique identifier for this policy.</span></span> <span data-ttu-id="6e112-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e112-139">Read-only.</span></span>|
|<span data-ttu-id="6e112-140">RDLC</span><span class="sxs-lookup"><span data-stu-id="6e112-140">definition</span></span>|<span data-ttu-id="6e112-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e112-141">String collection</span></span>| <span data-ttu-id="6e112-142">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6e112-142">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="6e112-143">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="6e112-143">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="6e112-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e112-144">Required.</span></span>|
|<span data-ttu-id="6e112-145">description</span><span class="sxs-lookup"><span data-stu-id="6e112-145">description</span></span>|<span data-ttu-id="6e112-146">Строка</span><span class="sxs-lookup"><span data-stu-id="6e112-146">String</span></span>| <span data-ttu-id="6e112-147">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6e112-147">Description for this policy.</span></span>|
|<span data-ttu-id="6e112-148">displayName</span><span class="sxs-lookup"><span data-stu-id="6e112-148">displayName</span></span>|<span data-ttu-id="6e112-149">Строка</span><span class="sxs-lookup"><span data-stu-id="6e112-149">String</span></span>| <span data-ttu-id="6e112-150">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6e112-150">Display name for this policy.</span></span> <span data-ttu-id="6e112-151">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e112-151">Required.</span></span>|
|<span data-ttu-id="6e112-152">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="6e112-152">isOrganizationDefault</span></span>|<span data-ttu-id="6e112-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e112-153">Boolean</span></span>|<span data-ttu-id="6e112-154">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="6e112-154">If set to true, activates this policy.</span></span> <span data-ttu-id="6e112-155">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6e112-155">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="6e112-156">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="6e112-156">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="6e112-157">Свойства определения политики времени существования маркера</span><span class="sxs-lookup"><span data-stu-id="6e112-157">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="6e112-158">Свойства, приведенные ниже, формируют объект JSON, представляющий политику времени существования маркеров.</span><span class="sxs-lookup"><span data-stu-id="6e112-158">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="6e112-159">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="6e112-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="6e112-160">Ниже показан пример в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e112-160">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="6e112-161">**Примечание:** Все временные интервалы в этих свойствах указываются в формате "DD. чч: мм: СС".</span><span class="sxs-lookup"><span data-stu-id="6e112-161">**Note:** All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="6e112-162">**Примечание:** Максимальные значения свойств, обозначенных в "Days", задаются в течение 1 секунды с заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="6e112-162">**Note:** Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="6e112-163">Например, максимальное значение в 1 день задается как "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="6e112-163">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="6e112-164">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e112-164">Property</span></span>     | <span data-ttu-id="6e112-165">Тип</span><span class="sxs-lookup"><span data-stu-id="6e112-165">Type</span></span>   |<span data-ttu-id="6e112-166">Описание</span><span class="sxs-lookup"><span data-stu-id="6e112-166">Description</span></span>| <span data-ttu-id="6e112-167">Минимальное значение</span><span class="sxs-lookup"><span data-stu-id="6e112-167">Min Value</span></span> | <span data-ttu-id="6e112-168">Максимальное значение</span><span class="sxs-lookup"><span data-stu-id="6e112-168">Max Value</span></span> | <span data-ttu-id="6e112-169">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="6e112-169">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="6e112-170">акцесстокенлифетиме</span><span class="sxs-lookup"><span data-stu-id="6e112-170">AccessTokenLifetime</span></span>|<span data-ttu-id="6e112-171">Строка</span><span class="sxs-lookup"><span data-stu-id="6e112-171">String</span></span>|<span data-ttu-id="6e112-172">Управляет тем, как долго считаются действительными маркеры доступа и ИДЕНТИФИКАТОРы.</span><span class="sxs-lookup"><span data-stu-id="6e112-172">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="6e112-173">10 минут</span><span class="sxs-lookup"><span data-stu-id="6e112-173">10 minutes</span></span>|<span data-ttu-id="6e112-174">1 день</span><span class="sxs-lookup"><span data-stu-id="6e112-174">1 day</span></span>|<span data-ttu-id="6e112-175">1 час</span><span class="sxs-lookup"><span data-stu-id="6e112-175">1 hour</span></span>|
|<span data-ttu-id="6e112-176">Версия</span><span class="sxs-lookup"><span data-stu-id="6e112-176">Version</span></span>|<span data-ttu-id="6e112-177">Целое число</span><span class="sxs-lookup"><span data-stu-id="6e112-177">Integer</span></span>|<span data-ttu-id="6e112-178">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="6e112-178">Set value of 1.</span></span> <span data-ttu-id="6e112-179">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e112-179">Required.</span></span>|<span data-ttu-id="6e112-180">Нет</span><span class="sxs-lookup"><span data-stu-id="6e112-180">None</span></span>|<span data-ttu-id="6e112-181">Нет</span><span class="sxs-lookup"><span data-stu-id="6e112-181">None</span></span>|<span data-ttu-id="6e112-182">Нет</span><span class="sxs-lookup"><span data-stu-id="6e112-182">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e112-183">Связи</span><span class="sxs-lookup"><span data-stu-id="6e112-183">Relationships</span></span>

| <span data-ttu-id="6e112-184">Связь</span><span class="sxs-lookup"><span data-stu-id="6e112-184">Relationship</span></span> | <span data-ttu-id="6e112-185">Тип</span><span class="sxs-lookup"><span data-stu-id="6e112-185">Type</span></span>        | <span data-ttu-id="6e112-186">Описание</span><span class="sxs-lookup"><span data-stu-id="6e112-186">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6e112-187">Тег</span><span class="sxs-lookup"><span data-stu-id="6e112-187">appliesTo</span></span>|<span data-ttu-id="6e112-188">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="6e112-188">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="6e112-189">Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика.</span><span class="sxs-lookup"><span data-stu-id="6e112-189">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="6e112-190">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e112-190">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e112-191">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e112-191">JSON representation</span></span>

<span data-ttu-id="6e112-192">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e112-192">The following is a JSON representation of the resource.</span></span>

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

