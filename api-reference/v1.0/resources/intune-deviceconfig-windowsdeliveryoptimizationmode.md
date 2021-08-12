---
title: тип enum windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для одноранговой рассылки
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 59feb6b35d85faa10b816f7d27310b32441ed7298b2202364ce8502d754287ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54223482"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>тип enum windowsDeliveryOptimizationMode

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Режим оптимизации доставки для одноранговой рассылки

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Разрешить пользователю установить.|
|httpOnly|1|ТОЛЬКО HTTP, без одноранговых|
|httpWithPeeringNat|2|По умолчанию ОС — http blended with peering behind the same network address translator|
|httpWithPeeringPrivateGroup|3|HTTP, смешанный с вглядывом в частную группу|
|httpWithInternetPeering|4 |HTTP, смешанный с интернет-пирингом|
|simpleDownload|99|Простой режим загрузки без вглядывок|
|bypassMode|100|Режим обхода. Не используйте оптимизацию доставки и вместо этого используйте BITS|




