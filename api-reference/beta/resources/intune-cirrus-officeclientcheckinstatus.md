---
title: Тип ресурса Оффицеклиентчеккинстатус
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 465b07ba286b9ee3a58132424be2a25b1c7e564e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526701"
---
# <a name="officeclientcheckinstatus-resource-type"></a>Тип ресурса Оффицеклиентчеккинстатус

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, описывающая статистику по возврату клиента.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userPrincipalName|String|Имя участника пользователя, использующего устройство.|
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



