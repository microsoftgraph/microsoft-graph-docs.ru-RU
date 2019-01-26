---
title: Тип ресурса secureScores
description: 'в начало = n, где n — число дней данных, которую необходимо получить. '
localization_priority: Normal
ms.openlocfilehash: fef5c43130aecf1604677d07f785a0cee0539568
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576082"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="df8d7-103">Тип ресурса secureScores</span><span class="sxs-lookup"><span data-stu-id="df8d7-103">secureScores resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df8d7-104">Представляет безопасной счета клиента в день для оценки данных, на уровне клиента и элемента управления.</span><span class="sxs-lookup"><span data-stu-id="df8d7-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="df8d7-105">По умолчанию проводится данных в течение 90 дней.</span><span class="sxs-lookup"><span data-stu-id="df8d7-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="df8d7-106">Эти данные сортируются по **createdDateTime**от поздних к ранним.</span><span class="sxs-lookup"><span data-stu-id="df8d7-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="df8d7-107">Это позволит вам для запросов с помощью $top = n, где n — число дней данных, которую необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="df8d7-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="df8d7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="df8d7-108">Methods</span></span>

| <span data-ttu-id="df8d7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="df8d7-109">Method</span></span>   | <span data-ttu-id="df8d7-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="df8d7-110">Return Type</span></span>|<span data-ttu-id="df8d7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="df8d7-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="df8d7-112">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="df8d7-112">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="df8d7-113">secureScores</span><span class="sxs-lookup"><span data-stu-id="df8d7-113">secureScores</span></span>](securescores.md) |<span data-ttu-id="df8d7-114">Чтение свойства и метаданные объекта secureScores.</span><span class="sxs-lookup"><span data-stu-id="df8d7-114">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="df8d7-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="df8d7-115">Properties</span></span>
<span data-ttu-id="df8d7-116">Свойства содержащий тип сущности безопасности клиента широкополосном (ежедневного моментальный снимок данных).</span><span class="sxs-lookup"><span data-stu-id="df8d7-116">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="df8d7-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="df8d7-117">Property</span></span> |<span data-ttu-id="df8d7-118">Тип</span><span class="sxs-lookup"><span data-stu-id="df8d7-118">Type</span></span> |<span data-ttu-id="df8d7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="df8d7-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="df8d7-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="df8d7-120">azureTenantId</span></span>   |   <span data-ttu-id="df8d7-121">Строка</span><span class="sxs-lookup"><span data-stu-id="df8d7-121">String</span></span>  |   <span data-ttu-id="df8d7-122">Идентификатор GUID строки для клиента.</span><span class="sxs-lookup"><span data-stu-id="df8d7-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="df8d7-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df8d7-123">createdDateTime</span></span> |   <span data-ttu-id="df8d7-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df8d7-124">DateTimeOffset</span></span>  |   <span data-ttu-id="df8d7-125">Дата создания объекта.</span><span class="sxs-lookup"><span data-stu-id="df8d7-125">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="df8d7-126">id</span><span class="sxs-lookup"><span data-stu-id="df8d7-126">id</span></span>  |   <span data-ttu-id="df8d7-127">Строка</span><span class="sxs-lookup"><span data-stu-id="df8d7-127">String</span></span>  |   <span data-ttu-id="df8d7-128">Сочетание azureTenantId_createdDateTime.</span><span class="sxs-lookup"><span data-stu-id="df8d7-128">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="df8d7-129">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="df8d7-129">licensedUserCount</span></span>   |   <span data-ttu-id="df8d7-130">Int32</span><span class="sxs-lookup"><span data-stu-id="df8d7-130">Int32</span></span>   |   <span data-ttu-id="df8d7-131">Число пользователей данного клиента с корпоративным лицензированием.</span><span class="sxs-lookup"><span data-stu-id="df8d7-131">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="df8d7-132">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="df8d7-132">activeUserCount</span></span> |   <span data-ttu-id="df8d7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="df8d7-133">Int32</span></span>   |   <span data-ttu-id="df8d7-134">Число активных пользователей указанного клиента.</span><span class="sxs-lookup"><span data-stu-id="df8d7-134">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="df8d7-135">currentScore</span><span class="sxs-lookup"><span data-stu-id="df8d7-135">currentScore</span></span>    |   <span data-ttu-id="df8d7-136">Double</span><span class="sxs-lookup"><span data-stu-id="df8d7-136">Double</span></span>  |   <span data-ttu-id="df8d7-137">Оценка текущего обновления клиента на указанной даты.</span><span class="sxs-lookup"><span data-stu-id="df8d7-137">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="df8d7-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="df8d7-138">maxScore</span></span> |  <span data-ttu-id="df8d7-139">Double</span><span class="sxs-lookup"><span data-stu-id="df8d7-139">Double</span></span>  |   <span data-ttu-id="df8d7-140">Клиент максимальное возможному значению на указанной даты.</span><span class="sxs-lookup"><span data-stu-id="df8d7-140">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="df8d7-141">enabledServices</span><span class="sxs-lookup"><span data-stu-id="df8d7-141">enabledServices</span></span> |   <span data-ttu-id="df8d7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="df8d7-142">String collection</span></span>   |   <span data-ttu-id="df8d7-143">Службы Майкрософт для клиента (например, Exchange online, Скайп, Sharepoint).</span><span class="sxs-lookup"><span data-stu-id="df8d7-143">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="df8d7-144">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="df8d7-144">averageComparativeScores</span></span> |  <span data-ttu-id="df8d7-145">[averageComparativeScore](averagecomparativescore.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="df8d7-145">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="df8d7-146">Средняя оценка по различные области (например, среднее число разных отраслей, среднее, число) и элемент управления категории (удостоверения, данные, устройства, приложения, инфраструктуры) в области действия.</span><span class="sxs-lookup"><span data-stu-id="df8d7-146">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="df8d7-147">controlScores</span><span class="sxs-lookup"><span data-stu-id="df8d7-147">controlScores</span></span> | <span data-ttu-id="df8d7-148">[controlScore](controlscore.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="df8d7-148">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="df8d7-149">Содержит показателям клиента для набора элементов управления.</span><span class="sxs-lookup"><span data-stu-id="df8d7-149">Contains tenant scores for a set of controls.</span></span>   |
|   <span data-ttu-id="df8d7-150">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="df8d7-150">vendorInformation</span></span> | [<span data-ttu-id="df8d7-151">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="df8d7-151">securityVendorInformation</span></span>](securityvendorinformation.md) | <span data-ttu-id="df8d7-152">Содержит сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = корпорации Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="df8d7-152">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="df8d7-153">Связи</span><span class="sxs-lookup"><span data-stu-id="df8d7-153">Relationships</span></span>

<span data-ttu-id="df8d7-154">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="df8d7-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="df8d7-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="df8d7-155">JSON representation</span></span>

<span data-ttu-id="df8d7-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df8d7-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
}-->

```json
{
    "id": "String",
    "azureTenantId": "String (identifier)",
    "createdDateTime": "DateTimeOffset",
    "licensedUserCount": "Int32",
    "activeUserCount": "Int32",
    "currentScore": "Double",
    "maxScore": "Double",    
    "enabledServices": ["String"],
    "averageComparativeScores": [{ "@odata.type":"microsoft.graph.averageComparativeScores"}],
    "controlScores": [{"@odata.type":"microsoft.graph.controlScores"}],
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
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
