---
title: тип ресурса печати
description: В сопровождении подписки универсальной печати функция Print позволяет управлять принтерами и открывать печатные точки, которые можно использовать для управления принтерами и заданиями печати в Universal Print.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7ed4858a167a87be40ff31e540d402fa93a44cbd30f6ee6e67e63ed52510b9fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129990"
---
# <a name="print-resource-type"></a>тип ресурса печати

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

В сопровождении подписки универсальной печати функция Print позволяет управлять принтерами и открывать печатные [точки,](printserviceendpoint.md) которые можно использовать для управления принтерами и заданиями печати в Universal Print.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Перечисление соединителей](../api/print-list-connectors.md) | [коллекция printConnector](printconnector.md) | Получите список соединители печати. |
| [Перечисление принтеров](../api/print-list-printers.md) | [коллекция принтеров](printer.md) | Получите список принтеров. |
| [Перечисление общих ресурсов](../api/print-list-shares.md) | [коллекция printerShare](printershare.md) | Получите список акций принтера. |
| [Службы списка](../api/print-list-services.md) | [коллекция printService](printservice.md) | Получите список служб. |
| [Создание printerShare](../api/print-post-shares.md) | [printerShare](printershare.md) | Создайте новую долю принтера, разместив в **коллекции акций.** |
| [Создание принтера](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Создание (регистрация) нового принтера с универсальной печатью. |
| [Обновление параметров](../api/print-update-settings.md) |  [printSettings](printsettings.md) | Обновляет параметры для службы универсальной печати для клиента. |
| [Перечисление taskDefinitions](../api/print-list-taskdefinitions.md) | [printTaskDefinition collection](printtaskdefinition.md) | Получите список распечатокTaskDefinitions, созданных в универсальной печати. |
| [Создание taskDefinition](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Создайте новый шрифтTaskDefinition. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settings|[printSettings](../resources/printsettings.md)|Параметры для службы универсальной печати для клиента.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|службы|[коллекция printService](printservice.md)|Список доступных конечных точек службы универсальной печати.|
|принтеры|[коллекция принтеров](printer.md)|Список принтеров, зарегистрированных в клиенте.|
|shares|[коллекция printerShare](printershare.md)|Список акций принтера, зарегистрированных в клиенте.|
|соединители|[коллекция printConnector](printconnector.md)|Список доступных соединители печати.|
|operations|[коллекция printOperation](../resources/printoperation.md)|Список длительных операций печати.|
|службы|[коллекция printService](../resources/printservice.md)|Список экземпляров служб печати для различных компонентов инфраструктуры печати.|
|taskDefinitions|[printTaskDefinition collection](../resources/printtaskdefinition.md)|Список абстрактного определения задачи, которая может быть вызвана при различных событиях, происходящих в универсальной печати.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.print",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.print",
  "settings": {
    "@odata.type": "microsoft.graph.printSettings"
  }
}
```

