---
title: Тип ресурса synchronizationTemplate
description: " всем пользователям можно извлечь шаблон, чтобы увидеть параметры по умолчанию, включая схемы синхронизации."
localization_priority: Normal
ms.openlocfilehash: e98d3fa16d0a80ac9353aaa75200d8cb24d3e904
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833077"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="283d3-103">Тип ресурса synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="283d3-103">synchronizationTemplate resource type</span></span>

> <span data-ttu-id="283d3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="283d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="283d3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="283d3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="283d3-106">Предоставляет параметры предварительно настроенным синхронизации для конкретного приложения.</span><span class="sxs-lookup"><span data-stu-id="283d3-106">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="283d3-107">Эти параметры будет использоваться по умолчанию для каждого [задания синхронизации](synchronization-synchronizationjob.md) , основанный на шаблоне.</span><span class="sxs-lookup"><span data-stu-id="283d3-107">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="283d3-108">Разработчик приложений задает шаблон; всем пользователям можно извлечь шаблон, чтобы увидеть параметры по умолчанию, включая [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="283d3-108">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="283d3-109">Предоставление нескольких шаблонов для приложения и назначить шаблон по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="283d3-109">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="283d3-110">Если приложение, которое вы хотите несколько шаблонов, seek инструкции для определения, какой из них лучше всего соответствует потребностям приложения.</span><span class="sxs-lookup"><span data-stu-id="283d3-110">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="283d3-111">Методы</span><span class="sxs-lookup"><span data-stu-id="283d3-111">Methods</span></span>

| <span data-ttu-id="283d3-112">Метод</span><span class="sxs-lookup"><span data-stu-id="283d3-112">Method</span></span>        | <span data-ttu-id="283d3-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="283d3-113">Return Type</span></span>               | <span data-ttu-id="283d3-114">Описание</span><span class="sxs-lookup"><span data-stu-id="283d3-114">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="283d3-115">List</span><span class="sxs-lookup"><span data-stu-id="283d3-115">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="283d3-116">[synchronizationTemplate](synchronization-synchronizationtemplate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="283d3-116">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="283d3-117">Список шаблонов, доступных для приложения или экземпляра приложения (участников-служб).</span><span class="sxs-lookup"><span data-stu-id="283d3-117">List the templates that are available for an application or application instance (service principal).</span></span>|
|<span data-ttu-id="283d3-118">[получение](../api/synchronization-synchronizationtemplate-get.md);</span><span class="sxs-lookup"><span data-stu-id="283d3-118">[Get](../api/synchronization-synchronizationtemplate-get.md)</span></span>      |[<span data-ttu-id="283d3-119">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="283d3-119">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="283d3-120">Чтение свойства и связи объекта **synchronizationTemplate** .</span><span class="sxs-lookup"><span data-stu-id="283d3-120">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="283d3-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="283d3-121">Properties</span></span>

| <span data-ttu-id="283d3-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="283d3-122">Property</span></span>      | <span data-ttu-id="283d3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="283d3-123">Type</span></span>                      | <span data-ttu-id="283d3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="283d3-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="283d3-125">id</span><span class="sxs-lookup"><span data-stu-id="283d3-125">id</span></span>             |<span data-ttu-id="283d3-126">Строка</span><span class="sxs-lookup"><span data-stu-id="283d3-126">String</span></span>                     |<span data-ttu-id="283d3-127">Шаблон уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="283d3-127">Unique template identifier.</span></span>|
|<span data-ttu-id="283d3-128">applicationId</span><span class="sxs-lookup"><span data-stu-id="283d3-128">applicationId</span></span>  |<span data-ttu-id="283d3-129">String</span><span class="sxs-lookup"><span data-stu-id="283d3-129">String</span></span>                     |<span data-ttu-id="283d3-130">Идентификатор приложения, к которому принадлежит этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="283d3-130">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="283d3-131">по умолчанию</span><span class="sxs-lookup"><span data-stu-id="283d3-131">default</span></span>        |<span data-ttu-id="283d3-132">Логический</span><span class="sxs-lookup"><span data-stu-id="283d3-132">Boolean</span></span>                    |<span data-ttu-id="283d3-133">`true`Если этот шаблон рекомендуется по умолчанию для приложения.</span><span class="sxs-lookup"><span data-stu-id="283d3-133">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="283d3-134">описание</span><span class="sxs-lookup"><span data-stu-id="283d3-134">description</span></span>    |<span data-ttu-id="283d3-135">String</span><span class="sxs-lookup"><span data-stu-id="283d3-135">String</span></span>                     |<span data-ttu-id="283d3-136">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="283d3-136">Description of the template.</span></span>|
|<span data-ttu-id="283d3-137">обнаруживаемые</span><span class="sxs-lookup"><span data-stu-id="283d3-137">discoverable</span></span>   |<span data-ttu-id="283d3-138">Строка</span><span class="sxs-lookup"><span data-stu-id="283d3-138">String</span></span>                     |<span data-ttu-id="283d3-139">`true`Если этот шаблон должен отображаться в коллекцию шаблонов, доступных для экземпляра приложения (участников-служб).</span><span class="sxs-lookup"><span data-stu-id="283d3-139">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="283d3-140">factoryTag</span><span class="sxs-lookup"><span data-stu-id="283d3-140">factoryTag</span></span>     |<span data-ttu-id="283d3-141">Строка</span><span class="sxs-lookup"><span data-stu-id="283d3-141">String</span></span>                     |<span data-ttu-id="283d3-142">Один из известных фабрики тегов, поддерживаемые обработчиком синхронизации.</span><span class="sxs-lookup"><span data-stu-id="283d3-142">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="283d3-143">**FactoryTag** сообщает о том, обработчик синхронизации реализация для использования при обработке задания на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="283d3-143">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="283d3-144">метаданные</span><span class="sxs-lookup"><span data-stu-id="283d3-144">metadata</span></span>       |<span data-ttu-id="283d3-145">metadataEntry коллекции</span><span class="sxs-lookup"><span data-stu-id="283d3-145">metadataEntry collection</span></span>   |<span data-ttu-id="283d3-146">Расширение дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="283d3-146">Additional extension properties.</span></span> <span data-ttu-id="283d3-147">Если не указан явно, значения метаданных не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="283d3-147">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="283d3-148">Связи</span><span class="sxs-lookup"><span data-stu-id="283d3-148">Relationships</span></span>
| <span data-ttu-id="283d3-149">Связь</span><span class="sxs-lookup"><span data-stu-id="283d3-149">Relationship</span></span>      | <span data-ttu-id="283d3-150">Тип</span><span class="sxs-lookup"><span data-stu-id="283d3-150">Type</span></span>      |<span data-ttu-id="283d3-151">Описание</span><span class="sxs-lookup"><span data-stu-id="283d3-151">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="283d3-152">схема</span><span class="sxs-lookup"><span data-stu-id="283d3-152">schema</span></span>             |[<span data-ttu-id="283d3-153">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="283d3-153">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="283d3-154">Схема синхронизации по умолчанию для заданий на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="283d3-154">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="283d3-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="283d3-155">JSON representation</span></span>

<span data-ttu-id="283d3-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="283d3-156">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
