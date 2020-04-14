---
title: Тип ресурса Виндовскиосказуреадусер
description: Класс, используемый для определения учетной записи пользователя AzureAD для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9c1dd759906ec4a4891fdbb2fb57d9c5258aa102
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466780"
---
# <a name="windowskioskazureaduser-resource-type"></a>Тип ресурса Виндовскиосказуреадусер

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, используемый для определения учетной записи пользователя AzureAD для конфигурации киоска


Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userId|String|Идентификатор пользователя AzureAD, который будет заблокирован для этой конфигурации киоска|
|userPrincipalName|String|Учетные записи пользователей, которые будут заблокированы для этой конфигурации киоска|

## <a name="relationships"></a>Отношения
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



