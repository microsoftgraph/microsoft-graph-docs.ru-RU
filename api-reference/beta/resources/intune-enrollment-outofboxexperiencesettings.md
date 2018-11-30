---
title: Тип ресурса outOfBoxExperienceSettings
description: В соответствующем взаимодействия параметр
ms.openlocfilehash: 7d685c7e229828309e2ee759396215c3cd8dfac9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082200"
---
# <a name="outofboxexperiencesettings-resource-type"></a>Тип ресурса outOfBoxExperienceSettings

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

В соответствующем взаимодействия параметр
## <a name="properties"></a>Свойства
|Свойство|Тип|Description|
|:---|:---|:---|
|hidePrivacySettings|Логический|Показать или скрыть параметры конфиденциальности для пользователя|
|hideEULA|Логический|Показать или скрыть лицензионное соглашение для пользователя|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|Тип пользователя. Возможные значения: `administrator`, `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).|Тип проверки подлинности соединения AAD. Возможные значения: `singleUser`, `shared`.|
|skipKeyboardSelectionPage|Логический|Если набор, а затем пропустить раскладка клавиатуры страницы Если значение языка и региона|
|hideEscapeLink|Логический|Если параметр имеет значение true, затем пользователь не может запуститься через с другой учетной записи для входа в компании|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "hidePrivacySettings": true,
  "hideEULA": true,
  "userType": "String",
  "deviceUsageType": "String",
  "skipKeyboardSelectionPage": true,
  "hideEscapeLink": true
}
```





