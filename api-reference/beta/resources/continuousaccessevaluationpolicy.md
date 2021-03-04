---
title: тип ресурса continuousAccessEvaluationPolicy
description: Непрерывная оценка доступа (CAE) помогает в управлении сеансами проверки подлинности в режиме реального времени. CaE позволяет клиентам обрабатывать доступ к ресурсам, поддерживая события мгновенного отзыва.
author: jerrysai
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 58c4f913c8a5fc3b4f7c1c129c7126437035cbe7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444282"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a><span data-ttu-id="335a3-104">тип ресурса continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="335a3-104">continuousAccessEvaluationPolicy resource type</span></span>

<span data-ttu-id="335a3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="335a3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="335a3-106">Непрерывная оценка доступа (CAE) управляет сеансами проверки подлинности в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="335a3-106">Continuous Access Evaluation (CAE) manages authentication sessions in real time.</span></span> <span data-ttu-id="335a3-107">CaE позволяет клиентам обрабатывать доступ к ресурсам, поддерживая события мгновенного отзыва.</span><span class="sxs-lookup"><span data-stu-id="335a3-107">CAE allows customers to handle access to resources by supporting instant revocation events.</span></span>  <span data-ttu-id="335a3-108">Дополнительные сведения см. в [оценке непрерывного доступа.](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation)</span><span class="sxs-lookup"><span data-stu-id="335a3-108">For more information, see the [Continuous access evaluation](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).</span></span>

## <a name="methods"></a><span data-ttu-id="335a3-109">Методы</span><span class="sxs-lookup"><span data-stu-id="335a3-109">Methods</span></span>
|<span data-ttu-id="335a3-110">Метод</span><span class="sxs-lookup"><span data-stu-id="335a3-110">Method</span></span>|<span data-ttu-id="335a3-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="335a3-111">Return type</span></span>|<span data-ttu-id="335a3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="335a3-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="335a3-113">Get continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="335a3-113">Get continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-get.md)|[<span data-ttu-id="335a3-114">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="335a3-114">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="335a3-115">Ознакомьтесь с свойствами объекта [continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="335a3-115">Read the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|[<span data-ttu-id="335a3-116">Обновление continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="335a3-116">Update continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-update.md)|[<span data-ttu-id="335a3-117">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="335a3-117">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="335a3-118">Обновление свойств объекта [continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="335a3-118">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|
## <a name="properties"></a><span data-ttu-id="335a3-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="335a3-119">Properties</span></span>
|<span data-ttu-id="335a3-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="335a3-120">Property</span></span>|<span data-ttu-id="335a3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="335a3-121">Type</span></span>|<span data-ttu-id="335a3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="335a3-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="335a3-123">description</span><span class="sxs-lookup"><span data-stu-id="335a3-123">description</span></span>|<span data-ttu-id="335a3-124">String</span><span class="sxs-lookup"><span data-stu-id="335a3-124">String</span></span>|<span data-ttu-id="335a3-125">Непрерывная оценка доступа автоматически блокирует доступ к ресурсам и приложениям в режиме реального времени при удалении доступа пользователя или изменениях IP-адресов клиента.</span><span class="sxs-lookup"><span data-stu-id="335a3-125">Continuous access evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.</span></span> <span data-ttu-id="335a3-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="335a3-126">Read-only.</span></span>|
|<span data-ttu-id="335a3-127">displayName</span><span class="sxs-lookup"><span data-stu-id="335a3-127">displayName</span></span>|<span data-ttu-id="335a3-128">String</span><span class="sxs-lookup"><span data-stu-id="335a3-128">String</span></span>| <span data-ttu-id="335a3-129">Значение всегда является "Оценка непрерывного доступа".</span><span class="sxs-lookup"><span data-stu-id="335a3-129">The value is always 'Continuous Access Evaluation'.</span></span> <span data-ttu-id="335a3-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="335a3-130">Read-only.</span></span>|
|<span data-ttu-id="335a3-131">groups</span><span class="sxs-lookup"><span data-stu-id="335a3-131">groups</span></span>|<span data-ttu-id="335a3-132">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="335a3-132">String collection</span></span>|<span data-ttu-id="335a3-133">Коллекция идентификаторов групп в области для оценки.</span><span class="sxs-lookup"><span data-stu-id="335a3-133">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="335a3-134">Все группы находятся в области, когда коллекция пуста.</span><span class="sxs-lookup"><span data-stu-id="335a3-134">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="335a3-135">id</span><span class="sxs-lookup"><span data-stu-id="335a3-135">id</span></span>|<span data-ttu-id="335a3-136">String</span><span class="sxs-lookup"><span data-stu-id="335a3-136">String</span></span>|<span data-ttu-id="335a3-137">Указывает идентификатор объекта continuousAccessEvaluationPolicy.</span><span class="sxs-lookup"><span data-stu-id="335a3-137">Specifies the identifier of a continuousAccessEvaluationPolicy object.</span></span> <span data-ttu-id="335a3-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="335a3-138">Read-only.</span></span>|
|<span data-ttu-id="335a3-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="335a3-139">isEnabled</span></span>|<span data-ttu-id="335a3-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="335a3-140">Boolean</span></span>| <span data-ttu-id="335a3-141">`true` указать, следует ли проводить оценку непрерывного доступа; в противном `false` случае .</span><span class="sxs-lookup"><span data-stu-id="335a3-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="335a3-142">users</span><span class="sxs-lookup"><span data-stu-id="335a3-142">users</span></span>|<span data-ttu-id="335a3-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="335a3-143">String collection</span></span>|<span data-ttu-id="335a3-144">Коллекция идентификаторов пользователей в области для оценки.</span><span class="sxs-lookup"><span data-stu-id="335a3-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="335a3-145">Все пользователи находятся в области, когда коллекция пуста.</span><span class="sxs-lookup"><span data-stu-id="335a3-145">All users are in scope when the collection is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="335a3-146">Связи</span><span class="sxs-lookup"><span data-stu-id="335a3-146">Relationships</span></span>
<span data-ttu-id="335a3-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="335a3-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="335a3-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="335a3-148">JSON representation</span></span>
<span data-ttu-id="335a3-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="335a3-149">The following is a JSON representation of the resource.</span></span>
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
