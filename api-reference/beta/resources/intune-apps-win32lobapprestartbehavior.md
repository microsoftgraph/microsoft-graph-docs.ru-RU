---
title: тип перечисления win32LobAppRestartBehavior
description: Указывает тип действия перезапуска.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2902f3808ea1ebcc1442b0675c89da51b059f2c2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422641"
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



