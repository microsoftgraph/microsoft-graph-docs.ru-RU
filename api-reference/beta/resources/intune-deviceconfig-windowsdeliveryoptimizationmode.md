---
title: тип enum windowsDeliveryOptimizationMode
description: Режим оптимизации доставки для одноранговой рассылки
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7ee5580f22244b498803d925ca61f4d71f193298
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033632"
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
|httpOnly|1|ТОЛЬКО HTTP, без одноранговых|
|httpWithPeeringNat|2|По умолчанию ОС — http blended with peering behind the same network address translator|
|httpWithPeeringPrivateGroup|3|HTTP, смешанный с вглядывом в частную группу|
|httpWithInternetPeering|4 |HTTP, смешанный с интернет-пирингом|
|simpleDownload|99|Простой режим загрузки без вглядывок|
|bypassMode|100|Режим обхода. Не используйте оптимизацию доставки и вместо этого используйте BITS|



