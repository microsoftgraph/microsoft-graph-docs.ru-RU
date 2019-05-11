---
title: Тип ресурса Outofboxexperiencesettings.
description: Настройка "нет на месте"
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb8a3c0358343a3d1051258188028ffa5c1f0293
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941501"
---
# <a name="outofboxexperiencesettings-resource-type"></a>Тип ресурса Outofboxexperiencesettings.

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настройка "нет на месте"

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Хидепривацисеттингс|Логический|Отображение или скрытие параметров конфиденциальности для пользователя|
|Хидиула|Логический|Отображение или скрытие ЛИЦЕНЗИОНного соглашения для пользователя|
|userType|[Виндовсусертипе](../resources/intune-enrollment-windowsusertype.md)|Тип пользователя. Возможные значения: `administrator`, `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).|Тип проверки подлинности присоединения AAD. Возможные значения: `singleUser`, `shared`.|
|Скипкэйбоардселектионпаже|Логический|Если задано, пропускать страницу "Выбор клавиатуры", если задан язык и регион|
|Хидискапелинк|Логический|Если задано значение true, пользователь не сможет начать с другой учетной записи, при входе в компанию|

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




