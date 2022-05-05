---
title: Тип перечисления zebraFotaNetworkType
description: Представляет различные типы сетей для развертывания Zebra FOTA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9026673271e63ab386ad7a2c16a9fbc276ea52ba
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213563"
---
# <a name="zebrafotanetworktype-enum-type"></a>Тип перечисления zebraFotaNetworkType

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет различные типы сетей для развертывания Zebra FOTA.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|любой|0|Устройство установит обновление независимо от текущего типа сети.|
|Wifi|1|Устройство установит обновление только при подключении к сети Wi-Fi.|
|Сотовой|2|Устройство установит обновление только при подключении сети сотовой связи.|
|wifiAndCellular|3|Устройство установит обновление при подключении Wi-Fi и Сотовой сети.|
|unknownFutureValue|99|Неизвестное значение перечисления в будущем.|




