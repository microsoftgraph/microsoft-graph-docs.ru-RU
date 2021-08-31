---
title: тип enum browserSyncSetting
description: Разрешить (Не настроить) или предотвратить (заблокировать) синхронизацию параметров Microsoft Edge браузера. Возможность предотвратить синхронизацию между устройствами, но разрешить переопределение пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ef97db0168971b687d3dac5fb405f5c9482b2a3d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802784"
---
# <a name="browsersyncsetting-enum-type"></a>тип enum browserSyncSetting

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Разрешить (Не настроить) или предотвратить (заблокировать) синхронизацию параметров Microsoft Edge браузера. Возможность предотвратить синхронизацию между устройствами, но разрешить переопределение пользователя.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|По умолчанию — разрешить синхронизацию параметров браузера на устройствах.|
|blockedWithUserOverride|1|Запретить синхронизацию параметров браузера на устройствах пользователей, разрешить переопределение параметров пользователем.|
|заблокировано|2|Абсолютно запретить синхронизацию параметров браузера на устройствах пользователей.|



