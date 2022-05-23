---
title: Тип ресурса connectionQuota
description: Представляет квоту подключения, содержащую вычисляемые сведения об использовании квоты внешнего подключения.
author: snlraju-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 68a8015115157bbc7ca12a9851c7386053e2d72a
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629217"
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
| itemsRemaining | Int64 | Минимальное из двух значений: одно представляет элементы, оставшиеся в соединении *, а* остальные элементы на *уровне клиента*. <br/>Следующее уравнение представляет формулу, используемую для вычисления минимального числа:<br/> min (\{_&#65279;_\} \{ максимальной емкости в соединении _—&#65279;_\} число элементов в подключении _,_\} \{\{ квота&#65279;клиента —&#65279;количество элементов, индексированных во всех _подключениях_\}). <br/>Если подключение не монетизировано, например в соединителе предварительной версии или в режиме предварительного просмотра содержимого, это свойство представляет собой просто количество оставшихся элементов в соединении. |

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
