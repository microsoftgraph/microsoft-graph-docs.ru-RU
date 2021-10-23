---
title: тип ресурса printConnector
description: Представляет соединители печати, зарегистрированные с помощью подписки универсальной печати. Ресурс printConnector можно использовать для просмотра состояния соединитетеля и обновления свойств.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: ab2f1718837c88af61e0e790acb2ad198cfded32
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560046"
---
# <a name="printconnector-resource-type"></a>тип ресурса printConnector

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет соединители печати, зарегистрированные с помощью подписки универсальной печати. Ресурс printConnector можно использовать для просмотра состояния соединитетеля и обновления свойств.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Перечисление соединителей](../api/print-list-connectors.md) | [printConnector](printconnector.md) | Извлечение списка соединитений печати. |
| [Получение соединителя](../api/printconnector-get.md) | [printConnector](printconnector.md) | Ознакомьтесь с свойствами и отношениями объекта соединители. |
| [Соединители обновления](../api/printconnector-update.md) | [printConnector](printconnector.md) | Обновление объекта соединители. |
| [Удаление соединителя](../api/printconnector-delete.md) | Нет | Unregister the connector from the Universal Print service. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String| Только для чтения.|
|displayName|Строка|Имя соединитетеля.|
|fullyQualifiedDomainName|Строка|Имя хост-имени соединители.|
|operatingSystem|String|Версия операционной системы соединитетеля.|
|appVersion|Строка|Версия соединиттеля.|
|расположение|[printerLocation](printerlocation.md)|Физическое и/или организационное расположение соединитетеля.|
|registeredDateTime|DateTimeOffset|DateTimeOffset при регистрации соединитетеля.|
|registeredBy|[userIdentity](useridentity.md)|Пользователь, зарегистрировавший соединители.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printConnector",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "registeredDateTime": "String (timestamp)"
}
```
