---
title: Тип ресурса Континуаусакцессевалуатионполици
description: Оценка непрерывного доступа (КАЕ) помогает управлять сеансами проверки подлинности в режиме реального времени. КАЕ позволяет клиентам обрабатывать доступ к ресурсам, надерживая события для мгновенных вызовов.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a3027dea9a6c264b7af0ab805253946ebda8c97
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023600"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a><span data-ttu-id="e35cd-104">Тип ресурса Континуаусакцессевалуатионполици</span><span class="sxs-lookup"><span data-stu-id="e35cd-104">continuousAccessEvaluationPolicy resource type</span></span>

<span data-ttu-id="e35cd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e35cd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e35cd-106">Оценка непрерывного доступа (КАЕ) управляет сеансами проверки подлинности в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="e35cd-106">Continuous Access Evaluation (CAE) manages authentication sessions in real time.</span></span> <span data-ttu-id="e35cd-107">КАЕ позволяет клиентам обрабатывать доступ к ресурсам, надерживая события для мгновенных вызовов.</span><span class="sxs-lookup"><span data-stu-id="e35cd-107">CAE allows customers to handle access to resources by supporting instant revocation events.</span></span>  <span data-ttu-id="e35cd-108">Более подробную информацию можно узнать в статье [Оценка непрерывного доступа](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).</span><span class="sxs-lookup"><span data-stu-id="e35cd-108">For more information, see the [Continuous access evaluation](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).</span></span>

## <a name="methods"></a><span data-ttu-id="e35cd-109">Методы</span><span class="sxs-lookup"><span data-stu-id="e35cd-109">Methods</span></span>
|<span data-ttu-id="e35cd-110">Метод</span><span class="sxs-lookup"><span data-stu-id="e35cd-110">Method</span></span>|<span data-ttu-id="e35cd-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="e35cd-111">Return type</span></span>|<span data-ttu-id="e35cd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e35cd-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e35cd-113">Получение Континуаусакцессевалуатионполици</span><span class="sxs-lookup"><span data-stu-id="e35cd-113">Get continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-get.md)|[<span data-ttu-id="e35cd-114">континуаусакцессевалуатионполици</span><span class="sxs-lookup"><span data-stu-id="e35cd-114">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="e35cd-115">Чтение свойств объекта [континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e35cd-115">Read the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|[<span data-ttu-id="e35cd-116">Обновление Континуаусакцессевалуатионполици</span><span class="sxs-lookup"><span data-stu-id="e35cd-116">Update continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-update.md)|[<span data-ttu-id="e35cd-117">континуаусакцессевалуатионполици</span><span class="sxs-lookup"><span data-stu-id="e35cd-117">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="e35cd-118">Обновление свойств объекта [континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e35cd-118">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|
## <a name="properties"></a><span data-ttu-id="e35cd-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="e35cd-119">Properties</span></span>
|<span data-ttu-id="e35cd-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="e35cd-120">Property</span></span>|<span data-ttu-id="e35cd-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e35cd-121">Type</span></span>|<span data-ttu-id="e35cd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e35cd-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e35cd-123">description</span><span class="sxs-lookup"><span data-stu-id="e35cd-123">description</span></span>|<span data-ttu-id="e35cd-124">String</span><span class="sxs-lookup"><span data-stu-id="e35cd-124">String</span></span>|<span data-ttu-id="e35cd-125">Оценка непрерывного доступа автоматически блокирует доступ к ресурсам и приложениям почти в режиме реального времени при удалении доступа пользователя или изменении IP-адреса клиента.</span><span class="sxs-lookup"><span data-stu-id="e35cd-125">Continuous access evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.</span></span> <span data-ttu-id="e35cd-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e35cd-126">Read-only.</span></span>|
|<span data-ttu-id="e35cd-127">displayName</span><span class="sxs-lookup"><span data-stu-id="e35cd-127">displayName</span></span>|<span data-ttu-id="e35cd-128">String</span><span class="sxs-lookup"><span data-stu-id="e35cd-128">String</span></span>| <span data-ttu-id="e35cd-129">Значение всегда — "Оценка непрерывного доступа".</span><span class="sxs-lookup"><span data-stu-id="e35cd-129">The value is always 'Continuous Access Evaluation'.</span></span> <span data-ttu-id="e35cd-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e35cd-130">Read-only.</span></span>|
|<span data-ttu-id="e35cd-131">groups</span><span class="sxs-lookup"><span data-stu-id="e35cd-131">groups</span></span>|<span data-ttu-id="e35cd-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e35cd-132">String collection</span></span>|<span data-ttu-id="e35cd-133">Коллекция идентификаторов групп в области для оценки.</span><span class="sxs-lookup"><span data-stu-id="e35cd-133">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="e35cd-134">Если коллекция пуста, все группы находятся в области действия.</span><span class="sxs-lookup"><span data-stu-id="e35cd-134">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="e35cd-135">id</span><span class="sxs-lookup"><span data-stu-id="e35cd-135">id</span></span>|<span data-ttu-id="e35cd-136">String</span><span class="sxs-lookup"><span data-stu-id="e35cd-136">String</span></span>|<span data-ttu-id="e35cd-137">Задает идентификатор объекта Континуаусакцессевалуатионполици.</span><span class="sxs-lookup"><span data-stu-id="e35cd-137">Specifies the identifier of a continuousAccessEvaluationPolicy object.</span></span> <span data-ttu-id="e35cd-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e35cd-138">Read-only.</span></span>|
|<span data-ttu-id="e35cd-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e35cd-139">isEnabled</span></span>|<span data-ttu-id="e35cd-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="e35cd-140">Boolean</span></span>| <span data-ttu-id="e35cd-141">`true` , чтобы указать, следует ли выполнять оценку непрерывного доступа; в противном случае `false` .</span><span class="sxs-lookup"><span data-stu-id="e35cd-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="e35cd-142">users</span><span class="sxs-lookup"><span data-stu-id="e35cd-142">users</span></span>|<span data-ttu-id="e35cd-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e35cd-143">String collection</span></span>|<span data-ttu-id="e35cd-144">Коллекция идентификаторов пользователей в области для оценки.</span><span class="sxs-lookup"><span data-stu-id="e35cd-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="e35cd-145">Если коллекция пуста, все пользователи находятся в области действия.</span><span class="sxs-lookup"><span data-stu-id="e35cd-145">All users are in scope when the collection is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e35cd-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="e35cd-146">Relationships</span></span>
<span data-ttu-id="e35cd-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e35cd-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e35cd-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e35cd-148">JSON representation</span></span>
<span data-ttu-id="e35cd-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e35cd-149">The following is a JSON representation of the resource.</span></span>
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
