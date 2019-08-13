---
title: Тип ресурса Outofboxexperiencesettings.
description: Настройка "нет на месте"
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0edaa623b080e7b5884b6fe7c3f8817a1c6aecca
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327796"
---
# <a name="outofboxexperiencesettings-resource-type"></a>Тип ресурса Outofboxexperiencesettings.

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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



