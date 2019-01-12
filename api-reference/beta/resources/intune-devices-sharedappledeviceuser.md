---
title: Тип ресурса sharedAppleDeviceUser
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6106daff0b7c4af023c8bfbb8352b52efc674928
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987708"
---
# <a name="sharedappledeviceuser-resource-type"></a>Тип ресурса sharedAppleDeviceUser

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userPrincipalName|Строка|Имя пользователя|
|dataToSync|Логический|Данные для синхронизации|
|dataQuota|Int64|Квота данных|
|dataUsed|Int64|Квота данных|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedAppleDeviceUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
  "userPrincipalName": "String",
  "dataToSync": true,
  "dataQuota": 1024,
  "dataUsed": 1024
}
```





