---
title: Тип перечисления windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для распространения peer
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5565965f9ba9395d7cd07b2935e6772478e0bb50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406887"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>Тип перечисления windowsDeliveryOptimizationMode

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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




