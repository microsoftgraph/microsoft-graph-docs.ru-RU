---
title: Тип ресурса Оффицеклиентчеккинстатус
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 647d55e3d5eca6acb47b90092dc0502097b63cf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021765"
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
|devicePlatform|String|Платформа устройства пытается вернуться.|
|девицеплатформверсион|String|Версия платформы устройства, пытающаяся вернуть значение.|
|вассукцессфул|Boolean|, Если последний возврат выполнен успешно.|
|userId|String|Идентификатор пользователя, использующий устройство.|
|чеккиндатетиме|DateTimeOffset|Время последнего возврата устройства в формате UTC.|
|Ошибк|String|Сообщение об ошибке, если оно связано с последним возвратом.|
|appliedPolicies|Коллекция String|Список политик, доставляемых на устройство при последнем возврате.|

## <a name="relationships"></a>Отношения
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






