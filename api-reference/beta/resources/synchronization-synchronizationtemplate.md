---
title: Тип ресурса synchronizationTemplate
description: Предоставляет предварительно настроенные параметры синхронизации для конкретного приложения.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c08f5c3eee6225a1149ff993415f83b2e5916583
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132309"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="ac733-103">Тип ресурса synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="ac733-103">synchronizationTemplate resource type</span></span>

<span data-ttu-id="ac733-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac733-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac733-105">Предоставляет предварительно настроенные параметры синхронизации для конкретного приложения.</span><span class="sxs-lookup"><span data-stu-id="ac733-105">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="ac733-106">Эти параметры будут использоваться по умолчанию для [любого](synchronization-synchronizationjob.md) задания синхронизации, основанного на шаблоне.</span><span class="sxs-lookup"><span data-stu-id="ac733-106">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="ac733-107">Разработчик приложения определяет шаблон; Любой может получить шаблон, чтобы увидеть параметры по умолчанию, включая схему [синхронизации.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="ac733-107">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="ac733-108">Для приложения можно предоставить несколько шаблонов и назначить шаблон по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ac733-108">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="ac733-109">Если для интересуемого приложения доступно несколько шаблонов, обратитесь к конкретным приложениям, чтобы определить, какой из них лучше всего соответствует вашим потребностям.</span><span class="sxs-lookup"><span data-stu-id="ac733-109">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="ac733-110">Методы</span><span class="sxs-lookup"><span data-stu-id="ac733-110">Methods</span></span>

| <span data-ttu-id="ac733-111">Метод</span><span class="sxs-lookup"><span data-stu-id="ac733-111">Method</span></span>        | <span data-ttu-id="ac733-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ac733-112">Return Type</span></span>               | <span data-ttu-id="ac733-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ac733-113">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="ac733-114">Список</span><span class="sxs-lookup"><span data-stu-id="ac733-114">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="ac733-115">[Коллекция synchronizationTemplate](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="ac733-115">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="ac733-116">Список шаблонов, доступных для экземпляра приложения или приложения (участников-служб).</span><span class="sxs-lookup"><span data-stu-id="ac733-116">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="ac733-117">Get</span><span class="sxs-lookup"><span data-stu-id="ac733-117">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="ac733-118">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="ac733-118">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="ac733-119">Чтение свойств и связей объекта **synchronizationTemplate.**</span><span class="sxs-lookup"><span data-stu-id="ac733-119">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="ac733-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac733-120">Properties</span></span>

| <span data-ttu-id="ac733-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac733-121">Property</span></span>      | <span data-ttu-id="ac733-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ac733-122">Type</span></span>                      | <span data-ttu-id="ac733-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ac733-123">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="ac733-124">id</span><span class="sxs-lookup"><span data-stu-id="ac733-124">id</span></span>             |<span data-ttu-id="ac733-125">Строка</span><span class="sxs-lookup"><span data-stu-id="ac733-125">String</span></span>                     |<span data-ttu-id="ac733-126">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="ac733-126">Unique template identifier.</span></span>|
|<span data-ttu-id="ac733-127">applicationId</span><span class="sxs-lookup"><span data-stu-id="ac733-127">applicationId</span></span>  |<span data-ttu-id="ac733-128">String</span><span class="sxs-lookup"><span data-stu-id="ac733-128">String</span></span>                     |<span data-ttu-id="ac733-129">Идентификатор приложения, к которой принадлежит этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="ac733-129">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="ac733-130">default</span><span class="sxs-lookup"><span data-stu-id="ac733-130">default</span></span>        |<span data-ttu-id="ac733-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac733-131">Boolean</span></span>                    |<span data-ttu-id="ac733-132">`true` если этот шаблон рекомендуется использовать по умолчанию для приложения.</span><span class="sxs-lookup"><span data-stu-id="ac733-132">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="ac733-133">description</span><span class="sxs-lookup"><span data-stu-id="ac733-133">description</span></span>    |<span data-ttu-id="ac733-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ac733-134">String</span></span>                     |<span data-ttu-id="ac733-135">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="ac733-135">Description of the template.</span></span>|
|<span data-ttu-id="ac733-136">обнаруживаемый</span><span class="sxs-lookup"><span data-stu-id="ac733-136">discoverable</span></span>   |<span data-ttu-id="ac733-137">Строка</span><span class="sxs-lookup"><span data-stu-id="ac733-137">String</span></span>                     |<span data-ttu-id="ac733-138">`true` если этот шаблон должен отображаться в коллекции шаблонов, доступных для экземпляра приложения (основного приложения-службы).</span><span class="sxs-lookup"><span data-stu-id="ac733-138">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="ac733-139">factoryTag</span><span class="sxs-lookup"><span data-stu-id="ac733-139">factoryTag</span></span>     |<span data-ttu-id="ac733-140">Строка</span><span class="sxs-lookup"><span data-stu-id="ac733-140">String</span></span>                     |<span data-ttu-id="ac733-141">Один из известных заводских тегов, поддерживаемых механизмом синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ac733-141">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="ac733-142">FactoryTag **сообщает** механизму синхронизации, какую реализацию использовать при обработке заданий на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="ac733-142">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="ac733-143">метаданные</span><span class="sxs-lookup"><span data-stu-id="ac733-143">metadata</span></span>       |<span data-ttu-id="ac733-144">Коллекция metadataEntry</span><span class="sxs-lookup"><span data-stu-id="ac733-144">metadataEntry collection</span></span>   |<span data-ttu-id="ac733-145">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="ac733-145">Additional extension properties.</span></span> <span data-ttu-id="ac733-146">Если не было явно упомянуто, значения метаданных не следует менять.</span><span class="sxs-lookup"><span data-stu-id="ac733-146">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac733-147">Связи</span><span class="sxs-lookup"><span data-stu-id="ac733-147">Relationships</span></span>
| <span data-ttu-id="ac733-148">Связь</span><span class="sxs-lookup"><span data-stu-id="ac733-148">Relationship</span></span>      | <span data-ttu-id="ac733-149">Тип</span><span class="sxs-lookup"><span data-stu-id="ac733-149">Type</span></span>      |<span data-ttu-id="ac733-150">Описание</span><span class="sxs-lookup"><span data-stu-id="ac733-150">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="ac733-151">схема</span><span class="sxs-lookup"><span data-stu-id="ac733-151">schema</span></span>             |[<span data-ttu-id="ac733-152">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="ac733-152">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="ac733-153">Схема синхронизации по умолчанию для заданий, основанных на этом шаблоне.</span><span class="sxs-lookup"><span data-stu-id="ac733-153">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac733-154">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ac733-154">JSON representation</span></span>

<span data-ttu-id="ac733-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac733-155">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationTemplate"
}-->

```json
{
  "applicationId": "String (identifier)",
  "default": true,
  "description": "String",
  "discoverable": true,
  "factoryTag": "String",
  "id": "String (identifier)",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "schema": {"@odata.type": "microsoft.graph.synchronizationSchema"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


