---
title: Тип ресурса Оффицеклиентчеккинстатус
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 014246b973e9ea94ef79eba45c771110dca6da76
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694013"
---
# <a name="officeclientcheckinstatus-resource-type"></a>Тип ресурса Оффицеклиентчеккинстатус

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, описывающая статистику по возврату клиента.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userPrincipalName|String|Имя участника пользователя, использующего устройство.|
|deviceName|String|Имя устройства, пытающееся вернуть.|
|devicePlatform|Строка|Платформа устройства пытается вернуться.|
|девицеплатформверсион|Строка|Версия платформы устройства, пытающаяся вернуть значение.|
|вассукцессфул|Логический|, Если последний возврат выполнен успешно.|
|userId|String|Идентификатор пользователя, использующий устройство.|
|чеккиндатетиме|DateTimeOffset|Время последнего возврата устройства в формате UTC.|
|Ошибк|Строка|Сообщение об ошибке, если оно связано с последним возвратом.|
|appliedPolicies|Коллекция строк|Список политик, доставляемых на устройство при последнем возврате.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```





