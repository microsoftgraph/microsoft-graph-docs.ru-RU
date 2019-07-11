---
title: Тип ресурса Синчронизатионтемплате
description: " любой пользователь может получить шаблон для просмотра параметров по умолчанию, в том числе схемы синхронизации."
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 125b8fe81aedc285da33380c3043827c7c534ab8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620649"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="ef5b3-103">Тип ресурса Синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="ef5b3-103">synchronizationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef5b3-104">Предоставляет предварительно настроенные параметры синхронизации для определенного приложения.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-104">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="ef5b3-105">Эти параметры будут использоваться по умолчанию для всех [заданий синхронизации](synchronization-synchronizationjob.md) , основанных на шаблоне.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-105">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="ef5b3-106">Разработчик приложения определяет шаблон; любой пользователь может получить шаблон для просмотра параметров по умолчанию, в том числе [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="ef5b3-106">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="ef5b3-107">Вы можете предоставить несколько шаблонов для приложения и назначить шаблон по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-107">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="ef5b3-108">Если для интересующего вас приложения доступно несколько шаблонов, попросите рекомендаций для конкретного приложения, чтобы определить, какой из них наилучшим образом соответствует вашим потребностям.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-108">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="ef5b3-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ef5b3-109">Methods</span></span>

| <span data-ttu-id="ef5b3-110">Метод</span><span class="sxs-lookup"><span data-stu-id="ef5b3-110">Method</span></span>        | <span data-ttu-id="ef5b3-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ef5b3-111">Return Type</span></span>               | <span data-ttu-id="ef5b3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ef5b3-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="ef5b3-113">List</span><span class="sxs-lookup"><span data-stu-id="ef5b3-113">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="ef5b3-114">Коллекция [синчронизатионтемплате](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="ef5b3-114">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="ef5b3-115">Список шаблонов, доступных для приложения или экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="ef5b3-115">List the templates that are available for an application or application instance (service principal).</span></span>|
|<span data-ttu-id="ef5b3-116">[получение](../api/synchronization-synchronizationtemplate-get.md);</span><span class="sxs-lookup"><span data-stu-id="ef5b3-116">[Get](../api/synchronization-synchronizationtemplate-get.md)</span></span>      |[<span data-ttu-id="ef5b3-117">Синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="ef5b3-117">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="ef5b3-118">Чтение свойств и связей объекта **синчронизатионтемплате** .</span><span class="sxs-lookup"><span data-stu-id="ef5b3-118">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="ef5b3-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef5b3-119">Properties</span></span>

| <span data-ttu-id="ef5b3-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef5b3-120">Property</span></span>      | <span data-ttu-id="ef5b3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ef5b3-121">Type</span></span>                      | <span data-ttu-id="ef5b3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ef5b3-122">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="ef5b3-123">id</span><span class="sxs-lookup"><span data-stu-id="ef5b3-123">id</span></span>             |<span data-ttu-id="ef5b3-124">Строка</span><span class="sxs-lookup"><span data-stu-id="ef5b3-124">String</span></span>                     |<span data-ttu-id="ef5b3-125">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-125">Unique template identifier.</span></span>|
|<span data-ttu-id="ef5b3-126">applicationId</span><span class="sxs-lookup"><span data-stu-id="ef5b3-126">applicationId</span></span>  |<span data-ttu-id="ef5b3-127">String</span><span class="sxs-lookup"><span data-stu-id="ef5b3-127">String</span></span>                     |<span data-ttu-id="ef5b3-128">Идентификатор приложения, к которому принадлежит этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-128">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="ef5b3-129">умолчани</span><span class="sxs-lookup"><span data-stu-id="ef5b3-129">default</span></span>        |<span data-ttu-id="ef5b3-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef5b3-130">Boolean</span></span>                    |<span data-ttu-id="ef5b3-131">`true`Если этот шаблон рекомендуется использовать по умолчанию для приложения.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-131">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="ef5b3-132">description</span><span class="sxs-lookup"><span data-stu-id="ef5b3-132">description</span></span>    |<span data-ttu-id="ef5b3-133">String</span><span class="sxs-lookup"><span data-stu-id="ef5b3-133">String</span></span>                     |<span data-ttu-id="ef5b3-134">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-134">Description of the template.</span></span>|
|<span data-ttu-id="ef5b3-135">обнаружения</span><span class="sxs-lookup"><span data-stu-id="ef5b3-135">discoverable</span></span>   |<span data-ttu-id="ef5b3-136">String</span><span class="sxs-lookup"><span data-stu-id="ef5b3-136">String</span></span>                     |<span data-ttu-id="ef5b3-137">`true`Если этот шаблон должен отображаться в коллекции шаблонов, доступных для экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="ef5b3-137">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="ef5b3-138">Факторитаг</span><span class="sxs-lookup"><span data-stu-id="ef5b3-138">factoryTag</span></span>     |<span data-ttu-id="ef5b3-139">String</span><span class="sxs-lookup"><span data-stu-id="ef5b3-139">String</span></span>                     |<span data-ttu-id="ef5b3-140">Один из известных тегов фабрики, поддерживаемых обработчиком синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-140">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="ef5b3-141">**Факторитаг** сообщает обработчику синхронизации, какую реализацию следует использовать при обработке заданий на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-141">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="ef5b3-142">метаданных</span><span class="sxs-lookup"><span data-stu-id="ef5b3-142">metadata</span></span>       |<span data-ttu-id="ef5b3-143">Коллекция Метадатаентри</span><span class="sxs-lookup"><span data-stu-id="ef5b3-143">metadataEntry collection</span></span>   |<span data-ttu-id="ef5b3-144">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-144">Additional extension properties.</span></span> <span data-ttu-id="ef5b3-145">Если явно не указано иное, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-145">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef5b3-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="ef5b3-146">Relationships</span></span>
| <span data-ttu-id="ef5b3-147">Отношение</span><span class="sxs-lookup"><span data-stu-id="ef5b3-147">Relationship</span></span>      | <span data-ttu-id="ef5b3-148">Тип</span><span class="sxs-lookup"><span data-stu-id="ef5b3-148">Type</span></span>      |<span data-ttu-id="ef5b3-149">Описание</span><span class="sxs-lookup"><span data-stu-id="ef5b3-149">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="ef5b3-150">схемы</span><span class="sxs-lookup"><span data-stu-id="ef5b3-150">schema</span></span>             |[<span data-ttu-id="ef5b3-151">Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="ef5b3-151">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="ef5b3-152">Схема синхронизации по умолчанию для заданий, основанных на этом шаблоне.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-152">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef5b3-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef5b3-153">JSON representation</span></span>

<span data-ttu-id="ef5b3-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef5b3-154">The following is a JSON representation of the resource.</span></span>

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
