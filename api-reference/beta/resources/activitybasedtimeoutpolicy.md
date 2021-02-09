---
title: Тип ресурса activityBasedTimeoutPolicy
description: Представляет политику, которая может управлять временем ожидания простоя веб-сеансов для приложений, которые поддерживают функции времени ожидания на основе действий.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 62f18c7083f96abd7d1cf1d2840aa4e29ce66554
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155599"
---
# <a name="activitybasedtimeoutpolicy-resource-type"></a><span data-ttu-id="929df-103">Тип ресурса activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="929df-103">activityBasedTimeoutPolicy resource type</span></span>

<span data-ttu-id="929df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="929df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="929df-105">Представляет политику, которая может управлять временем ожидания простоя веб-сеансов для приложений, которые поддерживают функции времени ожидания на основе действий.</span><span class="sxs-lookup"><span data-stu-id="929df-105">Represents a policy that can control the idle timeout for web sessions for applications that support activity-based timeout functionality.</span></span> <span data-ttu-id="929df-106">Приложения принудительно принудительно выключат автоматический вход после периода бездействия.</span><span class="sxs-lookup"><span data-stu-id="929df-106">Applications enforce automatic signout after a period of inactivity.</span></span> <span data-ttu-id="929df-107">Этот тип политики может применяться только на уровне организации (путем установки свойства **isOrganizationDefault** `true` в ).</span><span class="sxs-lookup"><span data-stu-id="929df-107">This type of policy can only be applied at the organization level (by setting the **isOrganizationDefault** property to `true`).</span></span>

<span data-ttu-id="929df-108">Наследуется от [stsPolicy.](stsPolicy.md)</span><span class="sxs-lookup"><span data-stu-id="929df-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="929df-109">Методы</span><span class="sxs-lookup"><span data-stu-id="929df-109">Methods</span></span>

| <span data-ttu-id="929df-110">Метод</span><span class="sxs-lookup"><span data-stu-id="929df-110">Method</span></span>       | <span data-ttu-id="929df-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="929df-111">Return Type</span></span> | <span data-ttu-id="929df-112">Описание</span><span class="sxs-lookup"><span data-stu-id="929df-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="929df-113">Создание activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="929df-113">Create activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-post-activitybasedtimeoutpolicies.md) | [<span data-ttu-id="929df-114">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="929df-114">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="929df-115">Создание объекта activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="929df-115">Create an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="929df-116">Get activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="929df-116">Get activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-get.md) | [<span data-ttu-id="929df-117">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="929df-117">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="929df-118">Чтение свойств и связей объекта activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="929df-118">Read properties and relationships of an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="929df-119">Список activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="929df-119">List activityBasedTimeoutPolicies</span></span>](../api/activitybasedtimeoutpolicy-list.md) | [<span data-ttu-id="929df-120">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="929df-120">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="929df-121">Чтение свойств и связей объектов activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="929df-121">Read properties and relationships of activityBasedTimeoutPolicy objects.</span></span> |
| [<span data-ttu-id="929df-122">Обновление activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="929df-122">Update activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-update.md) | <span data-ttu-id="929df-123">Нет</span><span class="sxs-lookup"><span data-stu-id="929df-123">None</span></span> | <span data-ttu-id="929df-124">Обновление объекта activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="929df-124">Update an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="929df-125">Удаление activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="929df-125">Delete activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-delete.md) | <span data-ttu-id="929df-126">Нет</span><span class="sxs-lookup"><span data-stu-id="929df-126">None</span></span> | <span data-ttu-id="929df-127">Удаление объекта activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="929df-127">Delete an activityBasedTimeoutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="929df-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="929df-128">Properties</span></span>

