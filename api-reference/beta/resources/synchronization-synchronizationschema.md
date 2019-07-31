---
title: Тип ресурса Синчронизатионсчема
description: Определяет объекты, которые будут синхронизированы и как они будут синхронизированы. Схема синхронизации содержит большую часть сведений о настройке для определенного задания синхронизации. Как правило, вы настраиваете некоторые сопоставления атрибутов или добавляете фильтр областей для синхронизации только объектов, удовлетворяющих определенному условию.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 95cb2a9bc38b3c23d8ddece5abe5520bf0fe25a8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007783"
---
# <a name="synchronizationschema-resource-type"></a>Тип ресурса Синчронизатионсчема

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет объекты, которые будут синхронизированы и как они будут синхронизированы. Схема синхронизации содержит большую часть сведений о настройке для определенного задания синхронизации. Как правило, вы настраиваете некоторые [сопоставления атрибутов](synchronization-attributemapping.md)или добавляете [Фильтр областей](synchronization-filter.md) для синхронизации только объектов, удовлетворяющих определенному условию.

В следующих разделах описываются высокоуровневые компоненты схемы синхронизации.

## <a name="directory-definitions"></a>Определения каталогов

[Определения каталогов](synchronization-directorydefinition.md) предоставляют обработчику синхронизации сведения о каталогах и их объектах. Например, определение каталога сообщает механизму синхронизации, что каталог Azure AD содержит объекты с именем **User** и **Group**, какие атрибуты поддерживаются для этих объектов, а также типы этих атрибутов. Чтобы определенный объект и атрибут можно было использовать в правилах синхронизации/сопоставлениях объектов, они должны быть определены как часть определения каталога.

## <a name="synchronization-rules"></a>Правила синхронизации

[Правила синхронизации](synchronization-synchronizationrule.md) являются ядром настройки синхронизации. Они определяют для обработчика синхронизации, как следует выполнять синхронизацию, в том числе объекты, которые должны быть синхронизированы, как объекты из исходного каталога должны сопоставляться с объектами в целевом каталоге, и как атрибуты должны быть преобразованы при синхронизации из источника в целевой каталог. 

## <a name="object-mappings"></a>Сопоставления объектов

[Сопоставления объектов](synchronization-objectmapping.md) являются основной частью правила синхронизации. Каждое сопоставление объектов определяет способ синхронизации данного объекта из источника в целевой каталог. В частности, сопоставление определяет, как объект в исходном каталоге должен сопоставляться с объектом в целевом каталоге, какие фильтры области (если они есть) следует использовать, чтобы решить, следует ли подготавливать объект и как преобразуются атрибуты объекта. При синхронизации из источника в целевой каталог.

## <a name="methods"></a>Методы

| Метод        | Возвращаемый тип               | Описание                  |
|:--------------|:--------------------------|:-----------------------------|
|[Получение схемы](../api/synchronization-synchronizationschema-get.md)    |[Синчронизатионсчема](synchronization-synchronizationschema.md)   |Чтение свойств и связей объекта **синчронизатионсчема** .|
|[Обновление схемы](../api/synchronization-synchronizationschema-update.md)    |Нет   |Обновите схему синхронизации. |
|[Удаление схемы](../api/synchronization-synchronizationschema-delete.md)    |Нет   |Удаление настраиваемой схемы путем сброса схемы к конфигурации по умолчанию. |
|[Операторы фильтра списка](../api/synchronization-synchronizationschema-filteroperators.md)    |Коллекция [филтероператорсчема](../resources/synchronization-filteroperatorschema.md)   |Перечисление всех операторов, поддерживаемых в фильтрах областей видимости. |
|[Функции сопоставления атрибутов списка](../api/synchronization-synchronizationschema-functions.md)    |Коллекция [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md)   |Перечисление всех функций, поддерживаемых в выражениях сопоставления атрибутов. |
|[Анализ выражения сопоставления атрибутов](../api/synchronization-synchronizationschema-parseexpression.md)|[Парсикспрессионреспонсе](synchronization-parseexpressionresponse.md)|Синтаксический анализ строкового выражения в объект [Аттрибутемаппингсаурце|(.. Объект/ресаурцес/синчронизатион_аттрибутемаппингсаурце.МД).|


## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|каталоги            |Коллекция [директоридефинитион](synchronization-directorydefinition.md)   |Описывает каталоги и объекты, входящие в состав [синчронизатионжоб](synchronization-synchronizationjob.md) или [синчронизатионтемплате](synchronization-synchronizationtemplate.md). |
|Синчронизатионрулес   |Коллекция [синчронизатионруле](synchronization-synchronizationrule.md)   |Коллекция правил синхронизации, настроенных для [синчронизатионжоб](synchronization-synchronizationjob.md) или [синчронизатионтемплате](synchronization-synchronizationtemplate.md) |
|version                |String                             |Версия схемы, автоматически обновляемая при каждом изменении схемы.|


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
  "suppressions": []
}
-->
