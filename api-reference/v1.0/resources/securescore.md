---
title: Тип ресурса Секурескоре
description: Представляет безопасное значение клиента в день данных оценки на уровне клиента и элемента управления.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 395c5ed0594d1f509bb664b5aee6ea18bb42af0a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034484"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="91bd6-103">Тип ресурса Секурескоре</span><span class="sxs-lookup"><span data-stu-id="91bd6-103">secureScore resource type</span></span>

<span data-ttu-id="91bd6-104">Представляет безопасное значение клиента в день данных оценки на уровне клиента и элемента управления.</span><span class="sxs-lookup"><span data-stu-id="91bd6-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="91bd6-105">По умолчанию данные хранятся в 90 дней.</span><span class="sxs-lookup"><span data-stu-id="91bd6-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="91bd6-106">Эти данные сортируются по **createdDateTime**, от последних к ранним.</span><span class="sxs-lookup"><span data-stu-id="91bd6-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="91bd6-107">Это позволит получать ответы на страницы с помощью $top = n, где n = число дней, которые требуется получить.</span><span class="sxs-lookup"><span data-stu-id="91bd6-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="91bd6-108">Методы</span><span class="sxs-lookup"><span data-stu-id="91bd6-108">Methods</span></span>

| <span data-ttu-id="91bd6-109">Метод</span><span class="sxs-lookup"><span data-stu-id="91bd6-109">Method</span></span>   | <span data-ttu-id="91bd6-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="91bd6-110">Return Type</span></span>|<span data-ttu-id="91bd6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="91bd6-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="91bd6-112">Список объектов secureScore</span><span class="sxs-lookup"><span data-stu-id="91bd6-112">List secureScores</span></span>](../api/security-list-securescores.md) | <span data-ttu-id="91bd6-113">Коллекция [секурескорес](securescore.md)</span><span class="sxs-lookup"><span data-stu-id="91bd6-113">[secureScores](securescore.md) collection</span></span> |<span data-ttu-id="91bd6-114">Получение коллекции объектов Секурескоре.</span><span class="sxs-lookup"><span data-stu-id="91bd6-114">Get secureScore object collection.</span></span>|
|[<span data-ttu-id="91bd6-115">Получение объектов secureScore</span><span class="sxs-lookup"><span data-stu-id="91bd6-115">Get secureScore</span></span>](../api/securescore-get.md) | [<span data-ttu-id="91bd6-116">Секурескоре</span><span class="sxs-lookup"><span data-stu-id="91bd6-116">secureScore</span></span>](securescore.md) |<span data-ttu-id="91bd6-117">Чтение свойств и метаданных объекта Секурескоре.</span><span class="sxs-lookup"><span data-stu-id="91bd6-117">Read properties and metadata of a secureScore object.</span></span> | 



## <a name="properties"></a><span data-ttu-id="91bd6-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="91bd6-118">Properties</span></span>

