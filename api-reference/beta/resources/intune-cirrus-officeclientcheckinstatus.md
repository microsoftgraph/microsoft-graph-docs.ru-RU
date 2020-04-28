---
title: Тип ресурса Оффицеклиентчеккинстатус
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3a2f8bb8728a43187903016ca3417b8e6655b3ab
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471491"
---
# <a name="officeclientcheckinstatus-resource-type"></a>Тип ресурса Оффицеклиентчеккинстатус

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, описывающая статистику по возврату клиента.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userPrincipalName|Строка|Имя участника пользователя, использующего устройство.|
|deviceName|String|Имя устройства, пытающееся вернуть.|
|devicePlatform|String|Платформа устройства пытается вернуться.|
|девицеплатформверсион|String|Версия платформы устройства, пытающаяся вернуть значение.|
|вассукцессфул|Boolean|, Если последний возврат выполнен успешно.|
|userId|String|Идентификатор пользователя, использующий устройство.|
|чеккиндатетиме|DateTimeOffset|Время последнего возврата устройства в формате UTC.|
|Ошибк|String|Сообщение об ошибке, если оно связано с последним возвратом.|
|appliedPolicies|Коллекция объектов string|Список политик, доставляемых на устройство при последнем возврате.|

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



