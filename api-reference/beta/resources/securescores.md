---
title: Тип ресурса secureScores
description: 'в начало = n, где n — число дней данных, которую необходимо получить. '
ms.openlocfilehash: 96d5c487bb854559b0128d93ea8e0783fcc61f0c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075650"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="f3f03-103">Тип ресурса secureScores</span><span class="sxs-lookup"><span data-stu-id="f3f03-103">secureScores resource type</span></span>

> <span data-ttu-id="f3f03-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f3f03-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3f03-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3f03-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3f03-106">Представляет безопасной счета клиента в день для оценки данных, на уровне клиента и элемента управления.</span><span class="sxs-lookup"><span data-stu-id="f3f03-106">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="f3f03-107">По умолчанию проводится данных в течение 90 дней.</span><span class="sxs-lookup"><span data-stu-id="f3f03-107">By default, 90 days of data is held.</span></span> <span data-ttu-id="f3f03-108">Эти данные сортируются по **createdDateTime**от поздних к ранним.</span><span class="sxs-lookup"><span data-stu-id="f3f03-108">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="f3f03-109">Это позволит вам для запросов с помощью $top = n, где n — число дней данных, которую необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="f3f03-109">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="f3f03-110">Методы</span><span class="sxs-lookup"><span data-stu-id="f3f03-110">Methods</span></span>

| <span data-ttu-id="f3f03-111">Метод</span><span class="sxs-lookup"><span data-stu-id="f3f03-111">Method</span></span>   | <span data-ttu-id="f3f03-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f3f03-112">Return Type</span></span>|<span data-ttu-id="f3f03-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f3f03-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f3f03-114">Список secureScores</span><span class="sxs-lookup"><span data-stu-id="f3f03-114">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="f3f03-115">secureScores</span><span class="sxs-lookup"><span data-stu-id="f3f03-115">secureScores</span></span>](securescores.md) |<span data-ttu-id="f3f03-116">Чтение свойства и метаданные объекта secureScores.</span><span class="sxs-lookup"><span data-stu-id="f3f03-116">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="f3f03-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3f03-117">Properties</span></span>
<span data-ttu-id="f3f03-118">Свойства содержащий тип сущности безопасности клиента широкополосном (ежедневного моментальный снимок данных).</span><span class="sxs-lookup"><span data-stu-id="f3f03-118">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="f3f03-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3f03-119">Property</span></span> |<span data-ttu-id="f3f03-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f3f03-120">Type</span></span> |<span data-ttu-id="f3f03-121">Description</span><span class="sxs-lookup"><span data-stu-id="f3f03-121">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="f3f03-122">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="f3f03-122">azureTenantId</span></span>   |   <span data-ttu-id="f3f03-123">String</span><span class="sxs-lookup"><span data-stu-id="f3f03-123">String</span></span>  |   <span data-ttu-id="f3f03-124">Идентификатор GUID строки для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3f03-124">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="f3f03-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3f03-125">createdDateTime</span></span> |   <span data-ttu-id="f3f03-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3f03-126">DateTimeOffset</span></span>  |   <span data-ttu-id="f3f03-127">Дата создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f3f03-127">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="f3f03-128">id</span><span class="sxs-lookup"><span data-stu-id="f3f03-128">id</span></span>  |   <span data-ttu-id="f3f03-129">String</span><span class="sxs-lookup"><span data-stu-id="f3f03-129">String</span></span>  |   <span data-ttu-id="f3f03-130">Сочетание azureTenantId_createdDateTime.</span><span class="sxs-lookup"><span data-stu-id="f3f03-130">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="f3f03-131">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="f3f03-131">licensedUserCount</span></span>   |   <span data-ttu-id="f3f03-132">Int32</span><span class="sxs-lookup"><span data-stu-id="f3f03-132">Int32</span></span>   |   <span data-ttu-id="f3f03-133">Число пользователей данного клиента с корпоративным лицензированием.</span><span class="sxs-lookup"><span data-stu-id="f3f03-133">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="f3f03-134">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="f3f03-134">activeUserCount</span></span> |   <span data-ttu-id="f3f03-135">Int32</span><span class="sxs-lookup"><span data-stu-id="f3f03-135">Int32</span></span>   |   <span data-ttu-id="f3f03-136">Число активных пользователей указанного клиента.</span><span class="sxs-lookup"><span data-stu-id="f3f03-136">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="f3f03-137">currentScore</span><span class="sxs-lookup"><span data-stu-id="f3f03-137">currentScore</span></span>    |   <span data-ttu-id="f3f03-138">Double</span><span class="sxs-lookup"><span data-stu-id="f3f03-138">Double</span></span>  |   <span data-ttu-id="f3f03-139">Оценка текущего обновления клиента на указанной даты.</span><span class="sxs-lookup"><span data-stu-id="f3f03-139">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="f3f03-140">maxScore</span><span class="sxs-lookup"><span data-stu-id="f3f03-140">maxScore</span></span> |  <span data-ttu-id="f3f03-141">Double</span><span class="sxs-lookup"><span data-stu-id="f3f03-141">Double</span></span>  |   <span data-ttu-id="f3f03-142">Клиент максимальное возможному значению на указанной даты.</span><span class="sxs-lookup"><span data-stu-id="f3f03-142">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="f3f03-143">enabledServices</span><span class="sxs-lookup"><span data-stu-id="f3f03-143">enabledServices</span></span> |   <span data-ttu-id="f3f03-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f3f03-144">String collection</span></span>   |   <span data-ttu-id="f3f03-145">Службы Майкрософт для клиента (например, Exchange online, Скайп, Sharepoint).</span><span class="sxs-lookup"><span data-stu-id="f3f03-145">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="f3f03-146">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="f3f03-146">averageComparativeScores</span></span> |  <span data-ttu-id="f3f03-147">[averageComparativeScore](averagecomparativescore.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f3f03-147">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="f3f03-148">Средняя оценка по различные области (например, среднее число разных отраслей, среднее, число) и элемент управления категории (удостоверения, данные, устройства, приложения, инфраструктуры) в области действия.</span><span class="sxs-lookup"><span data-stu-id="f3f03-148">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="f3f03-149">controlScores</span><span class="sxs-lookup"><span data-stu-id="f3f03-149">controlScores</span></span> | <span data-ttu-id="f3f03-150">[controlScore](controlscore.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f3f03-150">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="f3f03-151">Содержит показателям клиента для набора элементов управления.</span><span class="sxs-lookup"><span data-stu-id="f3f03-151">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="f3f03-152">Связи</span><span class="sxs-lookup"><span data-stu-id="f3f03-152">Relationships</span></span>

<span data-ttu-id="f3f03-153">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f3f03-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3f03-154">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f3f03-154">JSON representation</span></span>

<span data-ttu-id="f3f03-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3f03-155">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"id": "String",
"azureTenantId": "Guid",
"createdDate": "DateTimeOffset",
"licensedUserCount": "Int32",
"activeUserCount": "Int32",
"currentScore": "Int32",
"maxScore": "Int32",
"averageScore": "Double",
"enabledServices": "Collection(string)",
"averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
"controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
}

```


<!-- {
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
