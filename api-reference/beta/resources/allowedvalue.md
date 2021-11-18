---
title: допустимый тип ресурса
description: Предварительное значение, разрешенное для настраиваемой определения атрибута безопасности.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 21e6b1836ae23e1cc6b7c78053ff458ac934087e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077561"
---
# <a name="allowedvalue-resource-type"></a>допустимый тип ресурса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предварительное значение, разрешенное для настраиваемой определения атрибута безопасности.

В настраиваемой `allowedValue` [БезопасностиAttributeDefinition](customsecurityattributedefinition.md)можно определить до 100 объектов. Этот объект нельзя переименовать или удалить, но его можно отключить с помощью операции [Update allowedValue.](../api/../api/allowedvalue-update.md) Этот объект определяется как свойство навигации на [ресурсе customSecurityAttributeDefinition](customsecurityattributedefinition.md) и его значение возвращается только на `$expand` .

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список разрешеноValues](../api/customsecurityattributedefinition-list-allowedvalues.md)|[коллекция allowedValue](../resources/allowedvalue.md)|Получите список разрешенных [объектовValue](../resources/allowedvalue.md) и их свойств.|
|[Get allowedValue](../api/allowedvalue-get.md)|[allowedValue](../resources/allowedvalue.md)|Ознакомьтесь с свойствами и отношениями объекта [allowedValue.](../resources/allowedvalue.md)|
|[Создание allowedValue](../api/customsecurityattributedefinition-post-allowedvalues.md)|[allowedValue](../resources/allowedvalue.md)|Создайте новый [объект allowedValue.](../resources/allowedvalue.md)|
|[Обновление allowedValue](../api/allowedvalue-update.md)|[allowedValue](../resources/allowedvalue.md)|Обновление свойств объекта [allowedValue.](../resources/allowedvalue.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| id | Строка | Идентификатор для предопределяемой величины. Может иметь длину до 64 символов и включать символы Unicode. Может включать пробелы, но некоторые специальные символы не допускаются. Не удается изменить позже. Деликатный. |
|isActive|Логическое|Указывает, активна ли заранее заранее активная или деактивированная величина. Если установлено значение, это предварительное значение не может быть назначено дополнительным поддерживаемым `false` объектам каталога.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.allowedValue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.allowedValue",
  "id": "String (identifier)",
  "isActive": "Boolean"
}
```
