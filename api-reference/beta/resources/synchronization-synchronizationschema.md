---
title: Тип ресурса synchronizationSchema
description: Определяет объекты, которые будут синхронизированы и как они будут синхронизироваться. Схема синхронизации содержит основные сведения об установке для задания синхронизации. Как правило будет настроить некоторые сопоставления атрибутов или добавить фильтр области видимости, чтобы синхронизировать только объекты, удовлетворяющие определенному условию.
localization_priority: Normal
ms.openlocfilehash: 696bdbbc6fa2d96965d11a12fb09fdfc0ce16106
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847322"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="307dd-105">Тип ресурса synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="307dd-105">synchronizationSchema resource type</span></span>

> <span data-ttu-id="307dd-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="307dd-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="307dd-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="307dd-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="307dd-108">Определяет объекты, которые будут синхронизированы и как они будут синхронизироваться.</span><span class="sxs-lookup"><span data-stu-id="307dd-108">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="307dd-109">Схема синхронизации содержит основные сведения об установке для задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="307dd-109">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="307dd-110">Как правило будет настроить некоторые [атрибут сопоставления](synchronization-attributemapping.md)или добавить [области видимости фильтров](synchronization-filter.md) синхронизировать только объекты, удовлетворяющие определенному условию.</span><span class="sxs-lookup"><span data-stu-id="307dd-110">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="307dd-111">В следующих разделах компонентов высокого уровня схемы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="307dd-111">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="307dd-112">Определения каталогов</span><span class="sxs-lookup"><span data-stu-id="307dd-112">Directory definitions</span></span>

<span data-ttu-id="307dd-113">[Каталог определения](synchronization-directorydefinition.md) обеспечивают синхронизации сведения о каталогах и их объектами.</span><span class="sxs-lookup"><span data-stu-id="307dd-113">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="307dd-114">Например определение каталога сообщает обработчик синхронизации, что в каталоге Azure AD объекты с именем **пользователя** и **группы**, какие атрибуты поддерживаются для этих объектов и типы для этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="307dd-114">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="307dd-115">Чтобы определенного объектов и атрибутов для использования в сопоставления правил/объекта синхронизации они должны быть определен как часть определения каталога.</span><span class="sxs-lookup"><span data-stu-id="307dd-115">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="307dd-116">Правила синхронизации</span><span class="sxs-lookup"><span data-stu-id="307dd-116">Synchronization rules</span></span>

<span data-ttu-id="307dd-117">[Правила синхронизации](synchronization-synchronizationrule.md) — это основной настройки синхронизации.</span><span class="sxs-lookup"><span data-stu-id="307dd-117">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="307dd-118">Они подсистемы синхронизации определяют, как выполнять синхронизацию, включая какие объекты должны быть синхронизированы, как объекты из исходного каталога должны совпадать с объектами в целевом каталоге, и как должен быть атрибуты преобразовать их в случае синхронизации из источника в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="307dd-118">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span> 

## <a name="object-mappings"></a><span data-ttu-id="307dd-119">Объект сопоставления</span><span class="sxs-lookup"><span data-stu-id="307dd-119">Object mappings</span></span>

<span data-ttu-id="307dd-120">[Объект сопоставления](synchronization-objectmapping.md) отличаются основной части правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="307dd-120">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="307dd-121">Сопоставление объектов в каждом определяет, как того или иного объекта должны быть синхронизированы из источника в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="307dd-121">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="307dd-122">В частности, сопоставление определяются как объект в исходный каталог должны совпадать с помощью объекта в целевой каталог, что (если они имеются) области Фильтры следует использовать в том, следует ли предоставить объект и как следует преобразование атрибуты объектов При их в случае синхронизации из источника в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="307dd-122">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="307dd-123">Методы</span><span class="sxs-lookup"><span data-stu-id="307dd-123">Methods</span></span>

