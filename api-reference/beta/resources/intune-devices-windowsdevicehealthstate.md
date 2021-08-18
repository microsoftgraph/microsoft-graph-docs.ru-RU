---
title: тип enum windowsDeviceHealthState
description: Состояние защиты конечной точки компьютера
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0372e67f24efe66eb432e5e9d4424940899dc7c294f7b1b1b550f69dc070e113
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227360"
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
|fullScanPending|1 |Компьютер находится в состоянии полной проверки|
|rebootPending|2|Компьютер находится в состоянии ожидания перезагрузки|
|manualStepsPending|4 |Компьютер находится в состоянии ожидания вручную|
|offlineScanPending|8 |Компьютер находится в состоянии автономного сканирования|
|критически важное значение|16 |Компьютер находится в критическом состоянии сбоя|




