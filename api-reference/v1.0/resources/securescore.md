---
title: Тип ресурса Секурескоре
description: Представляет безопасное значение клиента в день данных оценки на уровне клиента и элемента управления.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 89842579457365f7da10509b2b4ade31f55de4f9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629266"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="f634b-103">Тип ресурса Секурескоре</span><span class="sxs-lookup"><span data-stu-id="f634b-103">secureScore resource type</span></span>

<span data-ttu-id="f634b-104">Представляет безопасное значение клиента в день данных оценки на уровне клиента и элемента управления.</span><span class="sxs-lookup"><span data-stu-id="f634b-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="f634b-105">По умолчанию данные хранятся в 90 дней.</span><span class="sxs-lookup"><span data-stu-id="f634b-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="f634b-106">Эти данные сортируются по **createdDateTime**, от последних к ранним.</span><span class="sxs-lookup"><span data-stu-id="f634b-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="f634b-107">Это позволит получать ответы на страницы с помощью $top = n, где n = число дней, которые требуется получить.</span><span class="sxs-lookup"><span data-stu-id="f634b-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="f634b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f634b-108">Methods</span></span>

| <span data-ttu-id="f634b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f634b-109">Method</span></span>   | <span data-ttu-id="f634b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f634b-110">Return Type</span></span>|<span data-ttu-id="f634b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f634b-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f634b-112">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="f634b-112">List secureScores</span></span>](../api/security-list-securescores.md) | <span data-ttu-id="f634b-113">Коллекция [секурескорес](securescore.md)</span><span class="sxs-lookup"><span data-stu-id="f634b-113">[secureScores](securescore.md) collection</span></span> |<span data-ttu-id="f634b-114">Получение коллекции объектов Секурескоре.</span><span class="sxs-lookup"><span data-stu-id="f634b-114">Get secureScore object collection.</span></span>|
|[<span data-ttu-id="f634b-115">Получение Секурескоре</span><span class="sxs-lookup"><span data-stu-id="f634b-115">Get secureScore</span></span>](../api/securescore-get.md) | [<span data-ttu-id="f634b-116">Секурескоре</span><span class="sxs-lookup"><span data-stu-id="f634b-116">secureScore</span></span>](securescore.md) |<span data-ttu-id="f634b-117">Чтение свойств и метаданных объекта Секурескоре.</span><span class="sxs-lookup"><span data-stu-id="f634b-117">Read properties and metadata of a secureScore object.</span></span> | 



## <a name="properties"></a><span data-ttu-id="f634b-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="f634b-118">Properties</span></span>

|<span data-ttu-id="f634b-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="f634b-119">Property</span></span> |<span data-ttu-id="f634b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f634b-120">Type</span></span> |<span data-ttu-id="f634b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f634b-121">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="f634b-122">id</span><span class="sxs-lookup"><span data-stu-id="f634b-122">id</span></span> |<span data-ttu-id="f634b-123">String</span><span class="sxs-lookup"><span data-stu-id="f634b-123">String</span></span>|<span data-ttu-id="f634b-124">GUID или уникальный идентификатор, созданный поставщиком.</span><span class="sxs-lookup"><span data-stu-id="f634b-124">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="f634b-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f634b-125">Read-only.</span></span> <span data-ttu-id="f634b-126">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="f634b-126">Required.</span></span>|
|   <span data-ttu-id="f634b-127">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="f634b-127">azureTenantId</span></span>   |   <span data-ttu-id="f634b-128">String</span><span class="sxs-lookup"><span data-stu-id="f634b-128">String</span></span>  |   <span data-ttu-id="f634b-129">Строка GUID для идентификатора клиента.</span><span class="sxs-lookup"><span data-stu-id="f634b-129">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="f634b-130">Активеусеркаунт</span><span class="sxs-lookup"><span data-stu-id="f634b-130">activeUserCount</span></span> |   <span data-ttu-id="f634b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f634b-131">Int32</span></span>   |   <span data-ttu-id="f634b-132">Число активных пользователей для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="f634b-132">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="f634b-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f634b-133">createdDateTime</span></span> |   <span data-ttu-id="f634b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f634b-134">DateTimeOffset</span></span>  |   <span data-ttu-id="f634b-135">Дата создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f634b-135">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="f634b-136">Куррентскоре</span><span class="sxs-lookup"><span data-stu-id="f634b-136">currentScore</span></span>    |   <span data-ttu-id="f634b-137">Двойное</span><span class="sxs-lookup"><span data-stu-id="f634b-137">Double</span></span>  |   <span data-ttu-id="f634b-138">Текущий полученный рейтинг клиента на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="f634b-138">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="f634b-139">Енабледсервицес</span><span class="sxs-lookup"><span data-stu-id="f634b-139">enabledServices</span></span> |   <span data-ttu-id="f634b-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f634b-140">String collection</span></span>   |   <span data-ttu-id="f634b-141">Службы, предоставляемые корпорацией Майкрософт для клиента (например, Exchange Online, Skype, SharePoint).</span><span class="sxs-lookup"><span data-stu-id="f634b-141">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="f634b-142">Лиценседусеркаунт</span><span class="sxs-lookup"><span data-stu-id="f634b-142">licensedUserCount</span></span>   |   <span data-ttu-id="f634b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f634b-143">Int32</span></span>   |   <span data-ttu-id="f634b-144">Число лицензированных пользователей для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="f634b-144">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="f634b-145">Максскоре</span><span class="sxs-lookup"><span data-stu-id="f634b-145">maxScore</span></span> |  <span data-ttu-id="f634b-146">Двойное</span><span class="sxs-lookup"><span data-stu-id="f634b-146">Double</span></span>  |   <span data-ttu-id="f634b-147">Максимальная возможная Оценка клиента на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="f634b-147">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="f634b-148">Аверажекомпаративескорес</span><span class="sxs-lookup"><span data-stu-id="f634b-148">averageComparativeScores</span></span> |  <span data-ttu-id="f634b-149">Коллекция [аверажекомпаративескоре](averagecomparativescore.md)</span><span class="sxs-lookup"><span data-stu-id="f634b-149">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="f634b-150">Средняя оценка по различным областям (например, усреднение по отраслям, среднему на количество участников) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура) в области.</span><span class="sxs-lookup"><span data-stu-id="f634b-150">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="f634b-151">Контролскорес</span><span class="sxs-lookup"><span data-stu-id="f634b-151">controlScores</span></span> | <span data-ttu-id="f634b-152">Коллекция [контролскоре](controlscore.md)</span><span class="sxs-lookup"><span data-stu-id="f634b-152">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="f634b-153">Содержит результаты клиентов для набора элементов управления.</span><span class="sxs-lookup"><span data-stu-id="f634b-153">Contains tenant scores for a set of controls.</span></span>   |
|<span data-ttu-id="f634b-154">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="f634b-154">vendorInformation</span></span> |[<span data-ttu-id="f634b-155">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="f634b-155">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="f634b-156">Сложный тип, содержащий сведения о продукте, поставщике, поставщике и подобеспечении безопасности (например, Vendor = Microsoft; Provider = Секурескоре).</span><span class="sxs-lookup"><span data-stu-id="f634b-156">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="f634b-157">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f634b-157">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f634b-158">Связи</span><span class="sxs-lookup"><span data-stu-id="f634b-158">Relationships</span></span>

<span data-ttu-id="f634b-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f634b-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f634b-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f634b-160">JSON representation</span></span>

<span data-ttu-id="f634b-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f634b-161">The following is a JSON representation of the resource.</span></span>

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
