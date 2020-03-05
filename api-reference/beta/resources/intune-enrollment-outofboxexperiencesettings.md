---
title: Тип ресурса Outofboxexperiencesettings.
description: Настройка "нет на месте"
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 65ea22f4a0684fb77b267d7793082ae066af5bd8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528265"
---
# <a name="outofboxexperiencesettings-resource-type"></a>Тип ресурса Outofboxexperiencesettings.

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настройка "нет на месте"

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|хидепривацисеттингс|Логический|Отображение или скрытие параметров конфиденциальности для пользователя|
|хидиула|Логический|Отображение или скрытие лицензионного соглашения для пользователя|
|userType|[виндовсусертипе](../resources/intune-enrollment-windowsusertype.md)|Тип пользователя. Возможные значения: `administrator`, `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).|Тип проверки подлинности присоединения AAD. Возможные значения: `singleUser`, `shared`.|
|скипкэйбоардселектионпаже|Логический|Если задано, пропускать страницу "Выбор клавиатуры", если задан язык и регион|
|хидискапелинк|Логический|Если задано значение true, пользователь не сможет начать с другой учетной записи, при входе в компанию|

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



