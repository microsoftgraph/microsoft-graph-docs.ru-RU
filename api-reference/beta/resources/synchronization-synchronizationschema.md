---
title: Тип ресурса Синчронизатионсчема
description: Определяет объекты, которые будут синхронизированы и как они будут синхронизированы.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d463fa5a00318936ef0f1612f233851e42a9db11
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846137"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="05792-103">Тип ресурса Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="05792-103">synchronizationSchema resource type</span></span>

<span data-ttu-id="05792-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05792-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05792-105">Определяет объекты, которые будут синхронизированы и как они будут синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="05792-105">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="05792-106">Схема синхронизации содержит большую часть сведений о настройке для определенного задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="05792-106">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="05792-107">Как правило, вы настраиваете некоторые [сопоставления атрибутов](synchronization-attributemapping.md)или добавляете [Фильтр областей](synchronization-filter.md) для синхронизации только объектов, удовлетворяющих определенному условию.</span><span class="sxs-lookup"><span data-stu-id="05792-107">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="05792-108">В следующих разделах описываются высокоуровневые компоненты схемы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="05792-108">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="05792-109">Определения каталогов</span><span class="sxs-lookup"><span data-stu-id="05792-109">Directory definitions</span></span>

<span data-ttu-id="05792-110">[Определения каталогов](synchronization-directorydefinition.md) предоставляют обработчику синхронизации сведения о каталогах и их объектах.</span><span class="sxs-lookup"><span data-stu-id="05792-110">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="05792-111">Например, определение каталога сообщает механизму синхронизации, что каталог Azure AD содержит объекты с именем **User** и **Group**, какие атрибуты поддерживаются для этих объектов, а также типы этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="05792-111">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="05792-112">Чтобы определенный объект и атрибут можно было использовать в правилах синхронизации/сопоставлениях объектов, они должны быть определены как часть определения каталога.</span><span class="sxs-lookup"><span data-stu-id="05792-112">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="05792-113">Правила синхронизации</span><span class="sxs-lookup"><span data-stu-id="05792-113">Synchronization rules</span></span>

<span data-ttu-id="05792-114">[Правила синхронизации](synchronization-synchronizationrule.md) являются ядром настройки синхронизации.</span><span class="sxs-lookup"><span data-stu-id="05792-114">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="05792-115">Они определяют для обработчика синхронизации, как следует выполнять синхронизацию, в том числе объекты, которые должны быть синхронизированы, как объекты из исходного каталога должны сопоставляться с объектами в целевом каталоге, а также как преобразуются атрибуты при их синхронизации из источника в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="05792-115">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="object-mappings"></a><span data-ttu-id="05792-116">Сопоставления объектов</span><span class="sxs-lookup"><span data-stu-id="05792-116">Object mappings</span></span>

<span data-ttu-id="05792-117">[Сопоставления объектов](synchronization-objectmapping.md) являются основной частью правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="05792-117">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="05792-118">Каждое сопоставление объектов определяет способ синхронизации данного объекта из источника в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="05792-118">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="05792-119">В частности, сопоставление определяет, каким образом объект в исходном каталоге должен быть сопоставлен с объектом в целевом каталоге, какие фильтры области (если они есть) следует использовать, чтобы решить, следует ли подготовить объект, а также как должны быть преобразованы атрибуты объекта при синхронизации из источника с целевым каталогом.</span><span class="sxs-lookup"><span data-stu-id="05792-119">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="05792-120">Методы</span><span class="sxs-lookup"><span data-stu-id="05792-120">Methods</span></span>

