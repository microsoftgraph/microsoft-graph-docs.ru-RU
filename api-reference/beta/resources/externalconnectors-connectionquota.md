---
title: Тип ресурса connectionQuota
description: Представляет квоту подключения, содержащую вычисляемые сведения об использовании квоты внешнего подключения.
author: josmoran
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 968d0154a1a0bbc5fe33bdcad1123c0944e854fb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316546"
---
# <a name="connectionquota-resource-type"></a>Тип ресурса connectionQuota

Пространство имен: microsoft.graph.externalConnectors

Представляет квоту [подключения,](externalconnectors-externalconnection.md) содержащую вычисляемые сведения об использовании квоты внешнего подключения. Он возвращает допустимое количество элементов, которые можно принимать в соединение, учитывая элементы, принимаемые для подключения, в соответствии с квотой на уровне клиента для соединителей Microsoft Graph.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Получение connectionQuota](../api/externalconnectors-connectionquota-get.md) |[connectionQuota](../resources/externalconnectors-connectionquota.md)| Получение свойств и связей **connectionQuota**. |

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| itemsRemaining | Int64 | Возвращает минимальное число в диапазоне, содержащее следующие данные *: элементы* , оставшиеся в соединении, и *оставшиеся элементы на уровне клиента*. Следующее уравнение представляет формулу, используемую для вычисления минимального числа. `min(max capacity in the connection – number of items in the connection, tenant quota – number of items indexed in all connections)` Если подключение не является монетизированным (соединитель предварительной версии или предварительный просмотр содержимого), оно возвращает количество оставшихся элементов в соединении. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.connectionQuota",
  "openType": false
}
-->

``` json
{
  "itemsRemaining": "Int64"
}
```
