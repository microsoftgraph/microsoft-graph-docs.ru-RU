---
title: dmaGuardDeviceEnumerationPolicyType enum type
description: Возможные значения DmaGuardDeviceEnumerationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f6899594f226c7d5515d79464d9c80e7a90a2f84c40196804e2015fb832369f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124761"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>dmaGuardDeviceEnumerationPolicyType enum type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения DmaGuardDeviceEnumerationPolicy.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Значение по умолчанию. Устройства с dmapping несовместимыми драйверами будут перенацелены только после того, как пользователь откроет экран.|
|blockAll|1 |Устройства с dmapping несовместимыми драйверами никогда не будут разрешены к запуску и выполнению DMA в любое время.|
|allowAll|2|Все внешние устройства PCIe, способные к ДМА, будут в любое время переумещены.|




