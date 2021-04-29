---
title: тип ресурса noncustodialDataSource
description: Неконтлиционные источники данных позволяют добавлять данные в дело, не связывая их с хранителями
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 1e7dd0d656a58e65e460742158cdcc70da1f1d5a
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080908"
---
# <a name="noncustodialdatasource-resource-type"></a><span data-ttu-id="2680f-103">тип ресурса noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="2680f-103">noncustodialDataSource resource type</span></span>

<span data-ttu-id="2680f-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="2680f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2680f-105">Источники данных, не имеющие содержания под стражей, могут добавлять данные в дело, не связывая их с хранителями.</span><span class="sxs-lookup"><span data-stu-id="2680f-105">Non-custodial data sources let you add data to a case without having to associate it to a custodian.</span></span> <span data-ttu-id="2680f-106">Дополнительные сведения можно получить на [сайте Add non-custodial data sources to an Advanced eDiscovery case](https://docs.microsoft.com/microsoft-365/compliance/non-custodial-data-sources)</span><span class="sxs-lookup"><span data-stu-id="2680f-106">To learn more, visit [Add non-custodial data sources to an Advanced eDiscovery case ](https://docs.microsoft.com/microsoft-365/compliance/non-custodial-data-sources)</span></span>

<span data-ttu-id="2680f-107">Наследует [от dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span><span class="sxs-lookup"><span data-stu-id="2680f-107">Inherits from [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2680f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="2680f-108">Methods</span></span>

|<span data-ttu-id="2680f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="2680f-109">Method</span></span>|<span data-ttu-id="2680f-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="2680f-110">Return type</span></span>|<span data-ttu-id="2680f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2680f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2680f-112">Список noncustodialDataSources</span><span class="sxs-lookup"><span data-stu-id="2680f-112">List noncustodialDataSources</span></span>](../api/ediscovery-noncustodialdatasource-list.md)|<span data-ttu-id="2680f-113">[коллекция microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="2680f-113">[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) collection</span></span>|<span data-ttu-id="2680f-114">Получите список объектов [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="2680f-114">Get a list of the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) objects and their properties.</span></span>|
|[<span data-ttu-id="2680f-115">Получить noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="2680f-115">Get noncustodialDataSource</span></span>](../api/ediscovery-noncustodialdatasource-get.md)|[<span data-ttu-id="2680f-116">microsoft.graph.ediscovery.noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="2680f-116">microsoft.graph.ediscovery.noncustodialDataSource</span></span>](../resources/ediscovery-noncustodialdatasource.md)|<span data-ttu-id="2680f-117">Ознакомьтесь с свойствами и отношениями [объекта noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="2680f-117">Read the properties and relationships of a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>|
|[<span data-ttu-id="2680f-118">Release dataSource</span><span class="sxs-lookup"><span data-stu-id="2680f-118">Release dataSource</span></span>](../api/ediscovery-noncustodialdatasource-release.md)|<span data-ttu-id="2680f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="2680f-119">None</span></span>|<span data-ttu-id="2680f-120">Освобождает источник данных, не относясь к данным, не относяся к опеке.</span><span class="sxs-lookup"><span data-stu-id="2680f-120">Releases a non-custodial data source.</span></span>|
|[<span data-ttu-id="2680f-121">List dataSource</span><span class="sxs-lookup"><span data-stu-id="2680f-121">List dataSource</span></span>](../api/ediscovery-noncustodialdatasource-list-datasource.md)|<span data-ttu-id="2680f-122">[коллекция microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="2680f-122">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection</span></span>|<span data-ttu-id="2680f-123">Получите ресурсы dataSource из свойства навигации dataSource.</span><span class="sxs-lookup"><span data-stu-id="2680f-123">Get the dataSource resources from the dataSource navigation property.</span></span>|
|[<span data-ttu-id="2680f-124">Создание dataSource</span><span class="sxs-lookup"><span data-stu-id="2680f-124">Create dataSource</span></span>](../api/ediscovery-noncustodialdatasource-post.md)|[<span data-ttu-id="2680f-125">microsoft.graph.ediscovery.dataSource</span><span class="sxs-lookup"><span data-stu-id="2680f-125">microsoft.graph.ediscovery.dataSource</span></span>](../resources/ediscovery-datasource.md)|<span data-ttu-id="2680f-126">Создание нового объекта dataSource.</span><span class="sxs-lookup"><span data-stu-id="2680f-126">Create a new dataSource object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2680f-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="2680f-127">Properties</span></span>

|<span data-ttu-id="2680f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2680f-128">Property</span></span>|<span data-ttu-id="2680f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2680f-129">Type</span></span>|<span data-ttu-id="2680f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2680f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2680f-131">applyHoldToSource</span><span class="sxs-lookup"><span data-stu-id="2680f-131">applyHoldToSource</span></span>|<span data-ttu-id="2680f-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="2680f-132">Boolean</span></span>|<span data-ttu-id="2680f-133">Указывает, применяется ли удержание к источнику данных без хранения (например, к почтовому ящику или сайту).</span><span class="sxs-lookup"><span data-stu-id="2680f-133">Indicates if hold is applied to non-custodial data source (such as mailbox or site).</span></span>|
|<span data-ttu-id="2680f-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2680f-134">createdDateTime</span></span>|<span data-ttu-id="2680f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2680f-135">DateTimeOffset</span></span>|<span data-ttu-id="2680f-136">Создана дата и время nonCustodialDataSource.</span><span class="sxs-lookup"><span data-stu-id="2680f-136">Created date and time of the nonCustodialDataSource.</span></span> <span data-ttu-id="2680f-137">Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span><span class="sxs-lookup"><span data-stu-id="2680f-137">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>|
|<span data-ttu-id="2680f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="2680f-138">displayName</span></span>|<span data-ttu-id="2680f-139">String</span><span class="sxs-lookup"><span data-stu-id="2680f-139">String</span></span>|<span data-ttu-id="2680f-140">Отображение имени noncustodialDataSource.</span><span class="sxs-lookup"><span data-stu-id="2680f-140">Display name of the noncustodialDataSource.</span></span> <span data-ttu-id="2680f-141">Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span><span class="sxs-lookup"><span data-stu-id="2680f-141">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>|
|<span data-ttu-id="2680f-142">id</span><span class="sxs-lookup"><span data-stu-id="2680f-142">id</span></span>|<span data-ttu-id="2680f-143">String</span><span class="sxs-lookup"><span data-stu-id="2680f-143">String</span></span>|<span data-ttu-id="2680f-144">Уникальный идентификатор nonCustodialDataSource.</span><span class="sxs-lookup"><span data-stu-id="2680f-144">Unique identifier of the nonCustodialDataSource.</span></span> <span data-ttu-id="2680f-145">Наследуется от [сущности](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="2680f-145">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="2680f-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2680f-146">lastModifiedDateTime</span></span>|<span data-ttu-id="2680f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2680f-147">DateTimeOffset</span></span>|<span data-ttu-id="2680f-148">Последняя измененная дата и время nonCustodialDataSource.</span><span class="sxs-lookup"><span data-stu-id="2680f-148">Last modified date and time of the nonCustodialDataSource.</span></span> <span data-ttu-id="2680f-149">Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span><span class="sxs-lookup"><span data-stu-id="2680f-149">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>|
|<span data-ttu-id="2680f-150">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="2680f-150">releasedDateTime</span></span>|<span data-ttu-id="2680f-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2680f-151">DateTimeOffset</span></span>|<span data-ttu-id="2680f-152">Дата и время освобождения nonCustodialDataSource из дела.</span><span class="sxs-lookup"><span data-stu-id="2680f-152">Date and time that the nonCustodialDataSource was released from the case.</span></span> <span data-ttu-id="2680f-153">Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span><span class="sxs-lookup"><span data-stu-id="2680f-153">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span>|
|<span data-ttu-id="2680f-154">status</span><span class="sxs-lookup"><span data-stu-id="2680f-154">status</span></span>|<span data-ttu-id="2680f-155">microsoft.graph.ediscovery.dataSourceContainerStatus</span><span class="sxs-lookup"><span data-stu-id="2680f-155">microsoft.graph.ediscovery.dataSourceContainerStatus</span></span>|<span data-ttu-id="2680f-156">Последний статус nonCustodialDataSource.</span><span class="sxs-lookup"><span data-stu-id="2680f-156">Latest status of the nonCustodialDataSource.</span></span> <span data-ttu-id="2680f-157">Наследуется [от microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span><span class="sxs-lookup"><span data-stu-id="2680f-157">Inherited from [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md).</span></span> <span data-ttu-id="2680f-158">Возможные значения: `Active`, `Released`.</span><span class="sxs-lookup"><span data-stu-id="2680f-158">Possible values are: `Active`, `Released`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2680f-159">Связи</span><span class="sxs-lookup"><span data-stu-id="2680f-159">Relationships</span></span>

|<span data-ttu-id="2680f-160">Связь</span><span class="sxs-lookup"><span data-stu-id="2680f-160">Relationship</span></span>|<span data-ttu-id="2680f-161">Тип</span><span class="sxs-lookup"><span data-stu-id="2680f-161">Type</span></span>|<span data-ttu-id="2680f-162">Описание</span><span class="sxs-lookup"><span data-stu-id="2680f-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2680f-163">dataSource</span><span class="sxs-lookup"><span data-stu-id="2680f-163">dataSource</span></span>|[<span data-ttu-id="2680f-164">microsoft.graph.ediscovery.dataSource</span><span class="sxs-lookup"><span data-stu-id="2680f-164">microsoft.graph.ediscovery.dataSource</span></span>](../resources/ediscovery-datasource.md)|<span data-ttu-id="2680f-165">Источник данных пользователя или SharePoint в качестве источника данных, не в качестве источника данных, не в виде хранения.</span><span class="sxs-lookup"><span data-stu-id="2680f-165">User source or SharePoint site data source as non-custodial data source.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2680f-166">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2680f-166">JSON representation</span></span>

<span data-ttu-id="2680f-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2680f-167">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource",
  "baseType": "microsoft.graph.ediscovery.dataSourceContainer",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.noncustodialDataSource",
  "id": "String (identifier)",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "applyHoldToSource": "Boolean"
}
```
