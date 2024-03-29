---
title: тип ресурса win32LobAppRestartSettings
description: Содержит свойства, описывающие координацию перезапуска после установки приложения.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1db6681ca521224ec99abc36e7058a414e7e7b2c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59051113"
---
# <a name="win32lobapprestartsettings-resource-type"></a>тип ресурса win32LobAppRestartSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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



