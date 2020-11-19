---
title: тип перечисления win32LobAppRestartBehavior
description: Указывает тип действия перезапуска.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9632b0199fc3bdc659f4c94fe71311ad2e896ce8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49284563"
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




