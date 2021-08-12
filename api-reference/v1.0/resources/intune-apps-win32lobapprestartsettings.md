---
title: тип ресурса win32LobAppRestartSettings
description: Содержит свойства, описывающие координацию перезапуска после установки приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3f786a52c2a572ccaa1ba1fd7bea9e0c1f6b2358f238144f638c94dc6c48efde
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54175254"
---
# <a name="win32lobapprestartsettings-resource-type"></a>тип ресурса win32LobAppRestartSettings

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, описывающие координацию перезапуска после установки приложения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|gracePeriodInMinutes|Int32|Количество минут, которые необходимо подождать перед перезапуском устройства после установки приложения.|
|countdownDisplayBeforeRestartInMinutes|Int32|Количество минут до начала перезагрузки, чтобы отобразить диалоговое окно обратного отсчета для ожидающих перезапусков.|
|restartNotificationSnoozeDurationInMinutes|Int32|Количество минут, за которые нужно отсмеять диалоговое окно уведомления о перезапуске при выборе кнопки snooze.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRestartSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRestartSettings",
  "gracePeriodInMinutes": 1024,
  "countdownDisplayBeforeRestartInMinutes": 1024,
  "restartNotificationSnoozeDurationInMinutes": 1024
}
```




