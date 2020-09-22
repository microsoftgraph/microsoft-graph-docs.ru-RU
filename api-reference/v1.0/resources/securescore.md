---
title: Тип ресурса Секурескоре
description: Представляет безопасное значение клиента в день данных оценки на уровне клиента и элемента управления.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e4f798ae64b881c95ed4330901c0a34ba4073f0e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984098"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="69c04-103">Тип ресурса Секурескоре</span><span class="sxs-lookup"><span data-stu-id="69c04-103">secureScore resource type</span></span>

<span data-ttu-id="69c04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69c04-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69c04-105">Представляет безопасное значение клиента в день данных оценки на уровне клиента и элемента управления.</span><span class="sxs-lookup"><span data-stu-id="69c04-105">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="69c04-106">По умолчанию данные хранятся в 90 дней.</span><span class="sxs-lookup"><span data-stu-id="69c04-106">By default, 90 days of data is held.</span></span> <span data-ttu-id="69c04-107">Эти данные сортируются по **createdDateTime**, от последних к ранним.</span><span class="sxs-lookup"><span data-stu-id="69c04-107">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="69c04-108">Это позволит получать ответы на страницы с помощью $top = n, где n = число дней, которые требуется получить.</span><span class="sxs-lookup"><span data-stu-id="69c04-108">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="69c04-109">Методы</span><span class="sxs-lookup"><span data-stu-id="69c04-109">Methods</span></span>

| <span data-ttu-id="69c04-110">Метод</span><span class="sxs-lookup"><span data-stu-id="69c04-110">Method</span></span>   | <span data-ttu-id="69c04-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="69c04-111">Return Type</span></span>|<span data-ttu-id="69c04-112">Описание</span><span class="sxs-lookup"><span data-stu-id="69c04-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69c04-113">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="69c04-113">List secureScores</span></span>](../api/security-list-securescores.md) | <span data-ttu-id="69c04-114">Коллекция [секурескорес](securescore.md)</span><span class="sxs-lookup"><span data-stu-id="69c04-114">[secureScores](securescore.md) collection</span></span> |<span data-ttu-id="69c04-115">Получение коллекции объектов Секурескоре.</span><span class="sxs-lookup"><span data-stu-id="69c04-115">Get secureScore object collection.</span></span>|
|[<span data-ttu-id="69c04-116">Получение объектов secureScore</span><span class="sxs-lookup"><span data-stu-id="69c04-116">Get secureScore</span></span>](../api/securescore-get.md) | [<span data-ttu-id="69c04-117">секурескоре</span><span class="sxs-lookup"><span data-stu-id="69c04-117">secureScore</span></span>](securescore.md) |<span data-ttu-id="69c04-118">Чтение свойств и метаданных объекта Секурескоре.</span><span class="sxs-lookup"><span data-stu-id="69c04-118">Read properties and metadata of a secureScore object.</span></span> | 



## <a name="properties"></a><span data-ttu-id="69c04-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="69c04-119">Properties</span></span>

