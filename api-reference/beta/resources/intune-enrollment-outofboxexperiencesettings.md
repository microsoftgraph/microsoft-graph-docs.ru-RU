---
title: Тип ресурса outOfBoxExperienceSettings
description: В соответствующем взаимодействия параметр
author: tfitzmac
ms.openlocfilehash: 545fbe5c27063397a4d08c40729227804ebfc56d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308409"
---
# <a name="outofboxexperiencesettings-resource-type"></a>Тип ресурса outOfBoxExperienceSettings

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

В соответствующем взаимодействия параметр
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|hidePrivacySettings|Boolean.|Показать или скрыть параметры конфиденциальности для пользователя|
|hideEULA|Boolean.|Показать или скрыть лицензионное соглашение для пользователя|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|Тип пользователя. Возможные значения: `administrator`, `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).|Тип проверки подлинности соединения AAD. Возможные значения: `singleUser`, `shared`.|
|skipKeyboardSelectionPage|Boolean.|Если набор, а затем пропустить раскладка клавиатуры страницы Если значение языка и региона|
|hideEscapeLink|Boolean.|Если параметр имеет значение true, затем пользователь не может запуститься через с другой учетной записи для входа в компании|

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





