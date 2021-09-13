---
title: тип enum managedAppClipboardSharingLevel
description: Представляет уровень, на котором буфер обмена данными устройства может быть разделен между приложениями
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b947e0e4f3d81ed843c5e239dbe410594db70b8c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118091"
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




