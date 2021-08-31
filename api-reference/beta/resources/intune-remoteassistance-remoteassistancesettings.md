---
title: тип ресурса remoteAssistanceSettings
description: Параметры удаленной помощи для учетной записи
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 83bd4f0fd4da0f54687dbb1fb378b19e280614f9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58769448"
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
|id|Строка|Идентификатор параметров удаленной помощи|
|remoteAssistanceState|[remoteAssistanceState](../resources/intune-remoteassistance-remoteassistancestate.md)|Текущее состояние удаленной помощи для учетной записи. Возможные значения: неКонфигурационные, отключенные, включенные. Этот параметр настраивается администратором. Параметры удаленной помощи, которые еще не настроены администратором, имеют состояние notConfigured. Возвращается по умолчанию. Возможные значения: `notConfigured`, `disabled`, `enabled`.|
|allowSessionsToUnenrolledDevices|Логический| Указывает, разрешены ли сеансы для незавершенных устройств для учетной записи. Этот параметр настраивается администратором. Значение по умолчанию является ложным.|

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



