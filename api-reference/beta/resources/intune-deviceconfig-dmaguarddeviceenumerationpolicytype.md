---
title: Тип перечисления dmaGuardDeviceEnumerationPolicyType
description: Возможные значения DmaGuardDeviceEnumerationPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5baa0cfd5c80f954036e10f0e4d04d2b83e57f2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430778"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>Тип перечисления dmaGuardDeviceEnumerationPolicyType

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения DmaGuardDeviceEnumerationPolicy.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Значение по умолчанию. Устройства с DMA сопоставление несовместимые драйверы будут перечислены только после пользователь разблокирует экрана.|
|blockAll|1|Устройства с DMA сопоставление драйверы, несовместимые с никогда не смогут запуск и выполнение DMA в любое время.|
|allowAll|2|Все внешние DMA PCIe устройств с поддержкой будут перечислены в любое время.|




