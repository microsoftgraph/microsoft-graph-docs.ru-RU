---
title: тип enum win32LobAppRestartBehavior
description: Указывает тип действия перезагрузки.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 90eb7ed2c3f7568dfd4a69a4ffab8c52b7d79adb
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60451354"
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



