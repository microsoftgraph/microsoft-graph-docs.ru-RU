---
title: тип enum managedAppClipboardSharingLevel
description: Представляет уровень, на котором буфер обмена данными устройства может быть разделен между приложениями
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e8c3ba5b99b6f416e77ec41d51439fb3b6550370
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075146"
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
|managedAppsWithPasteIn|1|Разрешен общий доступ между всеми управляемыми приложениями с включенной вклейки|
|managedApps|2|Разрешен общий доступ между всеми управляемыми приложениями|
|заблокировано|3|Совместное использование между приложениями отключено|



