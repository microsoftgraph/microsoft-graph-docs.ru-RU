---
title: Тип ресурса synchronizationSchema
description: Определяет объекты, которые будут синхронизированы и как они будут синхронизироваться. Схема синхронизации содержит основные сведения об установке для задания синхронизации. Как правило будет настроить некоторые сопоставления атрибутов или добавить фильтр области видимости, чтобы синхронизировать только объекты, удовлетворяющие определенному условию.
localization_priority: Normal
ms.openlocfilehash: e7bb91ef473a04552c4c5f33ffc9d54eb86a9b7a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515932"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="d272d-105">Тип ресурса synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="d272d-105">synchronizationSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d272d-106">Определяет объекты, которые будут синхронизированы и как они будут синхронизироваться.</span><span class="sxs-lookup"><span data-stu-id="d272d-106">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="d272d-107">Схема синхронизации содержит основные сведения об установке для задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d272d-107">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="d272d-108">Как правило будет настроить некоторые [атрибут сопоставления](synchronization-attributemapping.md)или добавить [области видимости фильтров](synchronization-filter.md) синхронизировать только объекты, удовлетворяющие определенному условию.</span><span class="sxs-lookup"><span data-stu-id="d272d-108">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="d272d-109">В следующих разделах компонентов высокого уровня схемы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d272d-109">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="d272d-110">Определения каталогов</span><span class="sxs-lookup"><span data-stu-id="d272d-110">Directory definitions</span></span>

<span data-ttu-id="d272d-111">[Каталог определения](synchronization-directorydefinition.md) обеспечивают синхронизации сведения о каталогах и их объектами.</span><span class="sxs-lookup"><span data-stu-id="d272d-111">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="d272d-112">Например определение каталога сообщает обработчик синхронизации, что в каталоге Azure AD объекты с именем **пользователя** и **группы**, какие атрибуты поддерживаются для этих объектов и типы для этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="d272d-112">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="d272d-113">Чтобы определенного объектов и атрибутов для использования в сопоставления правил/объекта синхронизации они должны быть определен как часть определения каталога.</span><span class="sxs-lookup"><span data-stu-id="d272d-113">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="d272d-114">Правила синхронизации</span><span class="sxs-lookup"><span data-stu-id="d272d-114">Synchronization rules</span></span>

<span data-ttu-id="d272d-115">[Правила синхронизации](synchronization-synchronizationrule.md) — это основной настройки синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d272d-115">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="d272d-116">Они подсистемы синхронизации определяют, как выполнять синхронизацию, включая какие объекты должны быть синхронизированы, как объекты из исходного каталога должны совпадать с объектами в целевом каталоге, и как должен быть атрибуты преобразовать их в случае синхронизации из источника в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="d272d-116">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span> 

## <a name="object-mappings"></a><span data-ttu-id="d272d-117">Объект сопоставления</span><span class="sxs-lookup"><span data-stu-id="d272d-117">Object mappings</span></span>

<span data-ttu-id="d272d-118">[Объект сопоставления](synchronization-objectmapping.md) отличаются основной части правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d272d-118">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="d272d-119">Сопоставление объектов в каждом определяет, как того или иного объекта должны быть синхронизированы из источника в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="d272d-119">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="d272d-120">В частности, сопоставление определяются как объект в исходный каталог должны совпадать с помощью объекта в целевой каталог, что (если они имеются) области Фильтры следует использовать в том, следует ли предоставить объект и как следует преобразование атрибуты объектов При их в случае синхронизации из источника в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="d272d-120">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="d272d-121">Методы</span><span class="sxs-lookup"><span data-stu-id="d272d-121">Methods</span></span>