| <span data-ttu-id="929df-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="929df-129">Property</span></span>     | <span data-ttu-id="929df-130">Тип</span><span class="sxs-lookup"><span data-stu-id="929df-130">Type</span></span>        | <span data-ttu-id="929df-131">Описание</span><span class="sxs-lookup"><span data-stu-id="929df-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="929df-132">id</span><span class="sxs-lookup"><span data-stu-id="929df-132">id</span></span>|<span data-ttu-id="929df-133">String</span><span class="sxs-lookup"><span data-stu-id="929df-133">String</span></span>| <span data-ttu-id="929df-134">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="929df-134">Unique identifier for this policy.</span></span> <span data-ttu-id="929df-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="929df-135">Read-only.</span></span>|
|<span data-ttu-id="929df-136">definition</span><span class="sxs-lookup"><span data-stu-id="929df-136">definition</span></span>|<span data-ttu-id="929df-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="929df-137">String collection</span></span>| <span data-ttu-id="929df-138">Коллекция строк, содержащая строку JSON, которая определяет правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="929df-138">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="929df-139">Дополнительные сведения о схеме JSON для этого свойства см. ниже.</span><span class="sxs-lookup"><span data-stu-id="929df-139">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="929df-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="929df-140">Required.</span></span>|
|<span data-ttu-id="929df-141">description</span><span class="sxs-lookup"><span data-stu-id="929df-141">description</span></span>|<span data-ttu-id="929df-142">String</span><span class="sxs-lookup"><span data-stu-id="929df-142">String</span></span>| <span data-ttu-id="929df-143">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="929df-143">Description for this policy.</span></span>|
|<span data-ttu-id="929df-144">displayName</span><span class="sxs-lookup"><span data-stu-id="929df-144">displayName</span></span>|<span data-ttu-id="929df-145">String</span><span class="sxs-lookup"><span data-stu-id="929df-145">String</span></span>| <span data-ttu-id="929df-146">Отображаемого имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="929df-146">Display name for this policy.</span></span> <span data-ttu-id="929df-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="929df-147">Required.</span></span>|
|<span data-ttu-id="929df-148">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="929df-148">isOrganizationDefault</span></span>|<span data-ttu-id="929df-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="929df-149">Boolean</span></span>|<span data-ttu-id="929df-150">Если установлено true, активирует эту политику.</span><span class="sxs-lookup"><span data-stu-id="929df-150">If set to true, activates this policy.</span></span> <span data-ttu-id="929df-151">Для одного типа политики может быть несколько политик, но только одна может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="929df-151">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="929df-152">Необязательный, значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="929df-152">Optional, default value is false.</span></span>|


### <a name="properties-of-an-activity-based-timeout-policy-definition"></a><span data-ttu-id="929df-153">Свойства определения политики времени действия</span><span class="sxs-lookup"><span data-stu-id="929df-153">Properties of an activity-based timeout policy definition</span></span>
<span data-ttu-id="929df-154">Свойства ниже формируют объект JSON, который представляет политику времени действия.</span><span class="sxs-lookup"><span data-stu-id="929df-154">The properties below form the JSON object that represents an activity-based timeout policy.</span></span> <span data-ttu-id="929df-155">Этот объект JSON необходимо **преобразовать** в строку с escape-кавычками, чтобы вставить его в **свойство** определения.</span><span class="sxs-lookup"><span data-stu-id="929df-155">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="929df-156">Пример показан ниже в формате JSON:</span><span class="sxs-lookup"><span data-stu-id="929df-156">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```json
{
  "definition":["{\"ActivityBasedTimeoutPolicy\":{\"Version\":1,\"ApplicationPolicies\":[{\"ApplicationId\":\"default\",\"WebSessionIdleTimeout\":\"01:00:00\"},{\"ApplicationId\":\"c44b4083-3bb0-49c1-b47d-974e53cbdf3c\",\"WebSessionIdleTimeout\":\"00:15:00\"}]}}"]
}
```

