---
title: тип ресурса outOfBoxExperienceSettings
description: Параметр "Вне параметров работы с полем"
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e0caab818558ef9519b2a107b8c8dbecfe6fc71c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040003"
---
# <a name="outofboxexperiencesettings-resource-type"></a>тип ресурса outOfBoxExperienceSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметр "Вне параметров работы с полем"

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|hidePrivacySettings|Логическое|Показ или сокрытие параметров конфиденциальности пользователю|
|hideEULA|Логический|Показать пользователю или скрыть EULA|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|Тип пользователя. Возможные значения: `administrator`, `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md).|AAD присоединяется к типу проверки подлинности. Возможные значения: `singleUser`, `shared`.|
|skipKeyboardSelectionPage|Логическое|Если установлено, то пропустить страницу выбора клавиатуры, если за установлен язык и область|
|hideEscapeLink|Логическое|Если установлено, что это так, пользователь не может начать все сначала с другой учетной записи при входе в компанию.|

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



