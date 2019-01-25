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
# <a name="synchronizationschema-resource-type"></a>Тип ресурса synchronizationSchema

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет объекты, которые будут синхронизированы и как они будут синхронизироваться. Схема синхронизации содержит основные сведения об установке для задания синхронизации. Как правило будет настроить некоторые [атрибут сопоставления](synchronization-attributemapping.md)или добавить [области видимости фильтров](synchronization-filter.md) синхронизировать только объекты, удовлетворяющие определенному условию.

В следующих разделах компонентов высокого уровня схемы синхронизации.

## <a name="directory-definitions"></a>Определения каталогов

[Каталог определения](synchronization-directorydefinition.md) обеспечивают синхронизации сведения о каталогах и их объектами. Например определение каталога сообщает обработчик синхронизации, что в каталоге Azure AD объекты с именем **пользователя** и **группы**, какие атрибуты поддерживаются для этих объектов и типы для этих атрибутов. Чтобы определенного объектов и атрибутов для использования в сопоставления правил/объекта синхронизации они должны быть определен как часть определения каталога.

## <a name="synchronization-rules"></a>Правила синхронизации

[Правила синхронизации](synchronization-synchronizationrule.md) — это основной настройки синхронизации. Они подсистемы синхронизации определяют, как выполнять синхронизацию, включая какие объекты должны быть синхронизированы, как объекты из исходного каталога должны совпадать с объектами в целевом каталоге, и как должен быть атрибуты преобразовать их в случае синхронизации из источника в конечный каталог. 

## <a name="object-mappings"></a>Объект сопоставления

[Объект сопоставления](synchronization-objectmapping.md) отличаются основной части правила синхронизации. Сопоставление объектов в каждом определяет, как того или иного объекта должны быть синхронизированы из источника в конечный каталог. В частности, сопоставление определяются как объект в исходный каталог должны совпадать с помощью объекта в целевой каталог, что (если они имеются) области Фильтры следует использовать в том, следует ли предоставить объект и как следует преобразование атрибуты объектов При их в случае синхронизации из источника в конечный каталог.

## <a name="methods"></a>Методы

| Метод        | Возвращаемый тип               | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|[Получение схемы](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |Чтение свойства и связи объекта **synchronizationSchema** .|
|[Схема обновления](../api/synchronization-synchronizationschema-update.md)    |Нет   |Обновление схемы синхронизации. |
|[Удаление схемы](../api/synchronization-synchronizationschema-delete.md)    |Нет   |Удаление настраиваемой схемы, сброс схемы в конфигурации по умолчанию. |
|[Список фильтров операторы](../api/synchronization-synchronizationschema-filteroperators.md)    |[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) коллекции   |Список всех операторы, поддерживаемые в области видимости фильтров. |
|[Атрибут списка сопоставление функций](../api/synchronization-synchronizationschema-functions.md)    |[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) коллекции   |Перечислены все функции, поддерживаемые в выражениях сопоставления атрибута. |
|[Синтаксический анализ выражения сопоставление атрибутов](../api/synchronization-synchronizationschema-parseexpression.md)|[parseExpressionResponse](synchronization-parseexpressionresponse.md)|Синтаксический анализ строковое выражение в [attributeMappingSource|(.. / resources/synchronization_attributemappingsource.md) объекта.|


## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|directories            |[directoryDefinition](synchronization-directorydefinition.md) коллекции   |Описывает каталоги и объекты, которые входят в состав [synchronizationJob](synchronization-synchronizationjob.md) или [synchronizationTemplate](synchronization-synchronizationtemplate.md). |
|synchronizationRules   |[synchronizationRule](synchronization-synchronizationrule.md) коллекции   |Коллекция правил синхронизации, настроенных для [synchronizationJob](synchronization-synchronizationjob.md) или [synchronizationTemplate](synchronization-synchronizationtemplate.md) |
|version                |String                             |Версия схемы, автоматического обновления при каждом изменении схемы.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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
