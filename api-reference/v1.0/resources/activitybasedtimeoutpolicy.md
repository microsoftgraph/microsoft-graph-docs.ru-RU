---
title: Тип ресурса Активитибаседтимеаутполици
description: Представляет политику, которая может управлять временем ожидания простоя веб-сеансов для приложений, поддерживающих функциональность времени ожидания на основе действий.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91c8d3933f9ec1fe8e96a5f62c9d00791ffe4777
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003382"
---
# <a name="activitybasedtimeoutpolicy-resource-type"></a><span data-ttu-id="fe8fc-103">Тип ресурса Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="fe8fc-103">activityBasedTimeoutPolicy resource type</span></span>

<span data-ttu-id="fe8fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe8fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe8fc-105">Представляет политику, которая может управлять временем ожидания простоя веб-сеансов для приложений, поддерживающих функциональность времени ожидания на основе действий.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-105">Represents a policy that can control the idle timeout for web sessions for applications that support activity-based timeout functionality.</span></span> <span data-ttu-id="fe8fc-106">Приложения принудительно применяют функцию автоматического выхода после периода бездействия.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-106">Applications enforce automatic signout after a period of inactivity.</span></span> <span data-ttu-id="fe8fc-107">Этот тип политики можно применять только на уровне Организации (путем установки для свойства **исорганизатиондефаулт** значения `true` ).</span><span class="sxs-lookup"><span data-stu-id="fe8fc-107">This type of policy can only be applied at the organization level (by setting the **isOrganizationDefault** property to `true`).</span></span>

