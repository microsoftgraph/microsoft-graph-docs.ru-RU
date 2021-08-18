---
title: тип enum vpnServiceExceptionAction
description: Действие VPN для определенной службы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: baf1fa3bf6edcb3358c8ae56d2572365702c41273a04bd578c2c98af5e68d0ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139602"
---
# <a name="vpnserviceexceptionaction-enum-type"></a>тип enum vpnServiceExceptionAction

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Действие VPN для определенной службы.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|forceTrafficViaVPN|0|Чтобы весь трафик из этой службы прошел через VPN|
|allowTrafficOutside|1 |Разрешить службу за пределами VPN|
|dropTraffic|2|Падение всего трафика из службы|




