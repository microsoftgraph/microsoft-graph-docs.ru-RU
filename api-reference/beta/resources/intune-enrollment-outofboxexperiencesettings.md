---
title: Тип ресурса outOfBoxExperienceSettings
description: В соответствующем взаимодействия параметр
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d2b48fef00c9c3a291a0a2fdfe680b9f4e21030
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404605"
---
# <a name="outofboxexperiencesettings-resource-type"></a>Тип ресурса outOfBoxExperienceSettings

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В соответствующем взаимодействия параметр

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|hidePrivacySettings|Логический|Показать или скрыть параметры конфиденциальности для пользователя|
|hideEULA|Логический|Показать или скрыть лицензионное соглашение для пользователя|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|Тип пользователя. Возможные значения: `administrator`, `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).|Тип проверки подлинности соединения AAD. Возможные значения: `singleUser`, `shared`.|
|skipKeyboardSelectionPage|Логический|Если набор, а затем пропустить раскладка клавиатуры страницы Если значение языка и региона|
|hideEscapeLink|Логический|Если параметр имеет значение true, затем пользователь не может запуститься через с другой учетной записи для входа в компании|

## <a name="relationships"></a>Отношения
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




