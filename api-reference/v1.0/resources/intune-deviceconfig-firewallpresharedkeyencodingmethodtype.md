---
title: Тип перечисления firewallPreSharedKeyEncodingMethodType
description: Возможные значения для firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4ad59a11aec2fbf715657de95eb3aafc778da43a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947829"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a>Тип перечисления firewallPreSharedKeyEncodingMethodType

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для firewallPreSharedKeyEncodingMethod
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию|
|Нет|1|Предварительный ключ не кодируются. Вместо этого он будет храниться в формате Юникода|
|utF8|2|Кодирование предварительный ключ, используя UTF-8|