| <span data-ttu-id="05792-121">Метод</span><span class="sxs-lookup"><span data-stu-id="05792-121">Method</span></span>                                                                                                | <span data-ttu-id="05792-122">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="05792-122">Return Type</span></span>                                                                                                 | <span data-ttu-id="05792-123">Описание</span><span class="sxs-lookup"><span data-stu-id="05792-123">Description</span></span>                                                                                                                |
|:------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------|
| [<span data-ttu-id="05792-124">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="05792-124">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)                                     | [<span data-ttu-id="05792-125">синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="05792-125">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)                                           | <span data-ttu-id="05792-126">Чтение свойств и связей объекта **синчронизатионсчема** .</span><span class="sxs-lookup"><span data-stu-id="05792-126">Read properties and relationships of the **synchronizationSchema** object.</span></span>                                                 |
| [<span data-ttu-id="05792-127">Обновление схемы</span><span class="sxs-lookup"><span data-stu-id="05792-127">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)                               | <span data-ttu-id="05792-128">Нет</span><span class="sxs-lookup"><span data-stu-id="05792-128">None</span></span>                                                                                                        | <span data-ttu-id="05792-129">Обновите схему синхронизации.</span><span class="sxs-lookup"><span data-stu-id="05792-129">Update the synchronization schema.</span></span>                                                                                         |
| [<span data-ttu-id="05792-130">Удаление схемы</span><span class="sxs-lookup"><span data-stu-id="05792-130">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)                               | <span data-ttu-id="05792-131">Нет</span><span class="sxs-lookup"><span data-stu-id="05792-131">None</span></span>                                                                                                        | <span data-ttu-id="05792-132">Удаление настраиваемой схемы путем сброса схемы к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="05792-132">Delete the customized schema, resetting the schema to the default configuration.</span></span>                                           |
| [<span data-ttu-id="05792-133">Операторы фильтра списка</span><span class="sxs-lookup"><span data-stu-id="05792-133">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)              | <span data-ttu-id="05792-134">Коллекция [филтероператорсчема](../resources/synchronization-filteroperatorschema.md)</span><span class="sxs-lookup"><span data-stu-id="05792-134">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection</span></span>                      | <span data-ttu-id="05792-135">Перечисление всех операторов, поддерживаемых в фильтрах областей видимости.</span><span class="sxs-lookup"><span data-stu-id="05792-135">List all operators supported in the scoping filters.</span></span>                                                                       |
| [<span data-ttu-id="05792-136">Функции сопоставления атрибутов списка</span><span class="sxs-lookup"><span data-stu-id="05792-136">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)         | <span data-ttu-id="05792-137">Коллекция [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="05792-137">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span> | <span data-ttu-id="05792-138">Перечисление всех функций, поддерживаемых в выражениях сопоставления атрибутов.</span><span class="sxs-lookup"><span data-stu-id="05792-138">List all functions supported in the attribute mapping expressions.</span></span>                                                         |
| [<span data-ttu-id="05792-139">Анализ выражения сопоставления атрибутов</span><span class="sxs-lookup"><span data-stu-id="05792-139">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md) | [<span data-ttu-id="05792-140">парсикспрессионреспонсе</span><span class="sxs-lookup"><span data-stu-id="05792-140">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)                                       | <span data-ttu-id="05792-141">Синтаксический анализ строкового выражения в объект [аттрибутемаппингсаурце](../resources/synchronization-attributemappingsource.md) .</span><span class="sxs-lookup"><span data-stu-id="05792-141">Parse a string expression into an [attributeMappingSource](../resources/synchronization-attributemappingsource.md) object.</span></span> |


## <a name="properties"></a><span data-ttu-id="05792-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="05792-142">Properties</span></span>

| <span data-ttu-id="05792-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="05792-143">Property</span></span>      | <span data-ttu-id="05792-144">Тип</span><span class="sxs-lookup"><span data-stu-id="05792-144">Type</span></span>      | <span data-ttu-id="05792-145">Описание</span><span class="sxs-lookup"><span data-stu-id="05792-145">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="05792-146">каталоги</span><span class="sxs-lookup"><span data-stu-id="05792-146">directories</span></span>            |<span data-ttu-id="05792-147">Коллекция [директоридефинитион](synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="05792-147">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="05792-148">Описывает каталоги и объекты, входящие в состав [синчронизатионжоб](synchronization-synchronizationjob.md) или [синчронизатионтемплате](synchronization-synchronizationtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="05792-148">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="05792-149">синчронизатионрулес</span><span class="sxs-lookup"><span data-stu-id="05792-149">synchronizationRules</span></span>   |<span data-ttu-id="05792-150">Коллекция [синчронизатионруле](synchronization-synchronizationrule.md)</span><span class="sxs-lookup"><span data-stu-id="05792-150">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="05792-151">Коллекция правил синхронизации, настроенных для [синчронизатионжоб](synchronization-synchronizationjob.md) или [синчронизатионтемплате](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="05792-151">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="05792-152">version</span><span class="sxs-lookup"><span data-stu-id="05792-152">version</span></span>                |<span data-ttu-id="05792-153">String</span><span class="sxs-lookup"><span data-stu-id="05792-153">String</span></span>                             |<span data-ttu-id="05792-154">Версия схемы, автоматически обновляемая при каждом изменении схемы.</span><span class="sxs-lookup"><span data-stu-id="05792-154">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="05792-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05792-155">JSON representation</span></span>

<span data-ttu-id="05792-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05792-156">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
