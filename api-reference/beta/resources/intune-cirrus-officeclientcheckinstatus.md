---
title: тип ресурса officeClientCheckinStatus
description: Объект, описывая статистику регистрации клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bdd2d4f47244bb2eab1e7c357a9f599909166b6a
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52667173"
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
|appliedPolicies|Коллекция строк|Список политик, доставленных на устройство в качестве последней проверки.|

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




