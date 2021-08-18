---
title: тип enum windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для одноранговой рассылки
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6597b76ea76bdfad24f431d98643a487a6fe54256dce20e3afaf6f681b710ea1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227409"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>тип enum windowsDeliveryOptimizationMode

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Режим оптимизации доставки для одноранговой рассылки

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Разрешить пользователю установить.|
|httpOnly|1 |ТОЛЬКО HTTP, без одноранговых|
|httpWithPeeringNat|2|По умолчанию ОС — http blended with peering behind the same network address translator|
|httpWithPeeringPrivateGroup|3 |HTTP, смешанный с вглядывом в частную группу|
|httpWithInternetPeering|4 |HTTP, смешанный с интернет-пирингом|
|simpleDownload|99|Простой режим загрузки без вглядывок|
|bypassMode|100|Режим обхода. Не используйте оптимизацию доставки и вместо этого используйте BITS|




