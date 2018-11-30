---
title: Тип перечисления windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для распространения peer
ms.openlocfilehash: 99795f3d901b538990d4dfec7a426e66794c5946
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077245"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>Тип перечисления windowsDeliveryOptimizationMode

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Режим оптимизации доставки для распространения peer
## <a name="members"></a>Элементы
|Элемент|Значение|Description|
|:---|:---|:---|
|userDefined|0|Пользователь может задать.|
|httpOnly|1|HTTP, не авторами|
|httpWithPeeringNat|2|Операционная система по умолчанию — Http смешиваются, авторами за же преобразования сетевых адресов|
|httpWithPeeringPrivateGroup|3|HTTP смешиваются, авторами в частной группой|
|httpWithInternetPeering|4|HTTP смешиваются, авторами Интернета|
|simpleDownload|99|Режим простой файл для загрузки с не авторами|
|bypassMode|100|Режим сервера-посредника. Не используйте оптимизации доставки и вместо этого использовать бит|





