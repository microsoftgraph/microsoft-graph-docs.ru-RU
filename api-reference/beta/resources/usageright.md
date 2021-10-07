---
title: тип ресурса useRight
description: Содержит сведения об использованииПравить назначенное пользователем или устройством
author: jeeshnair
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e436ad4d793082cbd5c1c8d498b5dbe5b7c7fe54
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214742"
---
# <a name="usageright-resource-type"></a>тип ресурса useRight

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Право на использование представляет лицензию, которую пользователь или устройство имеет для программного обеспечения сторонних Power Apps или для подписки на устройства (только для устройств).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список пользовательских ресурсовRights](../api/user-list-usagerights.md)|Коллекция [usageRight](../resources/usageright.md)|Получите список прав использования для пользователя.|
|[Список использования устройствRights](../api/device-list-usagerights.md)|Коллекция [usageRight](../resources/usageright.md)|Получите список прав использования для устройства.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|catalogId|Строка|ID продукта, соответствующий правому использованию.|
|id|String|ID права использования.|
|serviceIdentifier|Строка|Идентификатор службы, соответствующей правом использования.|
|state|useRightState|Состояние права использования. Возможные значения: `active`, `inactive`, `warning`, `suspended`.|

### <a name="usagerightstate-values"></a>значения useRightState 

| Member             |  Описание               |
| :----------------- |  :------------------------ |
|active              | Указывает, что право на использование является активным и может использоваться для предоставления преимуществ.|
|неактивно                | Указывает, что право на использование не является активным и не может использоваться для предоставления преимуществ.|
|warning                | Указывает, что право использования находится в льготе из-за нарушения платежа. Это состояние можно использовать для напоминать о ожидающих оплате или предлагать деградировавую производительность.|
|suspended                | Указывает, что право на использование приостановлено из-за нарушения платежа|
|unknownFutureValue      | Значение Sentinel, чтобы указать будущие значения. |

>**Примечание:** Только активные и предупреждающие состояния представляют собой полезное преимущество. Ко всем другим состояниям следует относиться как к неугомеримым преимуществам.



## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.usageRight",
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

