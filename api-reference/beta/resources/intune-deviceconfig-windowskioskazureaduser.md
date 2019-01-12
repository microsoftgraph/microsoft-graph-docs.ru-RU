---
title: Тип ресурса windowsKioskAzureADUser
description: Класс, используемый для идентификации учетной записи пользователя в AzureAD для базовой конфигурации
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4497c6d42db45f518e3ef93e78e50d25f473ac00
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984145"
---
# <a name="windowskioskazureaduser-resource-type"></a>Тип ресурса windowsKioskAzureADUser

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Класс, используемый для идентификации учетной записи пользователя в AzureAD для базовой конфигурации

Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userId|String|Идентификатор пользователя AzureAD, который будет заблокирована этой базовой конфигурации|
|userPrincipalName|Строка|Учетные записи пользователей, которые будут заблокированы для этой конфигурации киоска|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```





