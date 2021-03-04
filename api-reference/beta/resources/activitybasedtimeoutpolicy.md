---
title: тип ресурса activityBasedTimeoutPolicy
description: Представляет политику, которая может контролировать время ожидания простоя для веб-сеансов для приложений, которые поддерживают функции времени ожидания на основе действий.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ec4cf6705a845e6920e614ba35c7a4190456e93f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433245"
---
# <a name="activitybasedtimeoutpolicy-resource-type"></a><span data-ttu-id="ecdce-103">тип ресурса activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="ecdce-103">activityBasedTimeoutPolicy resource type</span></span>

<span data-ttu-id="ecdce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecdce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecdce-105">Представляет политику, которая может контролировать время ожидания простоя для веб-сеансов для приложений, которые поддерживают функции времени ожидания на основе действий.</span><span class="sxs-lookup"><span data-stu-id="ecdce-105">Represents a policy that can control the idle timeout for web sessions for applications that support activity-based timeout functionality.</span></span> <span data-ttu-id="ecdce-106">Приложения применяют автоматическую вывеску после периода бездействия.</span><span class="sxs-lookup"><span data-stu-id="ecdce-106">Applications enforce automatic signout after a period of inactivity.</span></span> <span data-ttu-id="ecdce-107">Этот тип политики можно применять только на уровне организации (задав свойство **isOrganizationDefault).** `true`</span><span class="sxs-lookup"><span data-stu-id="ecdce-107">This type of policy can only be applied at the organization level (by setting the **isOrganizationDefault** property to `true`).</span></span>

<span data-ttu-id="ecdce-108">Наследует [от stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ecdce-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ecdce-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ecdce-109">Methods</span></span>

| <span data-ttu-id="ecdce-110">Метод</span><span class="sxs-lookup"><span data-stu-id="ecdce-110">Method</span></span>       | <span data-ttu-id="ecdce-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ecdce-111">Return Type</span></span> | <span data-ttu-id="ecdce-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ecdce-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ecdce-113">Создание activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="ecdce-113">Create activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-post-activitybasedtimeoutpolicies.md) | [<span data-ttu-id="ecdce-114">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="ecdce-114">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="ecdce-115">Создание объекта activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="ecdce-115">Create an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="ecdce-116">Get activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="ecdce-116">Get activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-get.md) | [<span data-ttu-id="ecdce-117">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="ecdce-117">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="ecdce-118">Чтение свойств и связей объекта activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="ecdce-118">Read properties and relationships of an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="ecdce-119">Список действийBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="ecdce-119">List activityBasedTimeoutPolicies</span></span>](../api/activitybasedtimeoutpolicy-list.md) | [<span data-ttu-id="ecdce-120">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="ecdce-120">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="ecdce-121">Чтение свойств и связей объектов activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="ecdce-121">Read properties and relationships of activityBasedTimeoutPolicy objects.</span></span> |
| [<span data-ttu-id="ecdce-122">Обновление activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="ecdce-122">Update activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-update.md) | <span data-ttu-id="ecdce-123">Нет</span><span class="sxs-lookup"><span data-stu-id="ecdce-123">None</span></span> | <span data-ttu-id="ecdce-124">Обновление объекта activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="ecdce-124">Update an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="ecdce-125">Удаление activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="ecdce-125">Delete activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-delete.md) | <span data-ttu-id="ecdce-126">Нет</span><span class="sxs-lookup"><span data-stu-id="ecdce-126">None</span></span> | <span data-ttu-id="ecdce-127">Удаление объекта activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="ecdce-127">Delete an activityBasedTimeoutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ecdce-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="ecdce-128">Properties</span></span>

