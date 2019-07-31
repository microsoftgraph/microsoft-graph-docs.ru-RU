---
title: Тип ресурса Outofboxexperiencesettings.
description: Настройка "нет на месте"
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 32336a0bc73c7d36ee4763dccbdc8a24197833ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999061"
---
# <a name="outofboxexperiencesettings-resource-type"></a>Тип ресурса Outofboxexperiencesettings.

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настройка "нет на месте"

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Хидепривацисеттингс|Boolean|Отображение или скрытие параметров конфиденциальности для пользователя|
|Хидиула|Boolean|Отображение или скрытие лицензионного соглашения для пользователя|
|userType|[Виндовсусертипе](../resources/intune-enrollment-windowsusertype.md)|Тип пользователя. Возможные значения: `administrator`, `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).|Тип проверки подлинности присоединения AAD. Возможные значения: `singleUser`, `shared`.|
|Скипкэйбоардселектионпаже|Boolean|Если задано, пропускать страницу "Выбор клавиатуры", если задан язык и регион|
|Хидискапелинк|Boolean|Если задано значение true, пользователь не сможет начать с другой учетной записи, при входе в компанию|

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





