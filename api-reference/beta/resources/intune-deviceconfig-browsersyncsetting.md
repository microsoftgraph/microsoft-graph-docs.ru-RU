---
title: тип enum browserSyncSetting
description: Разрешить (Не настроить) или предотвратить (заблокировать) синхронизацию параметров Microsoft Edge браузера. Возможность предотвратить синхронизацию между устройствами, но разрешить переопределение пользователя.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cfaec7d41ae18d12ad4801fdc1110250d6288b62
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127488"
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



