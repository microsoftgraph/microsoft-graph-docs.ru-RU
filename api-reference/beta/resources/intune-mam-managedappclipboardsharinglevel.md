---
title: тип enum managedAppClipboardSharingLevel
description: Представляет уровень, на котором буфер обмена данными устройства может быть разделен между приложениями
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7b6bc0cb68b28d154d7674246dd305e451623239
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58821103"
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



