---
title: Тип ресурса Синчронизатионтемплате
description: Предоставляет предварительно настроенные параметры синхронизации для определенного приложения.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d794391c4cf8043ab4eaeafcfa21958d93e3412a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985687"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="a2247-103">Тип ресурса Синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="a2247-103">synchronizationTemplate resource type</span></span>

<span data-ttu-id="a2247-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2247-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2247-105">Предоставляет предварительно настроенные параметры синхронизации для определенного приложения.</span><span class="sxs-lookup"><span data-stu-id="a2247-105">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="a2247-106">Эти параметры будут использоваться по умолчанию для всех [заданий синхронизации](synchronization-synchronizationjob.md) , основанных на шаблоне.</span><span class="sxs-lookup"><span data-stu-id="a2247-106">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="a2247-107">Разработчик приложения определяет шаблон; любой пользователь может получить шаблон для просмотра параметров по умолчанию, в том числе [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="a2247-107">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="a2247-108">Вы можете предоставить несколько шаблонов для приложения и назначить шаблон по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a2247-108">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="a2247-109">Если для интересующего вас приложения доступно несколько шаблонов, попросите рекомендаций для конкретного приложения, чтобы определить, какой из них наилучшим образом соответствует вашим потребностям.</span><span class="sxs-lookup"><span data-stu-id="a2247-109">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="a2247-110">Методы</span><span class="sxs-lookup"><span data-stu-id="a2247-110">Methods</span></span>

| <span data-ttu-id="a2247-111">Метод</span><span class="sxs-lookup"><span data-stu-id="a2247-111">Method</span></span>        | <span data-ttu-id="a2247-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a2247-112">Return Type</span></span>               | <span data-ttu-id="a2247-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a2247-113">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="a2247-114">Список</span><span class="sxs-lookup"><span data-stu-id="a2247-114">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="a2247-115">Коллекция [синчронизатионтемплате](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="a2247-115">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="a2247-116">Список шаблонов, доступных для приложения или экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="a2247-116">List the templates that are available for an application or application instance (service principal).</span></span>|
|<span data-ttu-id="a2247-117">[получение](../api/synchronization-synchronizationtemplate-get.md);</span><span class="sxs-lookup"><span data-stu-id="a2247-117">[Get](../api/synchronization-synchronizationtemplate-get.md)</span></span>      |[<span data-ttu-id="a2247-118">синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="a2247-118">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="a2247-119">Чтение свойств и связей объекта **синчронизатионтемплате** .</span><span class="sxs-lookup"><span data-stu-id="a2247-119">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="a2247-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2247-120">Properties</span></span>

| <span data-ttu-id="a2247-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2247-121">Property</span></span>      | <span data-ttu-id="a2247-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a2247-122">Type</span></span>                      | <span data-ttu-id="a2247-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a2247-123">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="a2247-124">id</span><span class="sxs-lookup"><span data-stu-id="a2247-124">id</span></span>             |<span data-ttu-id="a2247-125">String</span><span class="sxs-lookup"><span data-stu-id="a2247-125">String</span></span>                     |<span data-ttu-id="a2247-126">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="a2247-126">Unique template identifier.</span></span>|
|<span data-ttu-id="a2247-127">applicationId</span><span class="sxs-lookup"><span data-stu-id="a2247-127">applicationId</span></span>  |<span data-ttu-id="a2247-128">String</span><span class="sxs-lookup"><span data-stu-id="a2247-128">String</span></span>                     |<span data-ttu-id="a2247-129">Идентификатор приложения, к которому принадлежит этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="a2247-129">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="a2247-130">умолчани</span><span class="sxs-lookup"><span data-stu-id="a2247-130">default</span></span>        |<span data-ttu-id="a2247-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2247-131">Boolean</span></span>                    |<span data-ttu-id="a2247-132">`true` Если этот шаблон рекомендуется использовать по умолчанию для приложения.</span><span class="sxs-lookup"><span data-stu-id="a2247-132">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="a2247-133">description</span><span class="sxs-lookup"><span data-stu-id="a2247-133">description</span></span>    |<span data-ttu-id="a2247-134">String</span><span class="sxs-lookup"><span data-stu-id="a2247-134">String</span></span>                     |<span data-ttu-id="a2247-135">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="a2247-135">Description of the template.</span></span>|
|<span data-ttu-id="a2247-136">обнаружения</span><span class="sxs-lookup"><span data-stu-id="a2247-136">discoverable</span></span>   |<span data-ttu-id="a2247-137">String</span><span class="sxs-lookup"><span data-stu-id="a2247-137">String</span></span>                     |<span data-ttu-id="a2247-138">`true` Если этот шаблон должен отображаться в коллекции шаблонов, доступных для экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="a2247-138">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="a2247-139">факторитаг</span><span class="sxs-lookup"><span data-stu-id="a2247-139">factoryTag</span></span>     |<span data-ttu-id="a2247-140">String</span><span class="sxs-lookup"><span data-stu-id="a2247-140">String</span></span>                     |<span data-ttu-id="a2247-141">Один из известных тегов фабрики, поддерживаемых обработчиком синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a2247-141">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="a2247-142">**Факторитаг** сообщает обработчику синхронизации, какую реализацию следует использовать при обработке заданий на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="a2247-142">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="a2247-143">метаданных</span><span class="sxs-lookup"><span data-stu-id="a2247-143">metadata</span></span>       |<span data-ttu-id="a2247-144">Коллекция Метадатаентри</span><span class="sxs-lookup"><span data-stu-id="a2247-144">metadataEntry collection</span></span>   |<span data-ttu-id="a2247-145">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="a2247-145">Additional extension properties.</span></span> <span data-ttu-id="a2247-146">Если явно не указано иное, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="a2247-146">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2247-147">Связи</span><span class="sxs-lookup"><span data-stu-id="a2247-147">Relationships</span></span>
| <span data-ttu-id="a2247-148">Связь</span><span class="sxs-lookup"><span data-stu-id="a2247-148">Relationship</span></span>      | <span data-ttu-id="a2247-149">Тип</span><span class="sxs-lookup"><span data-stu-id="a2247-149">Type</span></span>      |<span data-ttu-id="a2247-150">Описание</span><span class="sxs-lookup"><span data-stu-id="a2247-150">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="a2247-151">схемы</span><span class="sxs-lookup"><span data-stu-id="a2247-151">schema</span></span>             |[<span data-ttu-id="a2247-152">синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="a2247-152">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="a2247-153">Схема синхронизации по умолчанию для заданий, основанных на этом шаблоне.</span><span class="sxs-lookup"><span data-stu-id="a2247-153">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2247-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2247-154">JSON representation</span></span>

<span data-ttu-id="a2247-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2247-155">The following is a JSON representation of the resource.</span></span>

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


