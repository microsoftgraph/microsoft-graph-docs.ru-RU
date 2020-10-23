---
title: Тип ресурса Принтконнектор
description: Представляет соединитель печати, зарегистрированный с помощью универсальной подписки на печать. Ресурс Принтконнектор можно использовать для просмотра состояния соединителя и свойств обновления.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 9962bad290d6a07c214107e58c8a96afb9148394
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727992"
---
# <a name="printconnector-resource-type"></a>Тип ресурса Принтконнектор

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет соединитель печати, зарегистрированный с помощью универсальной подписки на печать. Ресурс Принтконнектор можно использовать для просмотра состояния соединителя и свойств обновления.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение соединителя](../api/printconnector-get.md) | [принтконнектор](printconnector.md) | Считывание свойств и связей объекта Connector. |
| [Соединитель обновления](../api/printconnector-update.md) | [принтконнектор](printconnector.md) | Обновление объекта Connector. |
| [Удаление соединителя](../api/printconnector-delete.md) | Нет | Отмените регистрацию соединителя в универсальной службе печати. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения.|
|displayName|Строка|Имя соединителя.|
|fullyQualifiedDomainName|Строка|Имя узла для соединителя.|
|operatingSystem|String|Версия операционной системы на соединителе компьютера.|
|аппверсион|Строка|Версия соединителя.|
|девицехеалс|[девицехеалс](devicehealth.md)|Работоспособность устройства соединителя.|
|location|[принтерлокатион](printerlocation.md)|Физическое и/или организационное расположение соединителя.|
|регистереддатетиме|DateTimeOffset|Значение DateTimeOffset, когда соединитель был зарегистрирован.|
|регистередби|[userIdentity](useridentity.md)|Пользователь, который зарегистрировал соединитель.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printConnector"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "deviceHealth": {"@odata.type": "microsoft.graph.deviceHealth"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "registeredDateTime": "String (timestamp)",
  "registeredBy": {"@odata.type": "microsoft.graph.userIdentity"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printConnector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