| <span data-ttu-id="ecdce-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ecdce-129">Property</span></span>     | <span data-ttu-id="ecdce-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ecdce-130">Type</span></span>        | <span data-ttu-id="ecdce-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ecdce-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ecdce-132">id</span><span class="sxs-lookup"><span data-stu-id="ecdce-132">id</span></span>|<span data-ttu-id="ecdce-133">String</span><span class="sxs-lookup"><span data-stu-id="ecdce-133">String</span></span>| <span data-ttu-id="ecdce-134">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ecdce-134">Unique identifier for this policy.</span></span> <span data-ttu-id="ecdce-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ecdce-135">Read-only.</span></span>|
|<span data-ttu-id="ecdce-136">определение</span><span class="sxs-lookup"><span data-stu-id="ecdce-136">definition</span></span>|<span data-ttu-id="ecdce-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ecdce-137">String collection</span></span>| <span data-ttu-id="ecdce-138">Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики.</span><span class="sxs-lookup"><span data-stu-id="ecdce-138">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="ecdce-139">Дополнительные сведения о схеме JSON для этого свойства см. ниже.</span><span class="sxs-lookup"><span data-stu-id="ecdce-139">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="ecdce-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecdce-140">Required.</span></span>|
|<span data-ttu-id="ecdce-141">description</span><span class="sxs-lookup"><span data-stu-id="ecdce-141">description</span></span>|<span data-ttu-id="ecdce-142">String</span><span class="sxs-lookup"><span data-stu-id="ecdce-142">String</span></span>| <span data-ttu-id="ecdce-143">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="ecdce-143">Description for this policy.</span></span>|
|<span data-ttu-id="ecdce-144">displayName</span><span class="sxs-lookup"><span data-stu-id="ecdce-144">displayName</span></span>|<span data-ttu-id="ecdce-145">String</span><span class="sxs-lookup"><span data-stu-id="ecdce-145">String</span></span>| <span data-ttu-id="ecdce-146">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ecdce-146">Display name for this policy.</span></span> <span data-ttu-id="ecdce-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecdce-147">Required.</span></span>|
|<span data-ttu-id="ecdce-148">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="ecdce-148">isOrganizationDefault</span></span>|<span data-ttu-id="ecdce-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="ecdce-149">Boolean</span></span>|<span data-ttu-id="ecdce-150">Если заданной для true, активирует эту политику.</span><span class="sxs-lookup"><span data-stu-id="ecdce-150">If set to true, activates this policy.</span></span> <span data-ttu-id="ecdce-151">Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации.</span><span class="sxs-lookup"><span data-stu-id="ecdce-151">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="ecdce-152">Необязательный, значение по умолчанию является ложным.</span><span class="sxs-lookup"><span data-stu-id="ecdce-152">Optional, default value is false.</span></span>|


### <a name="properties-of-an-activity-based-timeout-policy-definition"></a><span data-ttu-id="ecdce-153">Свойства определения политики политики времени на основе действий</span><span class="sxs-lookup"><span data-stu-id="ecdce-153">Properties of an activity-based timeout policy definition</span></span>
<span data-ttu-id="ecdce-154">Свойства ниже формируют объект JSON, который представляет политику времени, основанную на действиях.</span><span class="sxs-lookup"><span data-stu-id="ecdce-154">The properties below form the JSON object that represents an activity-based timeout policy.</span></span> <span data-ttu-id="ecdce-155">Этот объект JSON необходимо **преобразовать** в строку с кавычками, которые будут вставлены в **свойство определения.**</span><span class="sxs-lookup"><span data-stu-id="ecdce-155">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="ecdce-156">Пример показан ниже в формате JSON:</span><span class="sxs-lookup"><span data-stu-id="ecdce-156">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```json
{
  "definition":["{\"ActivityBasedTimeoutPolicy\":{\"Version\":1,\"ApplicationPolicies\":[{\"ApplicationId\":\"default\",\"WebSessionIdleTimeout\":\"01:00:00\"},{\"ApplicationId\":\"c44b4083-3bb0-49c1-b47d-974e53cbdf3c\",\"WebSessionIdleTimeout\":\"00:15:00\"}]}}"]
}
```

