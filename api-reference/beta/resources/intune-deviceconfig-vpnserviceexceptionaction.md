---
title: тип enum vpnServiceExceptionAction
description: Действие VPN для определенной службы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 851292848633b17600228869e305b4504223dc96
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783948"
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
|allowTrafficOutside|1|Разрешить службу за пределами VPN|
|dropTraffic|2|Падение всего трафика из службы|



