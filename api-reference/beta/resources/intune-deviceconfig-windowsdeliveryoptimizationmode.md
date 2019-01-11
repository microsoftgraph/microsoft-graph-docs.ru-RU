---
title: Тип перечисления windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для распространения peer
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e62416328e596737c36d920d6877773c905680c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807723"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>Тип перечисления windowsDeliveryOptimizationMode

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Режим оптимизации доставки для распространения peer
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Пользователь может задать.|
|httpOnly|1|HTTP, не авторами|
|httpWithPeeringNat|2|Операционная система по умолчанию — Http смешиваются, авторами за же преобразования сетевых адресов|
|httpWithPeeringPrivateGroup|3|HTTP смешиваются, авторами в частной группой|
|httpWithInternetPeering|4|HTTP смешиваются, авторами Интернета|
|simpleDownload|99|Режим простой файл для загрузки с не авторами|
|bypassMode|100|Режим сервера-посредника. Не используйте оптимизации доставки и вместо этого использовать бит|





