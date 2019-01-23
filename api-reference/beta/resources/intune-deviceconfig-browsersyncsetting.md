---
title: Тип перечисления browserSyncSetting
description: Allow(NOT Configured) или prevent(Block) синхронизации параметров браузера Microsoft пограничного сервера. Вариант, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователя.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8dce2b82b1eea5e4b06ed0f6949ba6a403b073a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431680"
---
# <a name="browsersyncsetting-enum-type"></a>Тип перечисления browserSyncSetting

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Allow(NOT Configured) или prevent(Block) синхронизации параметров браузера Microsoft пограничного сервера. Вариант, чтобы запретить синхронизацию между устройствами, но разрешить переопределение пользователя.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Значение по умолчанию — разрешить синхронизацию параметров браузера на устройствах.|
|blockedWithUserOverride|1|Запретить синхронизацию параметров браузера на устройствах пользователей, разрешить переопределение параметров пользователя.|
|заблокировано|2|Абсолютно запретить синхронизацию параметров браузера на устройствах пользователей.|




