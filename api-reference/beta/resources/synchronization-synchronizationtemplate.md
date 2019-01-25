---
title: Тип ресурса synchronizationTemplate
description: " всем пользователям можно извлечь шаблон, чтобы увидеть параметры по умолчанию, включая схемы синхронизации."
localization_priority: Normal
ms.openlocfilehash: 75df13d55cfb58aafe8a751279e103424aa29367
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516555"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="298aa-103">Тип ресурса synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="298aa-103">synchronizationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="298aa-104">Предоставляет параметры предварительно настроенным синхронизации для конкретного приложения.</span><span class="sxs-lookup"><span data-stu-id="298aa-104">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="298aa-105">Эти параметры будет использоваться по умолчанию для каждого [задания синхронизации](synchronization-synchronizationjob.md) , основанный на шаблоне.</span><span class="sxs-lookup"><span data-stu-id="298aa-105">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="298aa-106">Разработчик приложений задает шаблон; всем пользователям можно извлечь шаблон, чтобы увидеть параметры по умолчанию, включая [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="298aa-106">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="298aa-107">Предоставление нескольких шаблонов для приложения и назначить шаблон по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="298aa-107">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="298aa-108">Если приложение, которое вы хотите несколько шаблонов, seek инструкции для определения, какой из них лучше всего соответствует потребностям приложения.</span><span class="sxs-lookup"><span data-stu-id="298aa-108">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="298aa-109">Методы</span><span class="sxs-lookup"><span data-stu-id="298aa-109">Methods</span></span>

| <span data-ttu-id="298aa-110">Метод</span><span class="sxs-lookup"><span data-stu-id="298aa-110">Method</span></span>        | <span data-ttu-id="298aa-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="298aa-111">Return Type</span></span>               | <span data-ttu-id="298aa-112">Описание</span><span class="sxs-lookup"><span data-stu-id="298aa-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="298aa-113">List</span><span class="sxs-lookup"><span data-stu-id="298aa-113">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="298aa-114">[synchronizationTemplate](synchronization-synchronizationtemplate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="298aa-114">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="298aa-115">Список шаблонов, доступных для приложения или экземпляра приложения (участников-служб).</span><span class="sxs-lookup"><span data-stu-id="298aa-115">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="298aa-116">Get</span><span class="sxs-lookup"><span data-stu-id="298aa-116">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="298aa-117">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="298aa-117">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="298aa-118">Чтение свойства и связи объекта **synchronizationTemplate** .</span><span class="sxs-lookup"><span data-stu-id="298aa-118">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="298aa-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="298aa-119">Properties</span></span>

| <span data-ttu-id="298aa-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="298aa-120">Property</span></span>      | <span data-ttu-id="298aa-121">Тип</span><span class="sxs-lookup"><span data-stu-id="298aa-121">Type</span></span>                      | <span data-ttu-id="298aa-122">Описание</span><span class="sxs-lookup"><span data-stu-id="298aa-122">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="298aa-123">id</span><span class="sxs-lookup"><span data-stu-id="298aa-123">id</span></span>             |<span data-ttu-id="298aa-124">String</span><span class="sxs-lookup"><span data-stu-id="298aa-124">String</span></span>                     |<span data-ttu-id="298aa-125">Шаблон уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="298aa-125">Unique template identifier.</span></span>|
|<span data-ttu-id="298aa-126">applicationId</span><span class="sxs-lookup"><span data-stu-id="298aa-126">applicationId</span></span>  |<span data-ttu-id="298aa-127">String</span><span class="sxs-lookup"><span data-stu-id="298aa-127">String</span></span>                     |<span data-ttu-id="298aa-128">Идентификатор приложения, к которому принадлежит этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="298aa-128">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="298aa-129">по умолчанию</span><span class="sxs-lookup"><span data-stu-id="298aa-129">default</span></span>        |<span data-ttu-id="298aa-130">Логическое</span><span class="sxs-lookup"><span data-stu-id="298aa-130">Boolean</span></span>                    |<span data-ttu-id="298aa-131">`true`Если этот шаблон рекомендуется по умолчанию для приложения.</span><span class="sxs-lookup"><span data-stu-id="298aa-131">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="298aa-132">description</span><span class="sxs-lookup"><span data-stu-id="298aa-132">description</span></span>    |<span data-ttu-id="298aa-133">String</span><span class="sxs-lookup"><span data-stu-id="298aa-133">String</span></span>                     |<span data-ttu-id="298aa-134">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="298aa-134">Description of the template.</span></span>|
|<span data-ttu-id="298aa-135">обнаруживаемые</span><span class="sxs-lookup"><span data-stu-id="298aa-135">discoverable</span></span>   |<span data-ttu-id="298aa-136">String</span><span class="sxs-lookup"><span data-stu-id="298aa-136">String</span></span>                     |<span data-ttu-id="298aa-137">`true`Если этот шаблон должен отображаться в коллекцию шаблонов, доступных для экземпляра приложения (участников-служб).</span><span class="sxs-lookup"><span data-stu-id="298aa-137">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="298aa-138">factoryTag</span><span class="sxs-lookup"><span data-stu-id="298aa-138">factoryTag</span></span>     |<span data-ttu-id="298aa-139">String</span><span class="sxs-lookup"><span data-stu-id="298aa-139">String</span></span>                     |<span data-ttu-id="298aa-140">Один из известных фабрики тегов, поддерживаемые обработчиком синхронизации.</span><span class="sxs-lookup"><span data-stu-id="298aa-140">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="298aa-141">**FactoryTag** сообщает о том, обработчик синхронизации реализация для использования при обработке задания на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="298aa-141">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="298aa-142">Метаданные</span><span class="sxs-lookup"><span data-stu-id="298aa-142">metadata</span></span>       |<span data-ttu-id="298aa-143">metadataEntry коллекции</span><span class="sxs-lookup"><span data-stu-id="298aa-143">metadataEntry collection</span></span>   |<span data-ttu-id="298aa-144">Расширение дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="298aa-144">Additional extension properties.</span></span> <span data-ttu-id="298aa-145">Если не указан явно, значения метаданных не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="298aa-145">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="298aa-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="298aa-146">Relationships</span></span>
| <span data-ttu-id="298aa-147">Связь</span><span class="sxs-lookup"><span data-stu-id="298aa-147">Relationship</span></span>      | <span data-ttu-id="298aa-148">Тип</span><span class="sxs-lookup"><span data-stu-id="298aa-148">Type</span></span>      |<span data-ttu-id="298aa-149">Описание</span><span class="sxs-lookup"><span data-stu-id="298aa-149">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="298aa-150">схема</span><span class="sxs-lookup"><span data-stu-id="298aa-150">schema</span></span>             |[<span data-ttu-id="298aa-151">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="298aa-151">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="298aa-152">Схема синхронизации по умолчанию для заданий на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="298aa-152">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="298aa-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="298aa-153">JSON representation</span></span>

<span data-ttu-id="298aa-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="298aa-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
