---
title: dmaGuardDeviceEnumerationPolicyType enum type
description: Возможные значения DmaGuardDeviceEnumerationPolicy.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 66a04e3288d9faaf34a42915ab03e859612e3fe9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59009191"
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
|blockAll|1|Устройства с dmapping несовместимыми драйверами никогда не будут разрешены к запуску и выполнению DMA в любое время.|
|allowAll|2|Все внешние устройства PCIe, способные к ДМА, будут в любое время переумещены.|



