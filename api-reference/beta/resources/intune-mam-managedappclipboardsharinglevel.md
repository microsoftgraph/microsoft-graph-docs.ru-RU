---
title: тип enum managedAppClipboardSharingLevel
description: Представляет уровень, на котором буфер обмена данными устройства может быть разделен между приложениями
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8bf20224470da6d1040befc03ff5eb2ead3db0a0c96a4071ebea34111f922966
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248392"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>тип enum managedAppClipboardSharingLevel

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет уровень, на котором буфер обмена данными устройства может быть разделен между приложениями

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|allApps|0|Разрешено совместное использование между всеми приложениями, управляемыми или не управляемыми|
|managedAppsWithPasteIn|1 |Разрешен общий доступ между всеми управляемыми приложениями с включенной вклейки|
|managedApps|2|Разрешен общий доступ между всеми управляемыми приложениями|
|заблокировано|3 |Совместное использование между приложениями отключено|




