---
title: тип enum windowsDeviceHealthState
description: Состояние защиты конечной точки компьютера
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 69323863875fa47d7763c904552b2fcd27dd0ae6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787850"
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



