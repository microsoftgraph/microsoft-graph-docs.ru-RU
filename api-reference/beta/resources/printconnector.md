---
title: тип ресурса printConnector
description: Представляет соединители печати, зарегистрированные с помощью подписки универсальной печати. Ресурс printConnector можно использовать для просмотра состояния соединитетеля и обновления свойств.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ad4a8f733f39490bbf126d60fe193a664b06888a
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561775"
---
# <a name="printconnector-resource-type"></a>тип ресурса printConnector

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет соединители печати, зарегистрированные с помощью подписки универсальной печати. Ресурс printConnector можно использовать для просмотра состояния соединитетеля и обновления свойств.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление соединителей](../api/print-list-connectors.md) | [printConnector](printconnector.md) | Извлечение списка соединитений печати. |
| [Получение соединителя](../api/printconnector-get.md) | [printConnector](printconnector.md) | Ознакомьтесь с свойствами и отношениями объекта соединители. |
| [Соединители обновления](../api/printconnector-update.md) | [printConnector](printconnector.md) | Обновление объекта соединители. |
| [Удаление соединителя](../api/printconnector-delete.md) | Нет | Unregister the connector from the Universal Print service. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения.|
|displayName|Строка|Имя соединитетеля.|
|fullyQualifiedDomainName|Строка|Имя хост-имени соединители.|
|operatingSystem|String|Версия операционной системы соединитетеля.|
|appVersion|Строка|Версия соединиттеля.|
|deviceHealth|[deviceHealth](devicehealth.md)|Состояние устройства соединиттеля.|
|расположение|[printerLocation](printerlocation.md)|Физическое и/или организационное расположение соединитетеля.|
|registeredDateTime|DateTimeOffset|DateTimeOffset при регистрации соединитетеля.|
|registeredBy|[userIdentity](useridentity.md)|Пользователь, зарегистрировавший соединители.|

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


