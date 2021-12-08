---
title: тип ресурса remoteAssistanceSettings
description: Параметры удаленной помощи для учетной записи
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 26c085a2acfe5299196e3784e9e9ed7b45af35a7
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338108"
---
# <a name="remoteassistancesettings-resource-type"></a>тип ресурса remoteAssistanceSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры удаленной помощи для учетной записи

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get remoteAssistanceSettings](../api/intune-remoteassistance-remoteassistancesettings-get.md)|[remoteAssistanceSettings](../resources/intune-remoteassistance-remoteassistancesettings.md)|Чтение свойств и связей объекта [remoteAssistanceSettings.](../resources/intune-remoteassistance-remoteassistancesettings.md)|
|[Обновление remoteAssistanceSettings](../api/intune-remoteassistance-remoteassistancesettings-update.md)|[remoteAssistanceSettings](../resources/intune-remoteassistance-remoteassistancesettings.md)|Обновление свойств объекта [remoteAssistanceSettings.](../resources/intune-remoteassistance-remoteassistancesettings.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор параметров удаленной помощи|
|remoteAssistanceState|[remoteAssistanceState](../resources/intune-remoteassistance-remoteassistancestate.md)|Текущее состояние удаленной помощи для учетной записи. Возможные значения: отключено, включено. Этот параметр настраивается администратором. Параметры удаленной помощи, которые еще не настроены администратором, отключены. Возвращается по умолчанию. Возможные значения: `disabled`, `enabled`.|
|allowSessionsToUnenrolledDevices|Boolean| Указывает, разрешены ли сеансы для незавершенных устройств для учетной записи. Этот параметр настраивается администратором. Значение по умолчанию является ложным.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistanceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistanceSettings",
  "id": "String (identifier)",
  "remoteAssistanceState": "String",
  "allowSessionsToUnenrolledDevices": true
}
```