<span data-ttu-id="fe8fc-108">Наследуется от [стсполици](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fe8fc-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fe8fc-109">Методы</span><span class="sxs-lookup"><span data-stu-id="fe8fc-109">Methods</span></span>

| <span data-ttu-id="fe8fc-110">Метод</span><span class="sxs-lookup"><span data-stu-id="fe8fc-110">Method</span></span>       | <span data-ttu-id="fe8fc-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fe8fc-111">Return Type</span></span> | <span data-ttu-id="fe8fc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fe8fc-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fe8fc-113">Список АктивитибаседтимеаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="fe8fc-113">List activityBasedTimeoutPolicies</span></span>](../api/activitybasedtimeoutpolicy-list.md) | [<span data-ttu-id="fe8fc-114">активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="fe8fc-114">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="fe8fc-115">Чтение свойств и связей объектов Активитибаседтимеаутполици.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-115">Read properties and relationships of activityBasedTimeoutPolicy objects.</span></span> |
| [<span data-ttu-id="fe8fc-116">Создание Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="fe8fc-116">Create activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-post-activitybasedtimeoutpolicies.md) | [<span data-ttu-id="fe8fc-117">активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="fe8fc-117">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="fe8fc-118">Создание объекта Активитибаседтимеаутполици.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-118">Create an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="fe8fc-119">Получение Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="fe8fc-119">Get activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-get.md) | [<span data-ttu-id="fe8fc-120">активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="fe8fc-120">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="fe8fc-121">Чтение свойств и связей объекта Активитибаседтимеаутполици.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-121">Read properties and relationships of an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="fe8fc-122">Обновление Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="fe8fc-122">Update activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-update.md) | <span data-ttu-id="fe8fc-123">Нет</span><span class="sxs-lookup"><span data-stu-id="fe8fc-123">None</span></span> | <span data-ttu-id="fe8fc-124">Обновление объекта Активитибаседтимеаутполици.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-124">Update an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="fe8fc-125">Удаление Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="fe8fc-125">Delete activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-delete.md) | <span data-ttu-id="fe8fc-126">Нет</span><span class="sxs-lookup"><span data-stu-id="fe8fc-126">None</span></span> | <span data-ttu-id="fe8fc-127">Удаление объекта Активитибаседтимеаутполици.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-127">Delete an activityBasedTimeoutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fe8fc-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe8fc-128">Properties</span></span>

| <span data-ttu-id="fe8fc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe8fc-129">Property</span></span>     | <span data-ttu-id="fe8fc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fe8fc-130">Type</span></span>        | <span data-ttu-id="fe8fc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fe8fc-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fe8fc-132">id</span><span class="sxs-lookup"><span data-stu-id="fe8fc-132">id</span></span>|<span data-ttu-id="fe8fc-133">String</span><span class="sxs-lookup"><span data-stu-id="fe8fc-133">String</span></span>| <span data-ttu-id="fe8fc-134">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-134">Unique identifier for this policy.</span></span> <span data-ttu-id="fe8fc-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-135">Read-only.</span></span>|
|<span data-ttu-id="fe8fc-136">RDLC</span><span class="sxs-lookup"><span data-stu-id="fe8fc-136">definition</span></span>|<span data-ttu-id="fe8fc-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fe8fc-137">String collection</span></span>| <span data-ttu-id="fe8fc-138">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-138">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="fe8fc-139">Ниже приведены дополнительные сведения о схеме JSON для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-139">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="fe8fc-140">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-140">Required.</span></span>|
|<span data-ttu-id="fe8fc-141">description</span><span class="sxs-lookup"><span data-stu-id="fe8fc-141">description</span></span>|<span data-ttu-id="fe8fc-142">String</span><span class="sxs-lookup"><span data-stu-id="fe8fc-142">String</span></span>| <span data-ttu-id="fe8fc-143">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-143">Description for this policy.</span></span>|
|<span data-ttu-id="fe8fc-144">displayName</span><span class="sxs-lookup"><span data-stu-id="fe8fc-144">displayName</span></span>|<span data-ttu-id="fe8fc-145">String</span><span class="sxs-lookup"><span data-stu-id="fe8fc-145">String</span></span>| <span data-ttu-id="fe8fc-146">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-146">Display name for this policy.</span></span> <span data-ttu-id="fe8fc-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-147">Required.</span></span>|
|<span data-ttu-id="fe8fc-148">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="fe8fc-148">isOrganizationDefault</span></span>|<span data-ttu-id="fe8fc-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe8fc-149">Boolean</span></span>|<span data-ttu-id="fe8fc-150">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-150">If set to true, activates this policy.</span></span> <span data-ttu-id="fe8fc-151">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-151">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="fe8fc-152">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-152">Optional, default value is false.</span></span>|


### <a name="properties-of-an-activity-based-timeout-policy-definition"></a><span data-ttu-id="fe8fc-153">Свойства определения политики времени ожидания на основе действий</span><span class="sxs-lookup"><span data-stu-id="fe8fc-153">Properties of an activity-based timeout policy definition</span></span>
<span data-ttu-id="fe8fc-154">Свойства, приведенные ниже, формируют объект JSON, представляющий политику времени ожидания, основанную на действиях.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-154">The properties below form the JSON object that represents an activity-based timeout policy.</span></span> <span data-ttu-id="fe8fc-155">Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** .</span><span class="sxs-lookup"><span data-stu-id="fe8fc-155">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="fe8fc-156">Ниже показан пример в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-156">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```json
{
  "definition":["{\"ActivityBasedTimeoutPolicy\":{\"Version\":1,\"ApplicationPolicies\":[{\"ApplicationId\":\"default\",\"WebSessionIdleTimeout\":\"01:00:00\"},{\"ApplicationId\":\"c44b4083-3bb0-49c1-b47d-974e53cbdf3c\",\"WebSessionIdleTimeout\":\"00:15:00\"}]}}"]
}
```

><span data-ttu-id="fe8fc-157">**Примечание:** Все временные интервалы в этих свойствах указываются в формате "DD. чч: мм: СС".</span><span class="sxs-lookup"><span data-stu-id="fe8fc-157">**Note:** All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="fe8fc-158">**Примечание:** Максимальные значения свойств, обозначенных в "Days", задаются в течение 1 секунды с заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-158">**Note:** Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="fe8fc-159">Например, максимальное значение в 1 день задается как "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="fe8fc-159">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="fe8fc-160">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe8fc-160">Property</span></span>     | <span data-ttu-id="fe8fc-161">Тип</span><span class="sxs-lookup"><span data-stu-id="fe8fc-161">Type</span></span>   |<span data-ttu-id="fe8fc-162">Описание</span><span class="sxs-lookup"><span data-stu-id="fe8fc-162">Description</span></span>|
|:-------------|:------|:---------|
|<span data-ttu-id="fe8fc-163">Версия</span><span class="sxs-lookup"><span data-stu-id="fe8fc-163">Version</span></span>|<span data-ttu-id="fe8fc-164">Целое число</span><span class="sxs-lookup"><span data-stu-id="fe8fc-164">Integer</span></span>|<span data-ttu-id="fe8fc-165">Версия политики.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-165">Policy version.</span></span> <span data-ttu-id="fe8fc-166">Установите значение 1.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-166">Set value of 1.</span></span> <span data-ttu-id="fe8fc-167">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-167">Required.</span></span>|
|<span data-ttu-id="fe8fc-168">аппликатионполиЦиес</span><span class="sxs-lookup"><span data-stu-id="fe8fc-168">ApplicationPolicies</span></span>|<span data-ttu-id="fe8fc-169">Объект JSON</span><span class="sxs-lookup"><span data-stu-id="fe8fc-169">JSON object</span></span>|<span data-ttu-id="fe8fc-170">Коллекция политики приложений.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-170">Collection of application policy.</span></span> <span data-ttu-id="fe8fc-171">Политика приложений — это сочетание объекта ApplicationId и объекта Вебсессионидлетимеаут:</span><span class="sxs-lookup"><span data-stu-id="fe8fc-171">An application policy, is a combination of an ApplicationId and a WebSessionIdleTimeout:</span></span> <br> <ul><li><span data-ttu-id="fe8fc-172">**ApplicationId**: допустимые значения:</span><span class="sxs-lookup"><span data-stu-id="fe8fc-172">**ApplicationId**: Allowed values:</span></span><ul><li> <span data-ttu-id="fe8fc-173">по умолчанию: применяет политику ко всем приложениям, поддерживающим функциональность времени ожидания на основе действий, но не зависящее от приложения</span><span class="sxs-lookup"><span data-stu-id="fe8fc-173">default: applies the policy to all applications that support activity-based timeout functionality but do not have application-specific override</span></span></li><li> <span data-ttu-id="fe8fc-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: применение политики к порталу Azure</span><span class="sxs-lookup"><span data-stu-id="fe8fc-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: applies the policy to the Azure Portal</span></span></li></ul></li><li><span data-ttu-id="fe8fc-175">**Вебсессионидлетимеаут**: период бездействия пользователя, по истечении которого срок действия веб-сеанса пользователя считается истекшим.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-175">**WebSessionIdleTimeout**: The period of user inactivity after which the user's web session is considered expired.</span></span> <span data-ttu-id="fe8fc-176">Минимальное значение — 5 минут; Максимальное значение — 1 день.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-176">The minimum value is 5 minutes; the maximum value is 1 day.</span></span></li></ul> |


## <a name="relationships"></a><span data-ttu-id="fe8fc-177">Связи</span><span class="sxs-lookup"><span data-stu-id="fe8fc-177">Relationships</span></span>

<span data-ttu-id="fe8fc-178">Нет</span><span class="sxs-lookup"><span data-stu-id="fe8fc-178">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe8fc-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe8fc-179">JSON representation</span></span>

<span data-ttu-id="fe8fc-180">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe8fc-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
  "baseType": "",
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

