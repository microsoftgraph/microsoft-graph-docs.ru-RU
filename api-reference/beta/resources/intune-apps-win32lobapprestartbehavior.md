---
title: тип перечисления win32LobAppRestartBehavior
description: Указывает тип действия перезапуска.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e99dde25fb1b57e06cddddc9610a6860a193059
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490317"
---
# <a name="win32lobapprestartbehavior-enum-type"></a>тип перечисления win32LobAppRestartBehavior

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает тип действия перезапуска.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|баседонретурнкоде|нуль|Intune перезапускает устройство после выполнения установки приложения, если операция возвращает код перезагрузки.|
|разрешить|1 |Intune не будет предпринимать никаких определенных действий по кодам перезагрузки, полученным в результате установки приложения. Intune не будет пытаться отключить перезапуск для приложений MSI.|
|подавлять|2 |Intune попытается отключить перезапуск для приложений MSI.|
|включить|3 |Intune вынуждает устройство перезапускать сразу после завершения установки приложения.|



