---
title: Тип ресурса Оффицеклиентчеккинстатус
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df8f1927329a34a51b5f6d8738faec05be01b451
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012004"
---
# <a name="officeclientcheckinstatus-resource-type"></a>Тип ресурса Оффицеклиентчеккинстатус

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, описывающая статистику по возврату клиента.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userPrincipalName|Строка|Имя участника пользователя, использующего устройство.|
|deviceName|String|Имя устройства, пытающееся вернуть.|
|devicePlatform|String|Платформа устройства пытается вернуться.|
|Девицеплатформверсион|String|Версия платформы устройства, пытающаяся вернуть значение.|
|Вассукцессфул|Boolean|, Если последний возврат выполнен успешно.|
|userId|String|Идентификатор пользователя, использующий устройство.|
|Чеккиндатетиме|DateTimeOffset|Время последнего возврата устройства в формате UTC.|
|Ошибк|String|Сообщение об ошибке, если оно связано с последним возвратом.|
|appliedPolicies|Коллекция строк|Список политик, доставляемых на устройство при последнем возврате.|

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



