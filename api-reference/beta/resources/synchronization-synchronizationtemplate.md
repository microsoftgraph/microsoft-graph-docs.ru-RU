---
title: Тип ресурса Синчронизатионтемплате
description: " любой пользователь может получить шаблон для просмотра параметров по умолчанию, в том числе схемы синхронизации."
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9952b06276efa712068091ecd8b7b5dc5e6769d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520018"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="27e53-103">Тип ресурса Синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="27e53-103">synchronizationTemplate resource type</span></span>

<span data-ttu-id="27e53-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="27e53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27e53-105">Предоставляет предварительно настроенные параметры синхронизации для определенного приложения.</span><span class="sxs-lookup"><span data-stu-id="27e53-105">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="27e53-106">Эти параметры будут использоваться по умолчанию для всех [заданий синхронизации](synchronization-synchronizationjob.md) , основанных на шаблоне.</span><span class="sxs-lookup"><span data-stu-id="27e53-106">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="27e53-107">Разработчик приложения определяет шаблон; любой пользователь может получить шаблон для просмотра параметров по умолчанию, в том числе [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="27e53-107">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="27e53-108">Вы можете предоставить несколько шаблонов для приложения и назначить шаблон по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="27e53-108">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="27e53-109">Если для интересующего вас приложения доступно несколько шаблонов, попросите рекомендаций для конкретного приложения, чтобы определить, какой из них наилучшим образом соответствует вашим потребностям.</span><span class="sxs-lookup"><span data-stu-id="27e53-109">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="27e53-110">Методы</span><span class="sxs-lookup"><span data-stu-id="27e53-110">Methods</span></span>

| <span data-ttu-id="27e53-111">Метод</span><span class="sxs-lookup"><span data-stu-id="27e53-111">Method</span></span>        | <span data-ttu-id="27e53-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="27e53-112">Return Type</span></span>               | <span data-ttu-id="27e53-113">Описание</span><span class="sxs-lookup"><span data-stu-id="27e53-113">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="27e53-114">List</span><span class="sxs-lookup"><span data-stu-id="27e53-114">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="27e53-115">Коллекция [синчронизатионтемплате](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="27e53-115">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="27e53-116">Список шаблонов, доступных для приложения или экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="27e53-116">List the templates that are available for an application or application instance (service principal).</span></span>|
|<span data-ttu-id="27e53-117">[получение](../api/synchronization-synchronizationtemplate-get.md);</span><span class="sxs-lookup"><span data-stu-id="27e53-117">[Get](../api/synchronization-synchronizationtemplate-get.md)</span></span>      |[<span data-ttu-id="27e53-118">синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="27e53-118">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="27e53-119">Чтение свойств и связей объекта **синчронизатионтемплате** .</span><span class="sxs-lookup"><span data-stu-id="27e53-119">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="27e53-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="27e53-120">Properties</span></span>

| <span data-ttu-id="27e53-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="27e53-121">Property</span></span>      | <span data-ttu-id="27e53-122">Тип</span><span class="sxs-lookup"><span data-stu-id="27e53-122">Type</span></span>                      | <span data-ttu-id="27e53-123">Описание</span><span class="sxs-lookup"><span data-stu-id="27e53-123">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="27e53-124">id</span><span class="sxs-lookup"><span data-stu-id="27e53-124">id</span></span>             |<span data-ttu-id="27e53-125">Строка</span><span class="sxs-lookup"><span data-stu-id="27e53-125">String</span></span>                     |<span data-ttu-id="27e53-126">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="27e53-126">Unique template identifier.</span></span>|
|<span data-ttu-id="27e53-127">applicationId</span><span class="sxs-lookup"><span data-stu-id="27e53-127">applicationId</span></span>  |<span data-ttu-id="27e53-128">String</span><span class="sxs-lookup"><span data-stu-id="27e53-128">String</span></span>                     |<span data-ttu-id="27e53-129">Идентификатор приложения, к которому принадлежит этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="27e53-129">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="27e53-130">умолчани</span><span class="sxs-lookup"><span data-stu-id="27e53-130">default</span></span>        |<span data-ttu-id="27e53-131">Логический</span><span class="sxs-lookup"><span data-stu-id="27e53-131">Boolean</span></span>                    |<span data-ttu-id="27e53-132">`true`Если этот шаблон рекомендуется использовать по умолчанию для приложения.</span><span class="sxs-lookup"><span data-stu-id="27e53-132">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="27e53-133">description</span><span class="sxs-lookup"><span data-stu-id="27e53-133">description</span></span>    |<span data-ttu-id="27e53-134">String</span><span class="sxs-lookup"><span data-stu-id="27e53-134">String</span></span>                     |<span data-ttu-id="27e53-135">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="27e53-135">Description of the template.</span></span>|
|<span data-ttu-id="27e53-136">обнаружения</span><span class="sxs-lookup"><span data-stu-id="27e53-136">discoverable</span></span>   |<span data-ttu-id="27e53-137">String</span><span class="sxs-lookup"><span data-stu-id="27e53-137">String</span></span>                     |<span data-ttu-id="27e53-138">`true`Если этот шаблон должен отображаться в коллекции шаблонов, доступных для экземпляра приложения (субъекта-службы).</span><span class="sxs-lookup"><span data-stu-id="27e53-138">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="27e53-139">факторитаг</span><span class="sxs-lookup"><span data-stu-id="27e53-139">factoryTag</span></span>     |<span data-ttu-id="27e53-140">String</span><span class="sxs-lookup"><span data-stu-id="27e53-140">String</span></span>                     |<span data-ttu-id="27e53-141">Один из известных тегов фабрики, поддерживаемых обработчиком синхронизации.</span><span class="sxs-lookup"><span data-stu-id="27e53-141">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="27e53-142">**Факторитаг** сообщает обработчику синхронизации, какую реализацию следует использовать при обработке заданий на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="27e53-142">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="27e53-143">метаданных</span><span class="sxs-lookup"><span data-stu-id="27e53-143">metadata</span></span>       |<span data-ttu-id="27e53-144">Коллекция Метадатаентри</span><span class="sxs-lookup"><span data-stu-id="27e53-144">metadataEntry collection</span></span>   |<span data-ttu-id="27e53-145">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="27e53-145">Additional extension properties.</span></span> <span data-ttu-id="27e53-146">Если явно не указано иное, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="27e53-146">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27e53-147">Связи</span><span class="sxs-lookup"><span data-stu-id="27e53-147">Relationships</span></span>
| <span data-ttu-id="27e53-148">Связь</span><span class="sxs-lookup"><span data-stu-id="27e53-148">Relationship</span></span>      | <span data-ttu-id="27e53-149">Тип</span><span class="sxs-lookup"><span data-stu-id="27e53-149">Type</span></span>      |<span data-ttu-id="27e53-150">Описание</span><span class="sxs-lookup"><span data-stu-id="27e53-150">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="27e53-151">схемы</span><span class="sxs-lookup"><span data-stu-id="27e53-151">schema</span></span>             |[<span data-ttu-id="27e53-152">синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="27e53-152">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="27e53-153">Схема синхронизации по умолчанию для заданий, основанных на этом шаблоне.</span><span class="sxs-lookup"><span data-stu-id="27e53-153">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27e53-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27e53-154">JSON representation</span></span>

<span data-ttu-id="27e53-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27e53-155">The following is a JSON representation of the resource.</span></span>

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
