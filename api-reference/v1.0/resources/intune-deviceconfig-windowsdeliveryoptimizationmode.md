---
title: Тип перечисления windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для однорангового распределения
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a2e05fe9c378f14f1b60a0ac520301010c5ac5c
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730667"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>Тип перечисления windowsDeliveryOptimizationMode

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Режим оптимизации доставки для однорангового распределения

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Разрешить пользователю задавать параметры.|
|httpOnly|1|Только HTTP, без пиринга.|
|httpWithPeeringNat|2|ОС по умолчанию — http с пирингом за тем же переводчиком сетевых адресов|
|httpWithPeeringPrivateGroup|3|HTTP и пиринг в частной группе.|
|httpWithInternetPeering|4|Сочетание HTTP с интернет-пирингом.|
|simpleDownload|99|Режим простого скачивания без пиринга.|
|bypassMode|100|Режим обхода. Не используйте оптимизацию доставки и используйте BITS|





