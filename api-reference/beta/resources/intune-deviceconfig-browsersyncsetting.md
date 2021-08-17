---
title: тип enum browserSyncSetting
description: Разрешить (Не настроить) или предотвратить (заблокировать) синхронизацию параметров Microsoft Edge браузера. Возможность предотвратить синхронизацию между устройствами, но разрешить переопределение пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9ab83353e8192ff62745946cbb40f8297013a959288808b622f0c102e2e3fdcf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54156354"
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
|blockedWithUserOverride|1 |Запретить синхронизацию параметров браузера на устройствах пользователей, разрешить переопределение параметров пользователем.|
|заблокировано|2|Абсолютно запретить синхронизацию параметров браузера на устройствах пользователей.|




