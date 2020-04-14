---
title: Тип ресурса win32LobAppRestartSettings
description: Содержит свойства, описывающие повторную координацию после установки приложения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e962c9e03a587f0393ddec1fe273be15c6547b22
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471999"
---
# <a name="win32lobapprestartsettings-resource-type"></a>Тип ресурса win32LobAppRestartSettings

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, описывающие повторную координацию после установки приложения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|грацепериодинминутес|Int32|Время ожидания перед перезапуском устройства после установки приложения (в минутах).|
|каунтдовндисплайбефоререстартинминутес|Int32|Время (в минутах) до того, как время перезапуска отображает диалоговое окно обратного отсчета для ожидающих перезапусков.|
|рестартнотификатионснузедуратионинминутес|Int32|Количество минут, в течение которых будет отложиться диалоговое окно уведомления о перезапуске при нажатии кнопки "проложить".|

## <a name="relationships"></a>Отношения
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



