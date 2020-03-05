---
title: Тип ресурса Секурескоре
description: 'TOP = n, где n — это количество дней, в течение которых требуется получить данные. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9c699ced69587d3e9791d22bc464013907319620
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520859"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="5851a-103">Тип ресурса Секурескоре</span><span class="sxs-lookup"><span data-stu-id="5851a-103">secureScore resource type</span></span>

<span data-ttu-id="5851a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5851a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5851a-105">Представляет безопасное значение клиента в день данных оценки на уровне клиента и элемента управления.</span><span class="sxs-lookup"><span data-stu-id="5851a-105">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="5851a-106">По умолчанию данные хранятся в 90 дней.</span><span class="sxs-lookup"><span data-stu-id="5851a-106">By default, 90 days of data is held.</span></span> <span data-ttu-id="5851a-107">Эти данные сортируются по **createdDateTime**, от последних к ранним.</span><span class="sxs-lookup"><span data-stu-id="5851a-107">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="5851a-108">Это позволит получать ответы на страницы с помощью $top = n, где n = число дней, которые требуется получить.</span><span class="sxs-lookup"><span data-stu-id="5851a-108">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="5851a-109">Методы</span><span class="sxs-lookup"><span data-stu-id="5851a-109">Methods</span></span>

| <span data-ttu-id="5851a-110">Метод</span><span class="sxs-lookup"><span data-stu-id="5851a-110">Method</span></span>   | <span data-ttu-id="5851a-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5851a-111">Return Type</span></span>|<span data-ttu-id="5851a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5851a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5851a-113">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="5851a-113">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="5851a-114">secureScores</span><span class="sxs-lookup"><span data-stu-id="5851a-114">secureScores</span></span>](securescores.md) |<span data-ttu-id="5851a-115">Чтение свойств и метаданных объекта Секурескорес.</span><span class="sxs-lookup"><span data-stu-id="5851a-115">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="5851a-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="5851a-116">Properties</span></span>
<span data-ttu-id="5851a-117">Тип объекта, содержащий свойства оценки безопасности клиента (ежедневные данные моментального снимка).</span><span class="sxs-lookup"><span data-stu-id="5851a-117">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="5851a-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="5851a-118">Property</span></span> |<span data-ttu-id="5851a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5851a-119">Type</span></span> |<span data-ttu-id="5851a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5851a-120">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="5851a-121">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="5851a-121">azureTenantId</span></span>   |   <span data-ttu-id="5851a-122">String</span><span class="sxs-lookup"><span data-stu-id="5851a-122">String</span></span>  |   <span data-ttu-id="5851a-123">Строка GUID для идентификатора клиента.</span><span class="sxs-lookup"><span data-stu-id="5851a-123">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="5851a-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5851a-124">createdDateTime</span></span> |   <span data-ttu-id="5851a-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5851a-125">DateTimeOffset</span></span>  |   <span data-ttu-id="5851a-126">Дата создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5851a-126">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="5851a-127">id</span><span class="sxs-lookup"><span data-stu-id="5851a-127">id</span></span>  |   <span data-ttu-id="5851a-128">Строка</span><span class="sxs-lookup"><span data-stu-id="5851a-128">String</span></span>  |   <span data-ttu-id="5851a-129">Сочетание azureTenantId_createdDateTime.</span><span class="sxs-lookup"><span data-stu-id="5851a-129">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="5851a-130">лиценседусеркаунт</span><span class="sxs-lookup"><span data-stu-id="5851a-130">licensedUserCount</span></span>   |   <span data-ttu-id="5851a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="5851a-131">Int32</span></span>   |   <span data-ttu-id="5851a-132">Число лицензированных пользователей для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="5851a-132">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="5851a-133">активеусеркаунт</span><span class="sxs-lookup"><span data-stu-id="5851a-133">activeUserCount</span></span> |   <span data-ttu-id="5851a-134">Int32</span><span class="sxs-lookup"><span data-stu-id="5851a-134">Int32</span></span>   |   <span data-ttu-id="5851a-135">Число активных пользователей для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="5851a-135">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="5851a-136">куррентскоре</span><span class="sxs-lookup"><span data-stu-id="5851a-136">currentScore</span></span>    |   <span data-ttu-id="5851a-137">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="5851a-137">Double</span></span>  |   <span data-ttu-id="5851a-138">Текущий полученный рейтинг клиента на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="5851a-138">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="5851a-139">максскоре</span><span class="sxs-lookup"><span data-stu-id="5851a-139">maxScore</span></span> |  <span data-ttu-id="5851a-140">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="5851a-140">Double</span></span>  |   <span data-ttu-id="5851a-141">Максимальная возможная Оценка клиента на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="5851a-141">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="5851a-142">енабледсервицес</span><span class="sxs-lookup"><span data-stu-id="5851a-142">enabledServices</span></span> |   <span data-ttu-id="5851a-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5851a-143">String collection</span></span>   |   <span data-ttu-id="5851a-144">Службы, предоставляемые корпорацией Майкрософт для клиента (например, Exchange Online, Skype, SharePoint).</span><span class="sxs-lookup"><span data-stu-id="5851a-144">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="5851a-145">аверажекомпаративескорес</span><span class="sxs-lookup"><span data-stu-id="5851a-145">averageComparativeScores</span></span> |  <span data-ttu-id="5851a-146">Коллекция [аверажекомпаративескоре](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="5851a-146">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="5851a-147">Средняя оценка по различным областям (например, усреднение по отраслям, среднему на количество участников) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура) в области.</span><span class="sxs-lookup"><span data-stu-id="5851a-147">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="5851a-148">контролскорес</span><span class="sxs-lookup"><span data-stu-id="5851a-148">controlScores</span></span> | <span data-ttu-id="5851a-149">Коллекция [контролскоре](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="5851a-149">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="5851a-150">Содержит результаты клиентов для набора элементов управления.</span><span class="sxs-lookup"><span data-stu-id="5851a-150">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="5851a-151">Связи</span><span class="sxs-lookup"><span data-stu-id="5851a-151">Relationships</span></span>

<span data-ttu-id="5851a-152">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5851a-152">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5851a-153">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5851a-153">JSON representation</span></span>

<span data-ttu-id="5851a-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5851a-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
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
  "createdDateTime": "2019-02-07T20:33:53.156Z"
}

```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
