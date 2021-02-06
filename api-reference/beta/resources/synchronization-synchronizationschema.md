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
# <a name="synchronizationschema-resource-type"></a>Тип ресурса synchronizationSchema

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, какие объекты будут синхронизироваться и как они будут синхронизироваться. Схема синхронизации содержит большую часть сведений об установке для конкретного задания синхронизации. Обычно некоторые сопоставления атрибутов [](synchronization-attributemapping.md)настраиваются или добавляются [](synchronization-filter.md) фильтры области для синхронизации только объектов, удовлетворяющих определенному условию.

В следующих разделах описываются высокоуровневые компоненты схемы синхронизации.

## <a name="directory-definitions"></a>Определения каталогов

[Определения каталогов предоставляют](synchronization-directorydefinition.md) механизм синхронизации сведения о каталогах и их объектах. Например, определение каталога сообщает механизму синхронизации, что каталог Azure AD имеет объекты с именем **user** и **group,** какие атрибуты поддерживаются для этих объектов, а также типы этих атрибутов. Чтобы конкретный объект и атрибут использовались в сопоставлениях правил и объектов синхронизации, их необходимо определить как часть определения каталога.

## <a name="synchronization-rules"></a>Правила синхронизации

[Правила синхронизации](synchronization-synchronizationrule.md) являются основой настройки синхронизации. Они определяют движок синхронизации, как должна выполняться синхронизация, включая объекты, которые должны быть синхронизированы, как объекты из каталога источника должны соединяться с объектами в целевом каталоге и как атрибуты должны преобразовываться при их синхронизации из источника в целевой каталог.

## <a name="object-mappings"></a>Сопоставления объектов

[Сопоставления объектов](synchronization-objectmapping.md) являются основной частью правила синхронизации. Каждое сопоставление объектов определяет, как данный объект должен быть синхронизирован из источника в целевой каталог. В частности, сопоставление определяет, как объект в каталоге источника должен быть сопоставлен с объектом в целевом каталоге, какие (если имеются) фильтры области должны использоваться, чтобы решить, следует ли подготовка объекта и как атрибуты объекта должны преобразовываться при их синхронизации из источника в целевой каталог.

## <a name="methods"></a>Методы

| Метод                                                                                                | Возвращаемый тип                                                                                                 | Описание                                                                                                                |
|:------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------|
| [Получение схемы](../api/synchronization-synchronizationschema-get.md)                                     | [synchronizationSchema](synchronization-synchronizationschema.md)                                           | Чтение свойств и связей объекта **synchronizationSchema.**                                                 |
| [Обновление схемы](../api/synchronization-synchronizationschema-update.md)                               | Нет                                                                                                        | Обновление схемы синхронизации.                                                                                         |
| [Удаление схемы](../api/synchronization-synchronizationschema-delete.md)                               | Нет                                                                                                        | Удалите настроенную схему, сбросив схему до конфигурации по умолчанию.                                           |
| [Список операторов фильтра](../api/synchronization-synchronizationschema-filteroperators.md)              | [Коллекция filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)                      | Список всех операторов, поддерживаемых фильтрами области.                                                                       |
| [Функции сопоставления атрибутов списка](../api/synchronization-synchronizationschema-functions.md)         | [Коллекция attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) | Список всех функций, поддерживаемых выражениями сопоставления атрибутов.                                                         |
| [Выражение сопоставления атрибутов parse](../api/synchronization-synchronizationschema-parseexpression.md) | [parseExpressionResponse](synchronization-parseexpressionresponse.md)                                       | Раз parse a string expression into an [attributeMappingSource](../resources/synchronization-attributemappingsource.md) object. |


## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|id|Строка|Уникальный идентификатор схемы.|
|synchronizationRules   |[Коллекция synchronizationRule](synchronization-synchronizationrule.md)   |Коллекция правил синхронизации, настроенных для [synchronizationJob](synchronization-synchronizationjob.md) или [synchronizationTemplate.](synchronization-synchronizationtemplate.md) |
|version                |String                             |Версия схемы автоматически обновляется при каждом изменении схемы.|


## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|каталоги|[Коллекция directoryDefinition](../resources/synchronization-directorydefinition.md)|Содержит коллекцию каталогов и всех их объектов.|

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
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


