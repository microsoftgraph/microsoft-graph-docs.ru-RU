---
title: Тип ресурса Синчронизатионсчема
description: Определяет объекты, которые будут синхронизированы и как они будут синхронизированы. Схема синхронизации содержит большую часть сведений о настройке для определенного задания синхронизации. Как правило, вы настраиваете некоторые сопоставления атрибутов или добавляете фильтр областей для синхронизации только объектов, удовлетворяющих определенному условию.
localization_priority: Normal
ms.openlocfilehash: e7bb91ef473a04552c4c5f33ffc9d54eb86a9b7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453851"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="b20ed-105">Тип ресурса Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="b20ed-105">synchronizationSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b20ed-106">Определяет объекты, которые будут синхронизированы и как они будут синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="b20ed-106">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="b20ed-107">Схема синхронизации содержит большую часть сведений о настройке для определенного задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b20ed-107">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="b20ed-108">Как правило, вы настраиваете некоторые [сопоставления атрибутов](synchronization-attributemapping.md)или добавляете [Фильтр областей](synchronization-filter.md) для синхронизации только объектов, удовлетворяющих определенному условию.</span><span class="sxs-lookup"><span data-stu-id="b20ed-108">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="b20ed-109">В следующих разделах описываются высокоуровневые компоненты схемы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b20ed-109">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="b20ed-110">Определения каталогов</span><span class="sxs-lookup"><span data-stu-id="b20ed-110">Directory definitions</span></span>

<span data-ttu-id="b20ed-111">[Определения каталогов](synchronization-directorydefinition.md) предоставляют обработчику синхронизации сведения о каталогах и их объектах.</span><span class="sxs-lookup"><span data-stu-id="b20ed-111">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="b20ed-112">Например, определение каталога сообщает механизму синхронизации, что каталог Azure AD содержит объекты с именем **User** и **Group**, какие атрибуты поддерживаются для этих объектов, а также типы этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="b20ed-112">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="b20ed-113">Чтобы определенный объект и атрибут можно было использовать в правилах синхронизации/сопоставлениях объектов, они должны быть определены как часть определения каталога.</span><span class="sxs-lookup"><span data-stu-id="b20ed-113">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="b20ed-114">Правила синхронизации</span><span class="sxs-lookup"><span data-stu-id="b20ed-114">Synchronization rules</span></span>

<span data-ttu-id="b20ed-115">[Правила синхронизации](synchronization-synchronizationrule.md) являются ядром настройки синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b20ed-115">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="b20ed-116">Они определяют для обработчика синхронизации, как следует выполнять синхронизацию, в том числе объекты, которые должны быть синхронизированы, как объекты из исходного каталога должны сопоставляться с объектами в целевом каталоге, и как атрибуты должны быть преобразованы при синхронизации из источника в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="b20ed-116">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span> 

## <a name="object-mappings"></a><span data-ttu-id="b20ed-117">Сопоставления объектов</span><span class="sxs-lookup"><span data-stu-id="b20ed-117">Object mappings</span></span>

<span data-ttu-id="b20ed-118">[Сопоставления объектов](synchronization-objectmapping.md) являются основной частью правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b20ed-118">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="b20ed-119">Каждое сопоставление объектов определяет способ синхронизации данного объекта из источника в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="b20ed-119">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="b20ed-120">В частности, сопоставление определяет, как объект в исходном каталоге должен сопоставляться с объектом в целевом каталоге, какие фильтры области (если они есть) следует использовать, чтобы решить, следует ли подготавливать объект и как преобразуются атрибуты объекта. При синхронизации из источника в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="b20ed-120">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="b20ed-121">Методы</span><span class="sxs-lookup"><span data-stu-id="b20ed-121">Methods</span></span>

