---
title: тип enum vpnServiceExceptionAction
description: Действие VPN для определенной службы.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a43e97e993a9a605aee3561c188bf3a969f0510d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59027080"
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