|<span data-ttu-id="69c04-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="69c04-120">Property</span></span> |<span data-ttu-id="69c04-121">Тип</span><span class="sxs-lookup"><span data-stu-id="69c04-121">Type</span></span> |<span data-ttu-id="69c04-122">Описание</span><span class="sxs-lookup"><span data-stu-id="69c04-122">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="69c04-123">id</span><span class="sxs-lookup"><span data-stu-id="69c04-123">id</span></span> |<span data-ttu-id="69c04-124">String</span><span class="sxs-lookup"><span data-stu-id="69c04-124">String</span></span>|<span data-ttu-id="69c04-125">GUID или уникальный идентификатор, созданный поставщиком.</span><span class="sxs-lookup"><span data-stu-id="69c04-125">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="69c04-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69c04-126">Read-only.</span></span> <span data-ttu-id="69c04-127">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="69c04-127">Required.</span></span>|
|   <span data-ttu-id="69c04-128">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="69c04-128">azureTenantId</span></span>   |   <span data-ttu-id="69c04-129">String</span><span class="sxs-lookup"><span data-stu-id="69c04-129">String</span></span>  |   <span data-ttu-id="69c04-130">Строка GUID для идентификатора клиента.</span><span class="sxs-lookup"><span data-stu-id="69c04-130">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="69c04-131">активеусеркаунт</span><span class="sxs-lookup"><span data-stu-id="69c04-131">activeUserCount</span></span> |   <span data-ttu-id="69c04-132">Int32</span><span class="sxs-lookup"><span data-stu-id="69c04-132">Int32</span></span>   |   <span data-ttu-id="69c04-133">Число активных пользователей для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="69c04-133">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="69c04-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69c04-134">createdDateTime</span></span> |   <span data-ttu-id="69c04-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69c04-135">DateTimeOffset</span></span>  |   <span data-ttu-id="69c04-136">Дата создания объекта.</span><span class="sxs-lookup"><span data-stu-id="69c04-136">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="69c04-137">куррентскоре</span><span class="sxs-lookup"><span data-stu-id="69c04-137">currentScore</span></span>    |   <span data-ttu-id="69c04-138">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="69c04-138">Double</span></span>  |   <span data-ttu-id="69c04-139">Текущий полученный рейтинг клиента на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="69c04-139">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="69c04-140">енабледсервицес</span><span class="sxs-lookup"><span data-stu-id="69c04-140">enabledServices</span></span> |   <span data-ttu-id="69c04-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="69c04-141">String collection</span></span>   |   <span data-ttu-id="69c04-142">Службы, предоставляемые корпорацией Майкрософт для клиента (например, Exchange Online, Skype, SharePoint).</span><span class="sxs-lookup"><span data-stu-id="69c04-142">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="69c04-143">лиценседусеркаунт</span><span class="sxs-lookup"><span data-stu-id="69c04-143">licensedUserCount</span></span>   |   <span data-ttu-id="69c04-144">Int32</span><span class="sxs-lookup"><span data-stu-id="69c04-144">Int32</span></span>   |   <span data-ttu-id="69c04-145">Число лицензированных пользователей для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="69c04-145">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="69c04-146">максскоре</span><span class="sxs-lookup"><span data-stu-id="69c04-146">maxScore</span></span> |  <span data-ttu-id="69c04-147">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="69c04-147">Double</span></span>  |   <span data-ttu-id="69c04-148">Максимальная возможная Оценка клиента на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="69c04-148">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="69c04-149">аверажекомпаративескорес</span><span class="sxs-lookup"><span data-stu-id="69c04-149">averageComparativeScores</span></span> |  <span data-ttu-id="69c04-150">Коллекция [аверажекомпаративескоре](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="69c04-150">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="69c04-151">Средняя оценка по различным областям (например, усреднение по отраслям, среднему на количество участников) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура) в области.</span><span class="sxs-lookup"><span data-stu-id="69c04-151">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="69c04-152">контролскорес</span><span class="sxs-lookup"><span data-stu-id="69c04-152">controlScores</span></span> | <span data-ttu-id="69c04-153">Коллекция [контролскоре](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="69c04-153">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="69c04-154">Содержит результаты клиентов для набора элементов управления.</span><span class="sxs-lookup"><span data-stu-id="69c04-154">Contains tenant scores for a set of controls.</span></span>   |
|<span data-ttu-id="69c04-155">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="69c04-155">vendorInformation</span></span> |[<span data-ttu-id="69c04-156">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="69c04-156">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="69c04-157">Сложный тип, содержащий сведения о продукте, поставщике, поставщике и подобеспечении безопасности (например, Vendor = Microsoft; Provider = Секурескоре).</span><span class="sxs-lookup"><span data-stu-id="69c04-157">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="69c04-158">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="69c04-158">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="69c04-159">Связи</span><span class="sxs-lookup"><span data-stu-id="69c04-159">Relationships</span></span>

<span data-ttu-id="69c04-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="69c04-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="69c04-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="69c04-161">JSON representation</span></span>

<span data-ttu-id="69c04-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69c04-162">The following is a JSON representation of the resource.</span></span>

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