| <span data-ttu-id="d272d-122">Метод</span><span class="sxs-lookup"><span data-stu-id="d272d-122">Method</span></span>        | <span data-ttu-id="d272d-123">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d272d-123">Return Type</span></span>               | <span data-ttu-id="d272d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d272d-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="d272d-125">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="d272d-125">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="d272d-126">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="d272d-126">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="d272d-127">Чтение свойства и связи объекта **synchronizationSchema** .</span><span class="sxs-lookup"><span data-stu-id="d272d-127">Read properties and relationships of the **synchronizationSchema** object.</span></span>|
|[<span data-ttu-id="d272d-128">Схема обновления</span><span class="sxs-lookup"><span data-stu-id="d272d-128">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="d272d-129">Нет</span><span class="sxs-lookup"><span data-stu-id="d272d-129">None</span></span>   |<span data-ttu-id="d272d-130">Обновление схемы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d272d-130">Update the synchronization schema.</span></span> |
|[<span data-ttu-id="d272d-131">Удаление схемы</span><span class="sxs-lookup"><span data-stu-id="d272d-131">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)    |<span data-ttu-id="d272d-132">Нет</span><span class="sxs-lookup"><span data-stu-id="d272d-132">None</span></span>   |<span data-ttu-id="d272d-133">Удаление настраиваемой схемы, сброс схемы в конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d272d-133">Delete the customized schema, resetting the schema to the default configuration.</span></span> |
|[<span data-ttu-id="d272d-134">Список фильтров операторы</span><span class="sxs-lookup"><span data-stu-id="d272d-134">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)    |<span data-ttu-id="d272d-135">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d272d-135">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) colection</span></span>   |<span data-ttu-id="d272d-136">Список всех операторы, поддерживаемые в области видимости фильтров.</span><span class="sxs-lookup"><span data-stu-id="d272d-136">List all operators supported in the scoping filters.</span></span> |
|[<span data-ttu-id="d272d-137">Атрибут списка сопоставление функций</span><span class="sxs-lookup"><span data-stu-id="d272d-137">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)    |<span data-ttu-id="d272d-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d272d-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>   |<span data-ttu-id="d272d-139">Перечислены все функции, поддерживаемые в выражениях сопоставления атрибута.</span><span class="sxs-lookup"><span data-stu-id="d272d-139">List all functions supported in the attribute mapping expressions.</span></span> |
|[<span data-ttu-id="d272d-140">Синтаксический анализ выражения сопоставление атрибутов</span><span class="sxs-lookup"><span data-stu-id="d272d-140">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md)|[<span data-ttu-id="d272d-141">parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="d272d-141">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)|<span data-ttu-id="d272d-142">Синтаксический анализ строковое выражение в [attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="d272d-142">Parse a string expression into an [attributeMappingSource</span></span>|<span data-ttu-id="d272d-143">(.. / resources/synchronization_attributemappingsource.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="d272d-143">(../resources/synchronization_attributemappingsource.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="d272d-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="d272d-144">Properties</span></span>

| <span data-ttu-id="d272d-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="d272d-145">Property</span></span>      | <span data-ttu-id="d272d-146">Тип</span><span class="sxs-lookup"><span data-stu-id="d272d-146">Type</span></span>      | <span data-ttu-id="d272d-147">Описание</span><span class="sxs-lookup"><span data-stu-id="d272d-147">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="d272d-148">directories</span><span class="sxs-lookup"><span data-stu-id="d272d-148">directories</span></span>            |<span data-ttu-id="d272d-149">[directoryDefinition](synchronization-directorydefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d272d-149">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="d272d-150">Описывает каталоги и объекты, которые входят в состав [synchronizationJob](synchronization-synchronizationjob.md) или [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="d272d-150">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="d272d-151">synchronizationRules</span><span class="sxs-lookup"><span data-stu-id="d272d-151">synchronizationRules</span></span>   |<span data-ttu-id="d272d-152">[synchronizationRule](synchronization-synchronizationrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d272d-152">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="d272d-153">Коллекция правил синхронизации, настроенных для [synchronizationJob](synchronization-synchronizationjob.md) или [synchronizationTemplate](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="d272d-153">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="d272d-154">version</span><span class="sxs-lookup"><span data-stu-id="d272d-154">version</span></span>                |<span data-ttu-id="d272d-155">String</span><span class="sxs-lookup"><span data-stu-id="d272d-155">String</span></span>                             |<span data-ttu-id="d272d-156">Версия схемы, автоматического обновления при каждом изменении схемы.</span><span class="sxs-lookup"><span data-stu-id="d272d-156">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d272d-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d272d-157">JSON representation</span></span>

<span data-ttu-id="d272d-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d272d-158">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
