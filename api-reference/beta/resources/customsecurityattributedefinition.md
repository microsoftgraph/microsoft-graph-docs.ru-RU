---
title: тип ресурса customSecurityAttributeDefinition
description: Объект, который представляет схему настраиваемого атрибута безопасности (пары ключ-значение).
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 390af00d09d2b54fde5bf1cf510ad1752038d3fa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077706"
---
# <a name="customsecurityattributedefinition-resource-type"></a>тип ресурса customSecurityAttributeDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект, который представляет схему настраиваемого атрибута безопасности (пары ключ-значение). Например, имя атрибута настраиваемой безопасности, описание, тип данных и допустимые значения.

В клиенте можно определить до 500 активных объектов. Объект нельзя переименовать или удалить, но его можно отключить с помощью операции `customSecurityAttributeDefiniton` [Update customSecurityAttributeDefinition.](../api/customsecurityattributedefinition-update.md) Должно быть частью набора атрибутов.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список customSecurityAttributeDefinitions](../api/directory-list-customsecurityattributedefinitions.md)|[customSecurityAttributeDefinition collection](../resources/customsecurityattributedefinition.md)|Получите список объектов [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) и их свойств.|
|[Get customSecurityAttributeDefinition](../api/customsecurityattributedefinition-get.md)|[customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md)|Ознакомьтесь с свойствами и отношениями объекта [customSecurityAttributeDefinition.](../resources/customsecurityattributedefinition.md)|
|[Создание customSecurityAttributeDefinition](../api/directory-post-customsecurityattributedefinitions.md)|[customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md)|Создайте новый [объект customSecurityAttributeDefinition.](../resources/customsecurityattributedefinition.md)|
|[Обновление customSecurityAttributeDefinition](../api/customsecurityattributedefinition-update.md)|[customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md)|Обновление свойств объекта [customSecurityAttributeDefinition.](../resources/customsecurityattributedefinition.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|attributeSet|Строка|Имя набора атрибутов. Случай нечувствительный.|
|description|Строка|Описание настраиваемого атрибута безопасности. Может иметь длину до 128 символов и включать символы Unicode. Можно изменить позже.|
|id|String|Идентификатор настраиваемого атрибута безопасности, который является сочетанием имени набора атрибутов и настраиваемого имени атрибута безопасности, разделенного подчеркиваемой `attributeSet` (_ `name` ). Свойство `id` автогенерировано и не может быть установлено. Случай нечувствительный.|
|isCollection|Логическое|Указывает, можно ли наказать несколько значений к настраиваемой атрибуту безопасности. Не удается изменить позже. Если `type` задана настройка Boolean, `isCollection` не может быть задана истина.|
|isSearchable|Логическое|Указывает, будут ли индексироваться пользовательские значения атрибутов безопасности для поиска объектов, за которые назначены значения атрибутов. Не удается изменить позже.|
|name|String|Имя настраиваемого атрибута безопасности. Должно быть уникальным в наборе атрибутов. Может иметь длину до 32 символов и включать символы Unicode. Не может содержать пробелы или специальные символы. Не удается изменить позже. Случай нечувствительный.|
|status|String|Указывает, активен ли настраиваемый атрибут безопасности или отключен. Допустимые значения `Available` и `Deprecated` . Можно изменить позже.|
|type|Строка|Тип данных для пользовательских значений атрибута безопасности. Поддерживаемые типы `Boolean` , `Integer` и `String` . Не удается изменить позже.|
|usePreDefinedValuesOnly|Логическое|Указывает, могут ли быть назначены только предопределяемые значения атрибуту настраиваемой безопасности. Если установлено значение false, разрешены значения свободной формы. Позже может быть изменено с true на false, но не может быть изменено с false на true. Если `type` задана настройка Boolean, `usePreDefinedValuesOnly` не может быть задана истина. |


## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|allowedValues|[коллекция allowedValue](../resources/allowedvalue.md)|Значения, предопределяемые для этого настраиваемой атрибута безопасности.<br><br>Это свойство навигации не возвращается по умолчанию и должно быть указано в `$expand` запросе. Например, `/directory/customSecurityAttributeDefinitions?$expand=allowedValues`.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customSecurityAttributeDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSecurityAttributeDefinition",
  "attributeSet": "String",
  "description": "String",
  "id": "String (identifier)",
  "isCollection": "Boolean",
  "isSearchable": "Boolean",
  "name": "String",
  "status": "String",
  "type": "String",
  "usePreDefinedValuesOnly": "Boolean"
}
```
