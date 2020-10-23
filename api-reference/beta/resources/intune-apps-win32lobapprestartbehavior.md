---
title: тип перечисления win32LobAppRestartBehavior
description: Указывает тип действия перезапуска.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4ce16d0c064fb182352fa0a0061fb2296fd44d7a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706186"
---
# <a name="win32lobapprestartbehavior-enum-type"></a>тип перечисления win32LobAppRestartBehavior

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает тип действия перезапуска.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|баседонретурнкоде|нуль|Intune перезапускает устройство после выполнения установки приложения, если операция возвращает код перезагрузки.|
|разрешить|1,1|Intune не будет предпринимать никаких определенных действий по кодам перезагрузки, полученным в результате установки приложения. Intune не будет пытаться отключить перезапуск для приложений MSI.|
|подавлять|2|Intune попытается отключить перезапуск для приложений MSI.|
|включить|4|Intune вынуждает устройство перезапускать сразу после завершения установки приложения.|





