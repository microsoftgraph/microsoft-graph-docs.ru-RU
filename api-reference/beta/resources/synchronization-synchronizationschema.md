---
title: Тип ресурса Синчронизатионсчема
description: Определяет объекты, которые будут синхронизированы и как они будут синхронизированы.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ffcf6477b806048021fd06c5f21998561798a01b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046739"
---
# <a name="synchronizationschema-resource-type"></a>Тип ресурса Синчронизатионсчема

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет объекты, которые будут синхронизированы и как они будут синхронизированы. Схема синхронизации содержит большую часть сведений о настройке для определенного задания синхронизации. Как правило, вы настраиваете некоторые [сопоставления атрибутов](synchronization-attributemapping.md)или добавляете [Фильтр областей](synchronization-filter.md) для синхронизации только объектов, удовлетворяющих определенному условию.

В следующих разделах описываются высокоуровневые компоненты схемы синхронизации.

## <a name="directory-definitions"></a>Определения каталогов

[Определения каталогов](synchronization-directorydefinition.md) предоставляют обработчику синхронизации сведения о каталогах и их объектах. Например, определение каталога сообщает механизму синхронизации, что каталог Azure AD содержит объекты с именем **User** и **Group**, какие атрибуты поддерживаются для этих объектов, а также типы этих атрибутов. Чтобы определенный объект и атрибут можно было использовать в правилах синхронизации/сопоставлениях объектов, они должны быть определены как часть определения каталога.

## <a name="synchronization-rules"></a>Правила синхронизации

[Правила синхронизации](synchronization-synchronizationrule.md) являются ядром настройки синхронизации. Они определяют для обработчика синхронизации, как следует выполнять синхронизацию, в том числе объекты, которые должны быть синхронизированы, как объекты из исходного каталога должны сопоставляться с объектами в целевом каталоге, а также как преобразуются атрибуты при их синхронизации из источника в целевой каталог.

## <a name="object-mappings"></a>Сопоставления объектов

[Сопоставления объектов](synchronization-objectmapping.md) являются основной частью правила синхронизации. Каждое сопоставление объектов определяет способ синхронизации данного объекта из источника в целевой каталог. В частности, сопоставление определяет, каким образом объект в исходном каталоге должен быть сопоставлен с объектом в целевом каталоге, какие фильтры области (если они есть) следует использовать, чтобы решить, следует ли подготовить объект, а также как должны быть преобразованы атрибуты объекта при синхронизации из источника с целевым каталогом.

## <a name="methods"></a>Методы

| Метод                                                                                                | Возвращаемый тип                                                                                                 | Описание                                                                                                                |
|:------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------|
| [Получение схемы](../api/synchronization-synchronizationschema-get.md)                                     | [синчронизатионсчема](synchronization-synchronizationschema.md)                                           | Чтение свойств и связей объекта **синчронизатионсчема** .                                                 |
| [Обновление схемы](../api/synchronization-synchronizationschema-update.md)                               | Нет                                                                                                        | Обновите схему синхронизации.                                                                                         |
| [Удаление схемы](../api/synchronization-synchronizationschema-delete.md)                               | Нет                                                                                                        | Удаление настраиваемой схемы путем сброса схемы к конфигурации по умолчанию.                                           |
| [Операторы фильтра списка](../api/synchronization-synchronizationschema-filteroperators.md)              | Коллекция [филтероператорсчема](../resources/synchronization-filteroperatorschema.md)                      | Перечисление всех операторов, поддерживаемых в фильтрах областей видимости.                                                                       |
| [Функции сопоставления атрибутов списка](../api/synchronization-synchronizationschema-functions.md)         | Коллекция [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md) | Перечисление всех функций, поддерживаемых в выражениях сопоставления атрибутов.                                                         |
| [Анализ выражения сопоставления атрибутов](../api/synchronization-synchronizationschema-parseexpression.md) | [парсикспрессионреспонсе](synchronization-parseexpressionresponse.md)                                       | Синтаксический анализ строкового выражения в объект [аттрибутемаппингсаурце](../resources/synchronization-attributemappingsource.md) . |


## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|id|Строка|Уникальный идентификатор схемы.|
|синчронизатионрулес   |Коллекция [синчронизатионруле](synchronization-synchronizationrule.md)   |Коллекция правил синхронизации, настроенных для [синчронизатионжоб](synchronization-synchronizationjob.md) или [синчронизатионтемплате](synchronization-synchronizationtemplate.md). |
|version                |String                             |Версия схемы, автоматически обновляемая при каждом изменении схемы.|


## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|каталоги|Коллекция [директоридефинитион](../resources/synchronization-directorydefinition.md)|Содержит коллекцию каталогов и всех их объектов.|

## <a name="json-representation"></a>Представление JSON
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


