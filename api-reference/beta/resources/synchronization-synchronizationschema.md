---
title: Тип ресурса synchronizationSchema
description: Определяет, какие объекты будут синхронизироваться и как они будут синхронизироваться.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: b16e892c44cb69fb5039418a4a246e8b6f32ae9f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131602"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="023cc-103">Тип ресурса synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="023cc-103">synchronizationSchema resource type</span></span>

<span data-ttu-id="023cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="023cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="023cc-105">Определяет, какие объекты будут синхронизироваться и как они будут синхронизироваться.</span><span class="sxs-lookup"><span data-stu-id="023cc-105">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="023cc-106">Схема синхронизации содержит большую часть сведений об установке для конкретного задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="023cc-106">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="023cc-107">Обычно некоторые сопоставления атрибутов [](synchronization-attributemapping.md)настраиваются или добавляются [](synchronization-filter.md) фильтры области для синхронизации только объектов, удовлетворяющих определенному условию.</span><span class="sxs-lookup"><span data-stu-id="023cc-107">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="023cc-108">В следующих разделах описываются высокоуровневые компоненты схемы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="023cc-108">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="023cc-109">Определения каталогов</span><span class="sxs-lookup"><span data-stu-id="023cc-109">Directory definitions</span></span>

<span data-ttu-id="023cc-110">[Определения каталогов предоставляют](synchronization-directorydefinition.md) механизм синхронизации сведения о каталогах и их объектах.</span><span class="sxs-lookup"><span data-stu-id="023cc-110">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="023cc-111">Например, определение каталога сообщает механизму синхронизации, что каталог Azure AD имеет объекты с именем **user** и **group,** какие атрибуты поддерживаются для этих объектов, а также типы этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="023cc-111">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="023cc-112">Чтобы конкретный объект и атрибут использовались в сопоставлениях правил и объектов синхронизации, их необходимо определить как часть определения каталога.</span><span class="sxs-lookup"><span data-stu-id="023cc-112">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="023cc-113">Правила синхронизации</span><span class="sxs-lookup"><span data-stu-id="023cc-113">Synchronization rules</span></span>

<span data-ttu-id="023cc-114">[Правила синхронизации](synchronization-synchronizationrule.md) являются основой настройки синхронизации.</span><span class="sxs-lookup"><span data-stu-id="023cc-114">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="023cc-115">Они определяют движок синхронизации, как должна выполняться синхронизация, включая объекты, которые должны быть синхронизированы, как объекты из каталога источника должны соединяться с объектами в целевом каталоге и как атрибуты должны преобразовываться при их синхронизации из источника в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="023cc-115">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="object-mappings"></a><span data-ttu-id="023cc-116">Сопоставления объектов</span><span class="sxs-lookup"><span data-stu-id="023cc-116">Object mappings</span></span>

<span data-ttu-id="023cc-117">[Сопоставления объектов](synchronization-objectmapping.md) являются основной частью правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="023cc-117">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="023cc-118">Каждое сопоставление объектов определяет, как данный объект должен быть синхронизирован из источника в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="023cc-118">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="023cc-119">В частности, сопоставление определяет, как объект в каталоге источника должен быть сопоставлен с объектом в целевом каталоге, какие (если имеются) фильтры области должны использоваться, чтобы решить, следует ли подготовка объекта и как атрибуты объекта должны преобразовываться при их синхронизации из источника в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="023cc-119">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="023cc-120">Методы</span><span class="sxs-lookup"><span data-stu-id="023cc-120">Methods</span></span>