| <span data-ttu-id="307dd-124">Метод</span><span class="sxs-lookup"><span data-stu-id="307dd-124">Method</span></span>        | <span data-ttu-id="307dd-125">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="307dd-125">Return Type</span></span>               | <span data-ttu-id="307dd-126">Описание</span><span class="sxs-lookup"><span data-stu-id="307dd-126">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="307dd-127">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="307dd-127">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="307dd-128">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="307dd-128">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="307dd-129">Чтение свойства и связи объекта **synchronizationSchema** .</span><span class="sxs-lookup"><span data-stu-id="307dd-129">Read properties and relationships of the **synchronizationSchema** object.</span></span>|
|[<span data-ttu-id="307dd-130">Схема обновления</span><span class="sxs-lookup"><span data-stu-id="307dd-130">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="307dd-131">Нет</span><span class="sxs-lookup"><span data-stu-id="307dd-131">None</span></span>   |<span data-ttu-id="307dd-132">Обновление схемы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="307dd-132">Update the synchronization schema.</span></span> |
|[<span data-ttu-id="307dd-133">Удаление схемы</span><span class="sxs-lookup"><span data-stu-id="307dd-133">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)    |<span data-ttu-id="307dd-134">Нет</span><span class="sxs-lookup"><span data-stu-id="307dd-134">None</span></span>   |<span data-ttu-id="307dd-135">Удаление настраиваемой схемы, сброс схемы в конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="307dd-135">Delete the customized schema, resetting the schema to the default configuration.</span></span> |
|[<span data-ttu-id="307dd-136">Список фильтров операторы</span><span class="sxs-lookup"><span data-stu-id="307dd-136">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)    |<span data-ttu-id="307dd-137">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="307dd-137">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) colection</span></span>   |<span data-ttu-id="307dd-138">Список всех операторы, поддерживаемые в области видимости фильтров.</span><span class="sxs-lookup"><span data-stu-id="307dd-138">List all operators supported in the scoping filters.</span></span> |
|[<span data-ttu-id="307dd-139">Атрибут списка сопоставление функций</span><span class="sxs-lookup"><span data-stu-id="307dd-139">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)    |<span data-ttu-id="307dd-140">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="307dd-140">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>   |<span data-ttu-id="307dd-141">Перечислены все функции, поддерживаемые в выражениях сопоставления атрибута.</span><span class="sxs-lookup"><span data-stu-id="307dd-141">List all functions supported in the attribute mapping expressions.</span></span> |
|[<span data-ttu-id="307dd-142">Синтаксический анализ выражения сопоставление атрибутов</span><span class="sxs-lookup"><span data-stu-id="307dd-142">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md)|[<span data-ttu-id="307dd-143">parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="307dd-143">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)|<span data-ttu-id="307dd-144">Синтаксический анализ строковое выражение в [attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="307dd-144">Parse a string expression into an [attributeMappingSource</span></span>|<span data-ttu-id="307dd-145">(.. / resources/synchronization_attributemappingsource.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="307dd-145">(../resources/synchronization_attributemappingsource.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="307dd-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="307dd-146">Properties</span></span>

| <span data-ttu-id="307dd-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="307dd-147">Property</span></span>      | <span data-ttu-id="307dd-148">Тип</span><span class="sxs-lookup"><span data-stu-id="307dd-148">Type</span></span>      | <span data-ttu-id="307dd-149">Описание</span><span class="sxs-lookup"><span data-stu-id="307dd-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="307dd-150">directories</span><span class="sxs-lookup"><span data-stu-id="307dd-150">directories</span></span>            |<span data-ttu-id="307dd-151">[directoryDefinition](synchronization-directorydefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="307dd-151">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="307dd-152">Описывает каталоги и объекты, которые входят в состав [synchronizationJob](synchronization-synchronizationjob.md) или [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="307dd-152">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="307dd-153">synchronizationRules</span><span class="sxs-lookup"><span data-stu-id="307dd-153">synchronizationRules</span></span>   |<span data-ttu-id="307dd-154">[synchronizationRule](synchronization-synchronizationrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="307dd-154">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="307dd-155">Коллекция правил синхронизации, настроенных для [synchronizationJob](synchronization-synchronizationjob.md) или [synchronizationTemplate](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="307dd-155">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="307dd-156">version</span><span class="sxs-lookup"><span data-stu-id="307dd-156">version</span></span>                |<span data-ttu-id="307dd-157">Строка</span><span class="sxs-lookup"><span data-stu-id="307dd-157">String</span></span>                             |<span data-ttu-id="307dd-158">Версия схемы, автоматического обновления при каждом изменении схемы.</span><span class="sxs-lookup"><span data-stu-id="307dd-158">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="307dd-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="307dd-159">JSON representation</span></span>

<span data-ttu-id="307dd-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="307dd-160">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchema"
}-->

```json
{
  "directories": [{"@odata.type": "microsoft.graph.directoryDefinition"}],
  "provisioningTaskIdentifier": "String (identifier)",
  "synchronizationRules": [{"@odata.type": "microsoft.graph.synchronizationRule"}],
  "version": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
