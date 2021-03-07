---
title: тип ресурса printConnector
description: Представляет соединители печати, зарегистрированные с помощью подписки универсальной печати. Ресурс printConnector можно использовать для просмотра состояния соединитетеля и обновления свойств.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: e791ca755b695fc8e4704b65aff98a9db934d901
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517949"
---
# <a name="printconnector-resource-type"></a>тип ресурса printConnector

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет соединители печати, зарегистрированные с помощью подписки универсальной печати. Ресурс printConnector можно использовать для просмотра состояния соединитетеля и обновления свойств.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
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
|location|[printerLocation](printerlocation.md)|Физическое и/или организационное расположение соединитетеля.|
|registeredDateTime|DateTimeOffset|DateTimeOffset при регистрации соединитетеля.|
|registeredBy|[userIdentity](useridentity.md)|Пользователь, зарегистрировавший соединители.|

## <a name="relationships"></a>Отношения
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