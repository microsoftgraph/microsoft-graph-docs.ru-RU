---
title: Тип ресурса Секурескоре
description: 'TOP = n, где n — это количество дней, в течение которых требуется получить данные. '
localization_priority: Normal
ms.openlocfilehash: 1f4ee37b5e257cfb914f45a1260f3572403f00dd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343383"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="1bb0f-103">Тип ресурса Секурескоре</span><span class="sxs-lookup"><span data-stu-id="1bb0f-103">secureScore resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bb0f-104">Представляет безопасное значение клиента в день данных оценки на уровне клиента и элемента управления.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="1bb0f-105">По умолчанию данные хранятся в 90 дней.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="1bb0f-106">Эти данные сортируются по **createdDateTime**, от последних к ранним.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="1bb0f-107">Это позволит получать ответы на страницы с помощью $top = n, где n = число дней, которые требуется получить.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="1bb0f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1bb0f-108">Methods</span></span>

| <span data-ttu-id="1bb0f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1bb0f-109">Method</span></span>   | <span data-ttu-id="1bb0f-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1bb0f-110">Return Type</span></span>|<span data-ttu-id="1bb0f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1bb0f-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1bb0f-112">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="1bb0f-112">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="1bb0f-113">Секурескорес</span><span class="sxs-lookup"><span data-stu-id="1bb0f-113">secureScores</span></span>](securescores.md) |<span data-ttu-id="1bb0f-114">Чтение свойств и метаданных объекта Секурескорес.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-114">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="1bb0f-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="1bb0f-115">Properties</span></span>
<span data-ttu-id="1bb0f-116">Тип объекта, содержащий свойства оценки безопасности клиента (ежедневные данные моментального снимка).</span><span class="sxs-lookup"><span data-stu-id="1bb0f-116">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="1bb0f-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bb0f-117">Property</span></span> |<span data-ttu-id="1bb0f-118">Тип</span><span class="sxs-lookup"><span data-stu-id="1bb0f-118">Type</span></span> |<span data-ttu-id="1bb0f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1bb0f-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="1bb0f-120">Азуретенантид</span><span class="sxs-lookup"><span data-stu-id="1bb0f-120">azureTenantId</span></span>   |   <span data-ttu-id="1bb0f-121">String</span><span class="sxs-lookup"><span data-stu-id="1bb0f-121">String</span></span>  |   <span data-ttu-id="1bb0f-122">Строка GUID для идентификатора клиента.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="1bb0f-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1bb0f-123">createdDateTime</span></span> |   <span data-ttu-id="1bb0f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bb0f-124">DateTimeOffset</span></span>  |   <span data-ttu-id="1bb0f-125">Дата создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-125">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="1bb0f-126">id</span><span class="sxs-lookup"><span data-stu-id="1bb0f-126">id</span></span>  |   <span data-ttu-id="1bb0f-127">String</span><span class="sxs-lookup"><span data-stu-id="1bb0f-127">String</span></span>  |   <span data-ttu-id="1bb0f-128">Сочетание Азуретенантид_креатеддатетиме.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-128">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="1bb0f-129">Лиценседусеркаунт</span><span class="sxs-lookup"><span data-stu-id="1bb0f-129">licensedUserCount</span></span>   |   <span data-ttu-id="1bb0f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="1bb0f-130">Int32</span></span>   |   <span data-ttu-id="1bb0f-131">Число лицензированных пользователей для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-131">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="1bb0f-132">Активеусеркаунт</span><span class="sxs-lookup"><span data-stu-id="1bb0f-132">activeUserCount</span></span> |   <span data-ttu-id="1bb0f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1bb0f-133">Int32</span></span>   |   <span data-ttu-id="1bb0f-134">Число активных пользователей для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-134">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="1bb0f-135">Куррентскоре</span><span class="sxs-lookup"><span data-stu-id="1bb0f-135">currentScore</span></span>    |   <span data-ttu-id="1bb0f-136">Двойное</span><span class="sxs-lookup"><span data-stu-id="1bb0f-136">Double</span></span>  |   <span data-ttu-id="1bb0f-137">Текущий полученный рейтинг клиента на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-137">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="1bb0f-138">Максскоре</span><span class="sxs-lookup"><span data-stu-id="1bb0f-138">maxScore</span></span> |  <span data-ttu-id="1bb0f-139">Двойное</span><span class="sxs-lookup"><span data-stu-id="1bb0f-139">Double</span></span>  |   <span data-ttu-id="1bb0f-140">Максимальная возможная Оценка клиента на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-140">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="1bb0f-141">Енабледсервицес</span><span class="sxs-lookup"><span data-stu-id="1bb0f-141">enabledServices</span></span> |   <span data-ttu-id="1bb0f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1bb0f-142">String collection</span></span>   |   <span data-ttu-id="1bb0f-143">Службы, предоставляемые корпорацией Майкрософт для клиента (например, Exchange Online, Skype, SharePoint).</span><span class="sxs-lookup"><span data-stu-id="1bb0f-143">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="1bb0f-144">Аверажекомпаративескорес</span><span class="sxs-lookup"><span data-stu-id="1bb0f-144">averageComparativeScores</span></span> |  <span data-ttu-id="1bb0f-145">Коллекция [аверажекомпаративескоре](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="1bb0f-145">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="1bb0f-146">Средняя оценка по различным областям (например, усреднение по отраслям, среднему на количество участников) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура) в области.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-146">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="1bb0f-147">Контролскорес</span><span class="sxs-lookup"><span data-stu-id="1bb0f-147">controlScores</span></span> | <span data-ttu-id="1bb0f-148">Коллекция [контролскоре](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="1bb0f-148">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="1bb0f-149">Содержит результаты клиентов для набора элементов управления.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-149">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="1bb0f-150">Связи</span><span class="sxs-lookup"><span data-stu-id="1bb0f-150">Relationships</span></span>

<span data-ttu-id="1bb0f-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1bb0f-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1bb0f-152">JSON representation</span></span>

<span data-ttu-id="1bb0f-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bb0f-153">The following is a JSON representation of the resource.</span></span>

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
