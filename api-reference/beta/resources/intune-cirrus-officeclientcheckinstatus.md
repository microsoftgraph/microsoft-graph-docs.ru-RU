---
title: тип ресурса officeClientCheckinStatus
description: Объект, описывая статистику регистрации клиента.
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 416b7f20477109718ab8b2efd26190050d910fda
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064429"
---
# <a name="officeclientcheckinstatus-resource-type"></a>тип ресурса officeClientCheckinStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, описывая статистику регистрации клиента.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userPrincipalName|String|Имя основного пользователя с помощью устройства.|
|deviceName|String|Имя устройства при попытке регистрации.|
|devicePlatform|Строка|Платформа устройства, пытаемаяся проверить регистрацию.|
|devicePlatformVersion|String|Версия платформы устройства при попытке регистрации.|
|wasSuccessful|Boolean|Если последняя проверка прошла успешно.|
|userId|String|Идентификатор пользователя с помощью устройства.|
|checkinDateTime|DateTimeOffset|Последнее время регистрации устройства в UTC.|
|errorMessage|Строка|Сообщение об ошибке, связанное с последней проверкой.|
|appliedPolicies|Коллекция строк|Список политик, доставленных на устройство в качестве последней проверки.|

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



