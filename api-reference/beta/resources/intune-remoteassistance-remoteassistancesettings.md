---
title: тип ресурса remoteAssistanceSettings
description: Параметры удаленной помощи для учетной записи
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0179aaeb870c49c89bbb7795a1cc7962011dac68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039457"
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
|remoteAssistanceState|[remoteAssistanceState](../resources/intune-remoteassistance-remoteassistancestate.md)|Текущее состояние удаленной помощи для учетной записи. Возможные значения: неКонфигурационные, отключенные, включенные. Этот параметр настраивается администратором. Параметры удаленной помощи, которые еще не настроены администратором, имеют состояние notConfigured. Возвращается по умолчанию. Возможные значения: `notConfigured`, `disabled`, `enabled`.|
|allowSessionsToUnenrolledDevices|Логическое| Указывает, разрешены ли сеансы для незавершенных устройств для учетной записи. Этот параметр настраивается администратором. Значение по умолчанию является ложным.|

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