><span data-ttu-id="ecdce-157">Примечание. Все периоды времени в этих свойствах указаны в формате "dd.hh:mm:ss".</span><span class="sxs-lookup"><span data-stu-id="ecdce-157">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="ecdce-158">Примечание. Максимальные значения для свойств, обозначаемого в "днях", на 1 секунду меньше замечаемого числа дней.</span><span class="sxs-lookup"><span data-stu-id="ecdce-158">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="ecdce-159">Например, максимальное значение 1 дня указывается как "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="ecdce-159">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="ecdce-160">Свойство</span><span class="sxs-lookup"><span data-stu-id="ecdce-160">Property</span></span>     | <span data-ttu-id="ecdce-161">Тип</span><span class="sxs-lookup"><span data-stu-id="ecdce-161">Type</span></span>   |<span data-ttu-id="ecdce-162">Описание</span><span class="sxs-lookup"><span data-stu-id="ecdce-162">Description</span></span>|
|:-------------|:------|:---------|
|<span data-ttu-id="ecdce-163">Версия</span><span class="sxs-lookup"><span data-stu-id="ecdce-163">Version</span></span>|<span data-ttu-id="ecdce-164">Целое число</span><span class="sxs-lookup"><span data-stu-id="ecdce-164">Integer</span></span>|<span data-ttu-id="ecdce-165">Версия политики.</span><span class="sxs-lookup"><span data-stu-id="ecdce-165">Policy version.</span></span> <span data-ttu-id="ecdce-166">Значение 1.</span><span class="sxs-lookup"><span data-stu-id="ecdce-166">Set value of 1.</span></span> <span data-ttu-id="ecdce-167">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecdce-167">Required.</span></span>|
|<span data-ttu-id="ecdce-168">ApplicationPolicies</span><span class="sxs-lookup"><span data-stu-id="ecdce-168">ApplicationPolicies</span></span>|<span data-ttu-id="ecdce-169">Объект JSON</span><span class="sxs-lookup"><span data-stu-id="ecdce-169">JSON object</span></span>|<span data-ttu-id="ecdce-170">Коллекция политики приложений.</span><span class="sxs-lookup"><span data-stu-id="ecdce-170">Collection of application policy.</span></span> <span data-ttu-id="ecdce-171">Политика приложения — это сочетание ApplicationId и WebSessionIdleTimeout:</span><span class="sxs-lookup"><span data-stu-id="ecdce-171">An application policy, is a combination of an ApplicationId and a WebSessionIdleTimeout:</span></span> <br> <ul><li><span data-ttu-id="ecdce-172">**ApplicationId:** Допустимые значения:</span><span class="sxs-lookup"><span data-stu-id="ecdce-172">**ApplicationId**: Allowed values:</span></span><ul><li> <span data-ttu-id="ecdce-173">по умолчанию: применяет политику ко всем приложениям, которые поддерживают функции периодиа времени на основе действий, но не имеют переопределения, определенного для приложений</span><span class="sxs-lookup"><span data-stu-id="ecdce-173">default: applies the policy to all applications that support activity-based timeout functionality but do not have application-specific override</span></span></li><li> <span data-ttu-id="ecdce-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c3c: применяет политику к порталу Azure</span><span class="sxs-lookup"><span data-stu-id="ecdce-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: applies the policy to the Azure Portal</span></span></li></ul></li><li><span data-ttu-id="ecdce-175">**WebSessionIdleTimeout:** период бездействия пользователя, после которого веб-сеанс пользователя считается истекшим.</span><span class="sxs-lookup"><span data-stu-id="ecdce-175">**WebSessionIdleTimeout**: The period of user inactivity after which the user's web session is considered expired.</span></span> <span data-ttu-id="ecdce-176">Минимальное значение — 5 минут; максимальное значение — 1 день.</span><span class="sxs-lookup"><span data-stu-id="ecdce-176">The minimum value is 5 minutes; the maximum value is 1 day.</span></span></li></ul> |


## <a name="relationships"></a><span data-ttu-id="ecdce-177">Связи</span><span class="sxs-lookup"><span data-stu-id="ecdce-177">Relationships</span></span>

<span data-ttu-id="ecdce-178">Нет</span><span class="sxs-lookup"><span data-stu-id="ecdce-178">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ecdce-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ecdce-179">JSON representation</span></span>

<span data-ttu-id="ecdce-180">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ecdce-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activityBasedTimeoutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