| <span data-ttu-id="b20ed-122">Метод</span><span class="sxs-lookup"><span data-stu-id="b20ed-122">Method</span></span>        | <span data-ttu-id="b20ed-123">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b20ed-123">Return Type</span></span>               | <span data-ttu-id="b20ed-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b20ed-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="b20ed-125">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="b20ed-125">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="b20ed-126">Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="b20ed-126">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="b20ed-127">Чтение свойств и связей объекта **синчронизатионсчема** .</span><span class="sxs-lookup"><span data-stu-id="b20ed-127">Read properties and relationships of the **synchronizationSchema** object.</span></span>|
|[<span data-ttu-id="b20ed-128">Обновление схемы</span><span class="sxs-lookup"><span data-stu-id="b20ed-128">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="b20ed-129">Нет</span><span class="sxs-lookup"><span data-stu-id="b20ed-129">None</span></span>   |<span data-ttu-id="b20ed-130">Обновите схему синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b20ed-130">Update the synchronization schema.</span></span> |
|[<span data-ttu-id="b20ed-131">Удаление схемы</span><span class="sxs-lookup"><span data-stu-id="b20ed-131">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)    |<span data-ttu-id="b20ed-132">Нет</span><span class="sxs-lookup"><span data-stu-id="b20ed-132">None</span></span>   |<span data-ttu-id="b20ed-133">Удаление настраиваемой схемы путем сброса схемы к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b20ed-133">Delete the customized schema, resetting the schema to the default configuration.</span></span> |
|[<span data-ttu-id="b20ed-134">Операторы фильтра списка</span><span class="sxs-lookup"><span data-stu-id="b20ed-134">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)    |<span data-ttu-id="b20ed-135">Коллекция [филтероператорсчема](../resources/synchronization-filteroperatorschema.md)</span><span class="sxs-lookup"><span data-stu-id="b20ed-135">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) colection</span></span>   |<span data-ttu-id="b20ed-136">ПереЧисление всех операторов, поддерживаемых в фильтрах областей видимости.</span><span class="sxs-lookup"><span data-stu-id="b20ed-136">List all operators supported in the scoping filters.</span></span> |
|[<span data-ttu-id="b20ed-137">Функции сопоставления атрибутов списка</span><span class="sxs-lookup"><span data-stu-id="b20ed-137">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)    |<span data-ttu-id="b20ed-138">Коллекция [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="b20ed-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>   |<span data-ttu-id="b20ed-139">ПереЧисление всех функций, поддерживаемых в выражениях сопоставления атрибутов.</span><span class="sxs-lookup"><span data-stu-id="b20ed-139">List all functions supported in the attribute mapping expressions.</span></span> |
|[<span data-ttu-id="b20ed-140">Анализ выражения сопоставления атрибутов</span><span class="sxs-lookup"><span data-stu-id="b20ed-140">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md)|[<span data-ttu-id="b20ed-141">Парсикспрессионреспонсе</span><span class="sxs-lookup"><span data-stu-id="b20ed-141">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)|<span data-ttu-id="b20ed-142">Синтаксический анализ строкового выражения в объект [Аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="b20ed-142">Parse a string expression into an [attributeMappingSource</span></span>|<span data-ttu-id="b20ed-143">(.. Объект/ресаурцес/синчронизатион_аттрибутемаппингсаурце.МД).</span><span class="sxs-lookup"><span data-stu-id="b20ed-143">(../resources/synchronization_attributemappingsource.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="b20ed-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="b20ed-144">Properties</span></span>

| <span data-ttu-id="b20ed-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="b20ed-145">Property</span></span>      | <span data-ttu-id="b20ed-146">Тип</span><span class="sxs-lookup"><span data-stu-id="b20ed-146">Type</span></span>      | <span data-ttu-id="b20ed-147">Описание</span><span class="sxs-lookup"><span data-stu-id="b20ed-147">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="b20ed-148">каталоги</span><span class="sxs-lookup"><span data-stu-id="b20ed-148">directories</span></span>            |<span data-ttu-id="b20ed-149">Коллекция [директоридефинитион](synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b20ed-149">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="b20ed-150">Описывает каталоги и объекты, входящие в состав [синчронизатионжоб](synchronization-synchronizationjob.md) или [синчронизатионтемплате](synchronization-synchronizationtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="b20ed-150">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="b20ed-151">Синчронизатионрулес</span><span class="sxs-lookup"><span data-stu-id="b20ed-151">synchronizationRules</span></span>   |<span data-ttu-id="b20ed-152">Коллекция [синчронизатионруле](synchronization-synchronizationrule.md)</span><span class="sxs-lookup"><span data-stu-id="b20ed-152">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="b20ed-153">Коллекция правил синхронизации, настроенных для [синчронизатионжоб](synchronization-synchronizationjob.md) или [синчронизатионтемплате](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="b20ed-153">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="b20ed-154">version</span><span class="sxs-lookup"><span data-stu-id="b20ed-154">version</span></span>                |<span data-ttu-id="b20ed-155">String</span><span class="sxs-lookup"><span data-stu-id="b20ed-155">String</span></span>                             |<span data-ttu-id="b20ed-156">Версия схемы, автоматически обновляемая при каждом изменении схемы.</span><span class="sxs-lookup"><span data-stu-id="b20ed-156">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b20ed-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b20ed-157">JSON representation</span></span>

<span data-ttu-id="b20ed-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b20ed-158">The following is a JSON representation of the resource.</span></span>

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
