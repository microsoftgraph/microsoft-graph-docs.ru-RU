---
title: тип ресурса continuousAccessEvaluationPolicy
description: Непрерывная оценка доступа (CAE) помогает в управлении сеансами проверки подлинности в режиме реального времени. CaE позволяет клиентам обрабатывать доступ к ресурсам, поддерживая события мгновенного отзыва.
author: jerrysai
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f34fdacf75b991ff339f4b7cdd823290438e8fea
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962642"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a><span data-ttu-id="3fe55-104">тип ресурса continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="3fe55-104">continuousAccessEvaluationPolicy resource type</span></span>

<span data-ttu-id="3fe55-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fe55-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fe55-106">Непрерывная оценка доступа (CAE) управляет сеансами проверки подлинности в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="3fe55-106">Continuous Access Evaluation (CAE) manages authentication sessions in real time.</span></span> <span data-ttu-id="3fe55-107">CaE позволяет клиентам обрабатывать доступ к ресурсам, поддерживая события мгновенного отзыва.</span><span class="sxs-lookup"><span data-stu-id="3fe55-107">CAE allows customers to handle access to resources by supporting instant revocation events.</span></span>  <span data-ttu-id="3fe55-108">Дополнительные сведения см. в [оценке непрерывного доступа.](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation)</span><span class="sxs-lookup"><span data-stu-id="3fe55-108">For more information, see the [Continuous access evaluation](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).</span></span>

## <a name="methods"></a><span data-ttu-id="3fe55-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3fe55-109">Methods</span></span>
|<span data-ttu-id="3fe55-110">Метод</span><span class="sxs-lookup"><span data-stu-id="3fe55-110">Method</span></span>|<span data-ttu-id="3fe55-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="3fe55-111">Return type</span></span>|<span data-ttu-id="3fe55-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3fe55-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3fe55-113">Get continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="3fe55-113">Get continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-get.md)|[<span data-ttu-id="3fe55-114">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="3fe55-114">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="3fe55-115">Ознакомьтесь с свойствами объекта [continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3fe55-115">Read the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|[<span data-ttu-id="3fe55-116">Обновление continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="3fe55-116">Update continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-update.md)|[<span data-ttu-id="3fe55-117">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="3fe55-117">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="3fe55-118">Обновление свойств объекта [continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3fe55-118">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|
## <a name="properties"></a><span data-ttu-id="3fe55-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="3fe55-119">Properties</span></span>
|<span data-ttu-id="3fe55-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fe55-120">Property</span></span>|<span data-ttu-id="3fe55-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3fe55-121">Type</span></span>|<span data-ttu-id="3fe55-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3fe55-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fe55-123">description</span><span class="sxs-lookup"><span data-stu-id="3fe55-123">description</span></span>|<span data-ttu-id="3fe55-124">Строка</span><span class="sxs-lookup"><span data-stu-id="3fe55-124">String</span></span>|<span data-ttu-id="3fe55-125">Непрерывная оценка доступа автоматически блокирует доступ к ресурсам и приложениям в режиме реального времени при удалении доступа пользователя или изменениях IP-адресов клиента.</span><span class="sxs-lookup"><span data-stu-id="3fe55-125">Continuous access evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.</span></span> <span data-ttu-id="3fe55-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fe55-126">Read-only.</span></span>|
|<span data-ttu-id="3fe55-127">displayName</span><span class="sxs-lookup"><span data-stu-id="3fe55-127">displayName</span></span>|<span data-ttu-id="3fe55-128">Строка</span><span class="sxs-lookup"><span data-stu-id="3fe55-128">String</span></span>| <span data-ttu-id="3fe55-129">Значение всегда `Continuous Access Evaluation` .</span><span class="sxs-lookup"><span data-stu-id="3fe55-129">The value is always `Continuous Access Evaluation`.</span></span> <span data-ttu-id="3fe55-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fe55-130">Read-only.</span></span>|
|<span data-ttu-id="3fe55-131">groups</span><span class="sxs-lookup"><span data-stu-id="3fe55-131">groups</span></span>|<span data-ttu-id="3fe55-132">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3fe55-132">String collection</span></span>|<span data-ttu-id="3fe55-133">Коллекция идентификаторов групп в области для оценки.</span><span class="sxs-lookup"><span data-stu-id="3fe55-133">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="3fe55-134">Все группы находятся в области, когда коллекция пуста.</span><span class="sxs-lookup"><span data-stu-id="3fe55-134">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="3fe55-135">id</span><span class="sxs-lookup"><span data-stu-id="3fe55-135">id</span></span>|<span data-ttu-id="3fe55-136">Строка</span><span class="sxs-lookup"><span data-stu-id="3fe55-136">String</span></span>|<span data-ttu-id="3fe55-137">Указывает идентификатор объекта [continuousAccessEvaluationPolicy.](#continuousaccessevaluationpolicy-resource-type)</span><span class="sxs-lookup"><span data-stu-id="3fe55-137">Specifies the identifier of a [continuousAccessEvaluationPolicy](#continuousaccessevaluationpolicy-resource-type) object.</span></span> <span data-ttu-id="3fe55-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fe55-138">Read-only.</span></span>|
|<span data-ttu-id="3fe55-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3fe55-139">isEnabled</span></span>|<span data-ttu-id="3fe55-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fe55-140">Boolean</span></span>| <span data-ttu-id="3fe55-141">`true` указать, следует ли проводить оценку непрерывного доступа; в противном `false` случае .</span><span class="sxs-lookup"><span data-stu-id="3fe55-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="3fe55-142">users</span><span class="sxs-lookup"><span data-stu-id="3fe55-142">users</span></span>|<span data-ttu-id="3fe55-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3fe55-143">String collection</span></span>|<span data-ttu-id="3fe55-144">Коллекция идентификаторов пользователей в области для оценки.</span><span class="sxs-lookup"><span data-stu-id="3fe55-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="3fe55-145">Все пользователи находятся в области, когда коллекция пуста.</span><span class="sxs-lookup"><span data-stu-id="3fe55-145">All users are in scope when the collection is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3fe55-146">Связи</span><span class="sxs-lookup"><span data-stu-id="3fe55-146">Relationships</span></span>
<span data-ttu-id="3fe55-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3fe55-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3fe55-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3fe55-148">JSON representation</span></span>
<span data-ttu-id="3fe55-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fe55-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean",
  "users": [
    "String"
  ],
  "groups": [
    "String"
  ]
}
```
