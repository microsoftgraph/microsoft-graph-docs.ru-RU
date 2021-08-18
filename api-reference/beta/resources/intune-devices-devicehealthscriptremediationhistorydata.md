---
title: тип ресурса deviceHealthScriptRemediationHistoryData
description: Количество устройств, исправленных скриптом состояния устройства в заданную дату.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2f88d54cf9e2643c9dab4ef4c1c60e7b0fe7569f242612264dae201aa094375b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206391"
---
# <a name="devicehealthscriptremediationhistorydata-resource-type"></a>тип ресурса deviceHealthScriptRemediationHistoryData

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Количество устройств, исправленных скриптом состояния устройства в заданную дату.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|date|Date|Дата, в которую устройства были исправлены с помощью скрипта состояния устройства.|
|remediatedDeviceCount|Int32|Количество устройств, исправленных скриптом для здоровья устройств.|
|noIssueDeviceCount|Int32|Количество устройств, которые не имеют проблем со сценарием здоровья устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistoryData",
  "date": "String (Date)",
  "remediatedDeviceCount": 1024,
  "noIssueDeviceCount": 1024
}
```