|<span data-ttu-id="91bd6-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="91bd6-119">Property</span></span> |<span data-ttu-id="91bd6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="91bd6-120">Type</span></span> |<span data-ttu-id="91bd6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="91bd6-121">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="91bd6-122">id</span><span class="sxs-lookup"><span data-stu-id="91bd6-122">id</span></span> |<span data-ttu-id="91bd6-123">String</span><span class="sxs-lookup"><span data-stu-id="91bd6-123">String</span></span>|<span data-ttu-id="91bd6-124">GUID или уникальный идентификатор, созданный поставщиком.</span><span class="sxs-lookup"><span data-stu-id="91bd6-124">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="91bd6-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="91bd6-125">Read-only.</span></span> <span data-ttu-id="91bd6-126">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="91bd6-126">Required.</span></span>|
|   <span data-ttu-id="91bd6-127">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="91bd6-127">azureTenantId</span></span>   |   <span data-ttu-id="91bd6-128">String</span><span class="sxs-lookup"><span data-stu-id="91bd6-128">String</span></span>  |   <span data-ttu-id="91bd6-129">Строка GUID для идентификатора клиента.</span><span class="sxs-lookup"><span data-stu-id="91bd6-129">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="91bd6-130">Активеусеркаунт</span><span class="sxs-lookup"><span data-stu-id="91bd6-130">activeUserCount</span></span> |   <span data-ttu-id="91bd6-131">Int32</span><span class="sxs-lookup"><span data-stu-id="91bd6-131">Int32</span></span>   |   <span data-ttu-id="91bd6-132">Число активных пользователей для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="91bd6-132">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="91bd6-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91bd6-133">createdDateTime</span></span> |   <span data-ttu-id="91bd6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91bd6-134">DateTimeOffset</span></span>  |   <span data-ttu-id="91bd6-135">Дата создания объекта.</span><span class="sxs-lookup"><span data-stu-id="91bd6-135">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="91bd6-136">Куррентскоре</span><span class="sxs-lookup"><span data-stu-id="91bd6-136">currentScore</span></span>    |   <span data-ttu-id="91bd6-137">Двойное</span><span class="sxs-lookup"><span data-stu-id="91bd6-137">Double</span></span>  |   <span data-ttu-id="91bd6-138">Текущий полученный рейтинг клиента на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="91bd6-138">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="91bd6-139">Енабледсервицес</span><span class="sxs-lookup"><span data-stu-id="91bd6-139">enabledServices</span></span> |   <span data-ttu-id="91bd6-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="91bd6-140">String collection</span></span>   |   <span data-ttu-id="91bd6-141">Службы, предоставляемые корпорацией Майкрософт для клиента (например, Exchange Online, Skype, SharePoint).</span><span class="sxs-lookup"><span data-stu-id="91bd6-141">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="91bd6-142">Лиценседусеркаунт</span><span class="sxs-lookup"><span data-stu-id="91bd6-142">licensedUserCount</span></span>   |   <span data-ttu-id="91bd6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="91bd6-143">Int32</span></span>   |   <span data-ttu-id="91bd6-144">Число лицензированных пользователей для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="91bd6-144">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="91bd6-145">Максскоре</span><span class="sxs-lookup"><span data-stu-id="91bd6-145">maxScore</span></span> |  <span data-ttu-id="91bd6-146">Двойное</span><span class="sxs-lookup"><span data-stu-id="91bd6-146">Double</span></span>  |   <span data-ttu-id="91bd6-147">Максимальная возможная Оценка клиента на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="91bd6-147">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="91bd6-148">Аверажекомпаративескорес</span><span class="sxs-lookup"><span data-stu-id="91bd6-148">averageComparativeScores</span></span> |  <span data-ttu-id="91bd6-149">Коллекция [аверажекомпаративескоре](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="91bd6-149">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="91bd6-150">Средняя оценка по различным областям (например, усреднение по отраслям, среднему на количество участников) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура) в области.</span><span class="sxs-lookup"><span data-stu-id="91bd6-150">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="91bd6-151">Контролскорес</span><span class="sxs-lookup"><span data-stu-id="91bd6-151">controlScores</span></span> | <span data-ttu-id="91bd6-152">Коллекция [контролскоре](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="91bd6-152">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="91bd6-153">Содержит результаты клиентов для набора элементов управления.</span><span class="sxs-lookup"><span data-stu-id="91bd6-153">Contains tenant scores for a set of controls.</span></span>   |
|<span data-ttu-id="91bd6-154">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="91bd6-154">vendorInformation</span></span> |[<span data-ttu-id="91bd6-155">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="91bd6-155">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="91bd6-156">Сложный тип, содержащий сведения о продукте, поставщике, поставщике и подобеспечении безопасности (например, Vendor = Microsoft; Provider = Секурескоре).</span><span class="sxs-lookup"><span data-stu-id="91bd6-156">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="91bd6-157">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="91bd6-157">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="91bd6-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="91bd6-158">Relationships</span></span>

<span data-ttu-id="91bd6-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="91bd6-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="91bd6-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="91bd6-160">JSON representation</span></span>

<span data-ttu-id="91bd6-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91bd6-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
}-->

```json
{
"id": "String (identifier)",
"azureTenantId": "String",
"activeUserCount": "Int32",
"createdDateTime": "String (timestamp)",
"currentScore": "Double",
"enabledServices": ["String"],
"licensedUserCount": "Int32",
"maxScore": "Double",
"averageComparativeScores": [{"@odata.type": "microsoft.graph.averageComparativeScore"}],
"controlScores": [{"@odata.type": "microsoft.graph.controlScore"}],
"vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
