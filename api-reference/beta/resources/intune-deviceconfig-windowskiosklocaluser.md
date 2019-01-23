---
title: Тип ресурса windowsKioskLocalUser
description: Класс, используемый для идентификации локальная учетная запись для базовой конфигурации
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b808cdb6cb8bb8540a553104d2c00108341a3e14
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392670"
---
# <a name="windowskiosklocaluser-resource-type"></a>Тип ресурса windowsKioskLocalUser

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, используемый для идентификации локальная учетная запись для базовой конфигурации


Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userName|String|Локальный пользователь, который будет заблокирована этой базовой конфигурации|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```




