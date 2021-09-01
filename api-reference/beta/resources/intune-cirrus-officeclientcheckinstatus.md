---
title: тип ресурса officeClientCheckinStatus
description: Объект, описывая статистику регистрации клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae27c35842188bf3e1ce63f0906ab799867ca9a0
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58794986"
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
|devicePlatformVersion|Строка|Версия платформы устройства при попытке регистрации.|
|wasSuccessful|Логический|Если последняя проверка прошла успешно.|
|userId|String|Идентификатор пользователя с помощью устройства.|
|checkinDateTime|DateTimeOffset|Последнее время регистрации устройства в UTC.|
|errorMessage|Строка|Сообщение об ошибке, связанное с последней проверкой.|
|appliedPolicies|Коллекция String|Список политик, доставленных на устройство в качестве последней проверки.|

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



