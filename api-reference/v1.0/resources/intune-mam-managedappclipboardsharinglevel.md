---
title: тип enum managedAppClipboardSharingLevel
description: Представляет уровень, на котором буфер обмена данными устройства может быть разделен между приложениями
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b55b58cc0a5c3a514d805e149ace79c3e30f0a89
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457381"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>тип enum managedAppClipboardSharingLevel

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет уровень, на котором буфер обмена данными устройства может быть разделен между приложениями

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|allApps|0|Разрешено совместное использование между всеми приложениями, управляемыми или не управляемыми|
|managedAppsWithPasteIn|1|Разрешен общий доступ между всеми управляемыми приложениями с включенной вклейки|
|managedApps|2|Разрешен общий доступ между всеми управляемыми приложениями|
|заблокировано|3|Совместное использование между приложениями отключено|



