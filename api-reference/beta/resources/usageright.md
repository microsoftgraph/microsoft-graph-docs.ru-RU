---
title: Тип ресурса usageRight
description: Содержит сведения об usageRight, назначенного пользователем или устройством
author: jeeshnair
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d3d7ad0de7eb6929e54b7d3d692c6e562e9da76d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130413"
---
# <a name="usageright-resource-type"></a>Тип ресурса usageRight

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Право на использование представляет лицензию, которая есть у пользователя или устройства для сторонних программ, основанных на приложениях питания, или для подписок на устройства (только для устройств).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список user usageRights](../api/user-list-usagerights.md)|Коллекция [usageRight](../resources/usageright.md)|Получите список прав на использование для пользователя.|
|[Список устройств usageRights](../api/device-list-usagerights.md)|Коллекция [usageRight](../resources/usageright.md)|Получите список прав на использование для устройства.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|catalogId|Строка|ИД продукта, соответствующий правом на использование.|
|id|Строка|ИД права на использование.|
|serviceIdentifier|Строка|Идентификатор службы, соответствующей правом на использование.|
|state|usageRightState|Состояние права на использование. Возможные значения: `active`, `inactive`, `warning`, `suspended`.|

### <a name="usagerightstate-values"></a>значения usageRightState 

| Member             |  Описание               |
| :----------------- |  :------------------------ |
|active              | Указывает, что право на использование активно и может использоваться для предоставления преимуществ.|
|неактивный                | Указывает, что право на использование не является активным и не может использоваться для предоставления преимуществ.|
|warning                | Указывает, что право на использование, скорее всего, находится в льготной отсрочке из-за нарушения платежа. Это состояние можно использовать для напоминаия об ожидающих платежах или для ухудшения работы.|
|suspended                | Указывает, что право на использование, скорее всего, приостановлено из-за нарушения платежа|
|unknownFutureValue      | Значение Sentinel, чтобы указать будущие значения. |

>**Примечание.** Преимущества, которые можно получить, представляют только активные состояния и состояния предупреждений. Все остальные состояния должны рассматриваться как не приумещающие преимущества.



## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.usageRight",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.usageRight",
  "id": "String (identifier)",
  "catalogId": "String",
  "serviceIdentifier": "String",
  "state": "String"
}
```

