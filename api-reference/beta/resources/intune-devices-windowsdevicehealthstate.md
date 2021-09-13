---
title: тип enum windowsDeviceHealthState
description: Состояние защиты конечной точки компьютера
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5fe5692a8d694076cc060f2c21164fe6a5fe25bb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142987"
---
# <a name="windowsdevicehealthstate-enum-type"></a>тип enum windowsDeviceHealthState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние защиты конечной точки компьютера

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|очистка|0|Компьютер чист, и никаких действий не требуется|
|fullScanPending|1|Компьютер находится в состоянии полной проверки|
|rebootPending|2|Компьютер находится в состоянии ожидания перезагрузки|
|manualStepsPending|4 |Компьютер находится в состоянии ожидания вручную|
|offlineScanPending|8 |Компьютер находится в состоянии автономного сканирования|
|критически важное значение|16 |Компьютер находится в критическом состоянии сбоя|



