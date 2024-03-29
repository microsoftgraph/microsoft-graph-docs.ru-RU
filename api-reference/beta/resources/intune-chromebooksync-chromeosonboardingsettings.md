---
title: тип ресурса chromeOSOnboardingSettings
description: Объект, представляю который представляет параметры клиента Chromebook
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76310cd79a16302c94e9bd2d0c407e82b197683c
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336967"
---
# <a name="chromeosonboardingsettings-resource-type"></a>тип ресурса chromeOSOnboardingSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляю который представляет параметры клиента Chromebook

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список chromeOSOnboardingSettingses](../api/intune-chromebooksync-chromeosonboardingsettings-list.md)|[коллекция chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|Список свойств и связей [объектов chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|
|[Get chromeOSOnboardingSettings](../api/intune-chromebooksync-chromeosonboardingsettings-get.md)|[chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|Чтение свойств и связей [объекта chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|
|[Создание chromeOSOnboardingSettings](../api/intune-chromebooksync-chromeosonboardingsettings-create.md)|[chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|Создайте новый [объект chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|
|[Удаление chromeOSOnboardingSettings](../api/intune-chromebooksync-chromeosonboardingsettings-delete.md)|Нет|Удаляет [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md).|
|[Обновление chromeOSOnboardingSettings](../api/intune-chromebooksync-chromeosonboardingsettings-update.md)|[chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|Обновление свойств объекта [chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|
|[подключение действия](../api/intune-chromebooksync-chromeosonboardingsettings-connect.md)|[chromeOSOnboardingStatus](../resources/intune-chromebooksync-chromeosonboardingstatus.md)|Н/Д|
|[Действие disconnect](../api/intune-chromebooksync-chromeosonboardingsettings-disconnect.md)|[chromeOSOnboardingStatus](../resources/intune-chromebooksync-chromeosonboardingstatus.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id ChromebookTenant|
|ownerUserPrincipalName|String|OwnerUserPrincipalName ChromebookTenant|
|onboardingStatus|[onboardingStatus](../resources/intune-chromebooksync-onboardingstatus.md)|OnboardingStatus ChromebookTenant. Возможные значения: `unknown`, `inprogress`, `onboarded`, `failed`, `offboarding`, `unknownFutureValue`.|
|lastModifiedDateTime|DateTimeOffset|LastModifiedDateTime ChromebookTenant|
|lastDirectorySyncDateTime|DateTimeOffset|LastDirectorySyncDateTime в ChromebookTenant|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chromeOSOnboardingSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "id": "String (identifier)",
  "ownerUserPrincipalName": "String",
  "onboardingStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "lastDirectorySyncDateTime": "String (timestamp)"
}
```