><span data-ttu-id="929df-157">Примечание. Все сроки в этих свойствах заданы в формате "дд.чч:мм:сс".</span><span class="sxs-lookup"><span data-stu-id="929df-157">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="929df-158">Примечание. Максимальное количество свойств, обозначаемого в "днях", составляет 1 секунду от заметимого количества дней.</span><span class="sxs-lookup"><span data-stu-id="929df-158">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="929df-159">Например, максимальное значение 1 дня указывается как "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="929df-159">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="929df-160">Свойство</span><span class="sxs-lookup"><span data-stu-id="929df-160">Property</span></span>     | <span data-ttu-id="929df-161">Тип</span><span class="sxs-lookup"><span data-stu-id="929df-161">Type</span></span>   |<span data-ttu-id="929df-162">Описание</span><span class="sxs-lookup"><span data-stu-id="929df-162">Description</span></span>|
|:-------------|:------|:---------|
|<span data-ttu-id="929df-163">Версия</span><span class="sxs-lookup"><span data-stu-id="929df-163">Version</span></span>|<span data-ttu-id="929df-164">Целое число</span><span class="sxs-lookup"><span data-stu-id="929df-164">Integer</span></span>|<span data-ttu-id="929df-165">Версия политики.</span><span class="sxs-lookup"><span data-stu-id="929df-165">Policy version.</span></span> <span data-ttu-id="929df-166">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="929df-166">Set value of 1.</span></span> <span data-ttu-id="929df-167">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="929df-167">Required.</span></span>|
|<span data-ttu-id="929df-168">ApplicationPolicies</span><span class="sxs-lookup"><span data-stu-id="929df-168">ApplicationPolicies</span></span>|<span data-ttu-id="929df-169">Объект JSON</span><span class="sxs-lookup"><span data-stu-id="929df-169">JSON object</span></span>|<span data-ttu-id="929df-170">Коллекция политики приложений.</span><span class="sxs-lookup"><span data-stu-id="929df-170">Collection of application policy.</span></span> <span data-ttu-id="929df-171">Политика приложения — это сочетание ApplicationId и WebSessionIdleTimeout:</span><span class="sxs-lookup"><span data-stu-id="929df-171">An application policy, is a combination of an ApplicationId and a WebSessionIdleTimeout:</span></span> <br> <ul><li><span data-ttu-id="929df-172">**ApplicationId**: допустимые значения:</span><span class="sxs-lookup"><span data-stu-id="929df-172">**ApplicationId**: Allowed values:</span></span><ul><li> <span data-ttu-id="929df-173">по умолчанию: применяет политику ко всем приложениям, которые поддерживают функцию времени действия, но не имеют переопределения для конкретного приложения</span><span class="sxs-lookup"><span data-stu-id="929df-173">default: applies the policy to all applications that support activity-based timeout functionality but do not have application-specific override</span></span></li><li> <span data-ttu-id="929df-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: применяет политику к порталу Azure</span><span class="sxs-lookup"><span data-stu-id="929df-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: applies the policy to the Azure Portal</span></span></li></ul></li><li><span data-ttu-id="929df-175">**WebSessionIdleTimeout**: период бездействия пользователя, после которого веб-сеанс пользователя считается просроченным.</span><span class="sxs-lookup"><span data-stu-id="929df-175">**WebSessionIdleTimeout**: The period of user inactivity after which the user's web session is considered expired.</span></span> <span data-ttu-id="929df-176">Минимальное значение — 5 минут; максимальное значение — 1 день.</span><span class="sxs-lookup"><span data-stu-id="929df-176">The minimum value is 5 minutes; the maximum value is 1 day.</span></span></li></ul> |


## <a name="relationships"></a><span data-ttu-id="929df-177">Связи</span><span class="sxs-lookup"><span data-stu-id="929df-177">Relationships</span></span>

<span data-ttu-id="929df-178">Нет</span><span class="sxs-lookup"><span data-stu-id="929df-178">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="929df-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="929df-179">JSON representation</span></span>

<span data-ttu-id="929df-180">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="929df-180">The following is a JSON representation of the resource.</span></span>

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

