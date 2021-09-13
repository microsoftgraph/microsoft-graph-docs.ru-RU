---
title: тип enum win32LobAppRestartBehavior
description: Указывает тип действия перезагрузки.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 427328f8a7769f2aaac909f1c126d11614a240da
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021689"
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




