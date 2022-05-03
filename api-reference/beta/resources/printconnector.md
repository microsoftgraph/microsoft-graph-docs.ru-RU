---
title: Тип ресурса printConnector
description: Представляет соединитель печати, зарегистрированный с помощью подписки на универсальную печать. Ресурс printConnector можно использовать для просмотра состояния соединителя и обновления свойств.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c482d17cd702751f5f2cd2b8cff5e34166fb2075
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176905"
---
# <a name="printconnector-resource-type"></a>Тип ресурса printConnector

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет соединитель печати, зарегистрированный с помощью подписки на универсальную печать. Ресурс printConnector можно использовать для просмотра состояния соединителя и обновления свойств.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление соединителей](../api/print-list-connectors.md) | [printConnector](printconnector.md) | Получение списка соединителей печати. |
| [Получение соединителя](../api/printconnector-get.md) | [printConnector](printconnector.md) | Чтение свойств и связей объекта соединителя. |
| [Обновление соединителя](../api/printconnector-update.md) | [printConnector](printconnector.md) | Обновите объект соединителя. |
| [Удаление соединителя](../api/printconnector-delete.md) | Нет | Отмените регистрацию соединителя в службе универсальной печати. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения.|
|displayName|Строка|Имя соединителя.|
|fullyQualifiedDomainName|Строка|Имя узла компьютера соединителя.|
|operatingSystem|String|Версия операционной системы компьютера соединителя.|
|appVersion|Строка|Версия соединителя.|
|deviceHealth|[deviceHealth](devicehealth.md)|Работоспособность устройства соединителя.|
|расположение;|[printerLocation](printerlocation.md)|Физическое и (или) организационное расположение соединителя.|
|registeredDateTime|DateTimeOffset|DateTimeOffset, когда был зарегистрирован соединитель.|
|registeredBy|[userIdentity](useridentity.md)|Пользователь, зарегистрировавший соединитель.|

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


