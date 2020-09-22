---
title: Тип ресурса Outofboxexperiencesettings.
description: Настройка "нет на месте"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a258adda7de3a44e33e980fd6e78f7065824ea91
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079908"
---
# <a name="outofboxexperiencesettings-resource-type"></a>Тип ресурса Outofboxexperiencesettings.

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настройка "нет на месте"

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|хидепривацисеттингс|Boolean|Отображение или скрытие параметров конфиденциальности для пользователя|
|хидиула|Boolean|Отображение или скрытие лицензионного соглашения для пользователя|
|userType|[виндовсусертипе](../resources/intune-enrollment-windowsusertype.md)|Тип пользователя. Возможные значения: `administrator`, `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).|Тип проверки подлинности присоединения AAD. Возможные значения: `singleUser`, `shared`.|
|скипкэйбоардселектионпаже|Boolean|Если задано, пропускать страницу "Выбор клавиатуры", если задан язык и регион|
|хидискапелинк|Boolean|Если задано значение true, пользователь не сможет начать с другой учетной записи, при входе в компанию|

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






