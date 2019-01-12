---
title: Тип перечисления managedAppClipboardSharingLevel
description: Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 349f0ee08b8e3bff4e627c58318e2c21fa00847c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946786"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>Тип перечисления managedAppClipboardSharingLevel

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет уровень, на который устройство буфер обмена могут совместно использоваться приложений
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|allApps|0|Общий доступ к может между всем приложениям, управляемых или нет|
|managedAppsWithPasteIn|1|Общий доступ к может между все управляемые приложения с помощью вставки в включено|
|managedApps|2|Общий доступ к может между все управляемые приложения|
|заблокировано|3|Совместное использование приложений отключена|



