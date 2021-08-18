---
title: тип enum win32LobAppRestartBehavior
description: Указывает тип действия перезагрузки.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d850410b5380864988b9bd43abed41d9729138dbecd7d11f615da063a2b21c7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54153260"
---
# <a name="win32lobapprestartbehavior-enum-type"></a>тип enum win32LobAppRestartBehavior

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает тип действия перезагрузки.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|basedOnReturnCode|0|Intune перезапустит устройство после запуска установки приложения, если операция возвращает код перезагрузки.|
|разрешить|1 |Intune не будет принимать каких-либо конкретных действий по перезагрузке кодов в результате установки приложений. Intune не будет пытаться подавить перезапуски для приложений MSI.|
|подавление|2|Intune будет пытаться подавить перезапуски для приложений MSI.|
|force|3 |Intune заставит устройство перезапуститься сразу после операции установки приложения.|




