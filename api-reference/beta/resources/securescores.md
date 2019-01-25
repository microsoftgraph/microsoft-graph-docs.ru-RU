---
title: Тип ресурса secureScores
description: 'в начало = n, где n — число дней данных, которую необходимо получить. '
localization_priority: Normal
ms.openlocfilehash: 8b4be9822b782303efe38dbdf5bd43e1ee543421
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528664"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="9e57f-103">Тип ресурса secureScores</span><span class="sxs-lookup"><span data-stu-id="9e57f-103">secureScores resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e57f-104">Представляет безопасной счета клиента в день для оценки данных, на уровне клиента и элемента управления.</span><span class="sxs-lookup"><span data-stu-id="9e57f-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="9e57f-105">По умолчанию проводится данных в течение 90 дней.</span><span class="sxs-lookup"><span data-stu-id="9e57f-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="9e57f-106">Эти данные сортируются по **createdDateTime**от поздних к ранним.</span><span class="sxs-lookup"><span data-stu-id="9e57f-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="9e57f-107">Это позволит вам для запросов с помощью $top = n, где n — число дней данных, которую необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="9e57f-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="9e57f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="9e57f-108">Methods</span></span>

| <span data-ttu-id="9e57f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="9e57f-109">Method</span></span>   | <span data-ttu-id="9e57f-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9e57f-110">Return Type</span></span>|<span data-ttu-id="9e57f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9e57f-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9e57f-112">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="9e57f-112">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="9e57f-113">secureScores</span><span class="sxs-lookup"><span data-stu-id="9e57f-113">secureScores</span></span>](securescores.md) |<span data-ttu-id="9e57f-114">Чтение свойства и метаданные объекта secureScores.</span><span class="sxs-lookup"><span data-stu-id="9e57f-114">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="9e57f-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e57f-115">Properties</span></span>
<span data-ttu-id="9e57f-116">Свойства содержащий тип сущности безопасности клиента широкополосном (ежедневного моментальный снимок данных).</span><span class="sxs-lookup"><span data-stu-id="9e57f-116">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="9e57f-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e57f-117">Property</span></span> |<span data-ttu-id="9e57f-118">Тип</span><span class="sxs-lookup"><span data-stu-id="9e57f-118">Type</span></span> |<span data-ttu-id="9e57f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9e57f-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="9e57f-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="9e57f-120">azureTenantId</span></span>   |   <span data-ttu-id="9e57f-121">String</span><span class="sxs-lookup"><span data-stu-id="9e57f-121">String</span></span>  |   <span data-ttu-id="9e57f-122">Идентификатор GUID строки для клиента.</span><span class="sxs-lookup"><span data-stu-id="9e57f-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="9e57f-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e57f-123">createdDateTime</span></span> |   <span data-ttu-id="9e57f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e57f-124">DateTimeOffset</span></span>  |   <span data-ttu-id="9e57f-125">Дата создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9e57f-125">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="9e57f-126">id</span><span class="sxs-lookup"><span data-stu-id="9e57f-126">id</span></span>  |   <span data-ttu-id="9e57f-127">String</span><span class="sxs-lookup"><span data-stu-id="9e57f-127">String</span></span>  |   <span data-ttu-id="9e57f-128">Сочетание azureTenantId_createdDateTime.</span><span class="sxs-lookup"><span data-stu-id="9e57f-128">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="9e57f-129">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="9e57f-129">licensedUserCount</span></span>   |   <span data-ttu-id="9e57f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="9e57f-130">Int32</span></span>   |   <span data-ttu-id="9e57f-131">Число пользователей данного клиента с корпоративным лицензированием.</span><span class="sxs-lookup"><span data-stu-id="9e57f-131">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="9e57f-132">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="9e57f-132">activeUserCount</span></span> |   <span data-ttu-id="9e57f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="9e57f-133">Int32</span></span>   |   <span data-ttu-id="9e57f-134">Число активных пользователей указанного клиента.</span><span class="sxs-lookup"><span data-stu-id="9e57f-134">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="9e57f-135">currentScore</span><span class="sxs-lookup"><span data-stu-id="9e57f-135">currentScore</span></span>    |   <span data-ttu-id="9e57f-136">Double</span><span class="sxs-lookup"><span data-stu-id="9e57f-136">Double</span></span>  |   <span data-ttu-id="9e57f-137">Оценка текущего обновления клиента на указанной даты.</span><span class="sxs-lookup"><span data-stu-id="9e57f-137">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="9e57f-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="9e57f-138">maxScore</span></span> |  <span data-ttu-id="9e57f-139">Double</span><span class="sxs-lookup"><span data-stu-id="9e57f-139">Double</span></span>  |   <span data-ttu-id="9e57f-140">Клиент максимальное возможному значению на указанной даты.</span><span class="sxs-lookup"><span data-stu-id="9e57f-140">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="9e57f-141">enabledServices</span><span class="sxs-lookup"><span data-stu-id="9e57f-141">enabledServices</span></span> |   <span data-ttu-id="9e57f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9e57f-142">String collection</span></span>   |   <span data-ttu-id="9e57f-143">Службы Майкрософт для клиента (например, Exchange online, Скайп, Sharepoint).</span><span class="sxs-lookup"><span data-stu-id="9e57f-143">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="9e57f-144">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="9e57f-144">averageComparativeScores</span></span> |  <span data-ttu-id="9e57f-145">[averageComparativeScore](averagecomparativescore.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9e57f-145">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="9e57f-146">Средняя оценка по различные области (например, среднее число разных отраслей, среднее, число) и элемент управления категории (удостоверения, данные, устройства, приложения, инфраструктуры) в области действия.</span><span class="sxs-lookup"><span data-stu-id="9e57f-146">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="9e57f-147">controlScores</span><span class="sxs-lookup"><span data-stu-id="9e57f-147">controlScores</span></span> | <span data-ttu-id="9e57f-148">[controlScore](controlscore.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9e57f-148">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="9e57f-149">Содержит показателям клиента для набора элементов управления.</span><span class="sxs-lookup"><span data-stu-id="9e57f-149">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="9e57f-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="9e57f-150">Relationships</span></span>

<span data-ttu-id="9e57f-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9e57f-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e57f-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9e57f-152">JSON representation</span></span>

<span data-ttu-id="9e57f-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e57f-153">The following is a JSON representation of the resource.</span></span>

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


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescores.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