| <span data-ttu-id="023cc-121">Метод</span><span class="sxs-lookup"><span data-stu-id="023cc-121">Method</span></span>                                                                                                | <span data-ttu-id="023cc-122">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="023cc-122">Return Type</span></span>                                                                                                 | <span data-ttu-id="023cc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="023cc-123">Description</span></span>                                                                                                                |
|:------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------|
| [<span data-ttu-id="023cc-124">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="023cc-124">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)                                     | [<span data-ttu-id="023cc-125">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="023cc-125">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)                                           | <span data-ttu-id="023cc-126">Чтение свойств и связей объекта **synchronizationSchema.**</span><span class="sxs-lookup"><span data-stu-id="023cc-126">Read properties and relationships of the **synchronizationSchema** object.</span></span>                                                 |
| [<span data-ttu-id="023cc-127">Обновление схемы</span><span class="sxs-lookup"><span data-stu-id="023cc-127">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)                               | <span data-ttu-id="023cc-128">Нет</span><span class="sxs-lookup"><span data-stu-id="023cc-128">None</span></span>                                                                                                        | <span data-ttu-id="023cc-129">Обновление схемы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="023cc-129">Update the synchronization schema.</span></span>                                                                                         |
| [<span data-ttu-id="023cc-130">Удаление схемы</span><span class="sxs-lookup"><span data-stu-id="023cc-130">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)                               | <span data-ttu-id="023cc-131">Нет</span><span class="sxs-lookup"><span data-stu-id="023cc-131">None</span></span>                                                                                                        | <span data-ttu-id="023cc-132">Удалите настроенную схему, сбросив схему до конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="023cc-132">Delete the customized schema, resetting the schema to the default configuration.</span></span>                                           |
| [<span data-ttu-id="023cc-133">Список операторов фильтра</span><span class="sxs-lookup"><span data-stu-id="023cc-133">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)              | <span data-ttu-id="023cc-134">[Коллекция filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)</span><span class="sxs-lookup"><span data-stu-id="023cc-134">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection</span></span>                      | <span data-ttu-id="023cc-135">Список всех операторов, поддерживаемых фильтрами области.</span><span class="sxs-lookup"><span data-stu-id="023cc-135">List all operators supported in the scoping filters.</span></span>                                                                       |
| [<span data-ttu-id="023cc-136">Функции сопоставления атрибутов списка</span><span class="sxs-lookup"><span data-stu-id="023cc-136">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)         | <span data-ttu-id="023cc-137">[Коллекция attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="023cc-137">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span> | <span data-ttu-id="023cc-138">Список всех функций, поддерживаемых выражениями сопоставления атрибутов.</span><span class="sxs-lookup"><span data-stu-id="023cc-138">List all functions supported in the attribute mapping expressions.</span></span>                                                         |
| [<span data-ttu-id="023cc-139">Выражение сопоставления атрибутов parse</span><span class="sxs-lookup"><span data-stu-id="023cc-139">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md) | [<span data-ttu-id="023cc-140">parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="023cc-140">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)                                       | <span data-ttu-id="023cc-141">Раз parse a string expression into an [attributeMappingSource](../resources/synchronization-attributemappingsource.md) object.</span><span class="sxs-lookup"><span data-stu-id="023cc-141">Parse a string expression into an [attributeMappingSource](../resources/synchronization-attributemappingsource.md) object.</span></span> |


## <a name="properties"></a><span data-ttu-id="023cc-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="023cc-142">Properties</span></span>

| <span data-ttu-id="023cc-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="023cc-143">Property</span></span>      | <span data-ttu-id="023cc-144">Тип</span><span class="sxs-lookup"><span data-stu-id="023cc-144">Type</span></span>      | <span data-ttu-id="023cc-145">Описание</span><span class="sxs-lookup"><span data-stu-id="023cc-145">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="023cc-146">id</span><span class="sxs-lookup"><span data-stu-id="023cc-146">id</span></span>|<span data-ttu-id="023cc-147">Строка</span><span class="sxs-lookup"><span data-stu-id="023cc-147">String</span></span>|<span data-ttu-id="023cc-148">Уникальный идентификатор схемы.</span><span class="sxs-lookup"><span data-stu-id="023cc-148">Unique identifier for the schema.</span></span>|
|<span data-ttu-id="023cc-149">synchronizationRules</span><span class="sxs-lookup"><span data-stu-id="023cc-149">synchronizationRules</span></span>   |<span data-ttu-id="023cc-150">[Коллекция synchronizationRule](synchronization-synchronizationrule.md)</span><span class="sxs-lookup"><span data-stu-id="023cc-150">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="023cc-151">Коллекция правил синхронизации, настроенных для [synchronizationJob](synchronization-synchronizationjob.md) или [synchronizationTemplate.](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="023cc-151">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="023cc-152">version</span><span class="sxs-lookup"><span data-stu-id="023cc-152">version</span></span>                |<span data-ttu-id="023cc-153">String</span><span class="sxs-lookup"><span data-stu-id="023cc-153">String</span></span>                             |<span data-ttu-id="023cc-154">Версия схемы автоматически обновляется при каждом изменении схемы.</span><span class="sxs-lookup"><span data-stu-id="023cc-154">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="relationships"></a><span data-ttu-id="023cc-155">Связи</span><span class="sxs-lookup"><span data-stu-id="023cc-155">Relationships</span></span>
|<span data-ttu-id="023cc-156">Связь</span><span class="sxs-lookup"><span data-stu-id="023cc-156">Relationship</span></span>|<span data-ttu-id="023cc-157">Тип</span><span class="sxs-lookup"><span data-stu-id="023cc-157">Type</span></span>|<span data-ttu-id="023cc-158">Описание</span><span class="sxs-lookup"><span data-stu-id="023cc-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="023cc-159">каталоги</span><span class="sxs-lookup"><span data-stu-id="023cc-159">directories</span></span>|<span data-ttu-id="023cc-160">[Коллекция directoryDefinition](../resources/synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="023cc-160">[directoryDefinition](../resources/synchronization-directorydefinition.md) collection</span></span>|<span data-ttu-id="023cc-161">Содержит коллекцию каталогов и всех их объектов.</span><span class="sxs-lookup"><span data-stu-id="023cc-161">Contains the collection of directories and all of their objects.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="023cc-162">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="023cc-162">JSON representation</span></span>
<span data-ttu-id="023cc-163">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="023cc-163">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationSchema",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationSchema",
  "id": "String (identifier)",
  "synchronizationRules": [
    {
      "@odata.type": "microsoft.graph.synchronizationRule"
    }
  ],
  "version": "String"
}
```


