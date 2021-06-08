---
title: тип enum win32LobAppRestartBehavior
description: Указывает тип действия перезагрузки.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bc6ff030c2228ae108e034eea312c57d40b9006f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758969"
---
# <a name="win32lobapprestartbehavior-enum-type"></a>тип enum win32LobAppRestartBehavior

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает тип действия перезагрузки.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|basedOnReturnCode|0|Intune перезапустит устройство после запуска установки приложения, если операция возвращает код перезагрузки.|
|разрешить|1|Intune не будет принимать каких-либо конкретных действий по перезагрузке кодов в результате установки приложений. Intune не будет пытаться подавить перезапуски для приложений MSI.|
|подавление|2|Intune будет пытаться подавить перезапуски для приложений MSI.|
|force|3|Intune заставит устройство перезапуститься сразу после операции установки приложения.|




