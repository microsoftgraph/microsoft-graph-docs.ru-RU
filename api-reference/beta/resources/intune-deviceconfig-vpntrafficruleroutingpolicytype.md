---
title: тип enum vpnTrafficRuleRoutingPolicyType
description: Указывает политику маршрутивки для правила трафика VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2ae5091563a205c0fb8b3a4d787ca10b5f16a72b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788221"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a>тип enum vpnTrafficRuleRoutingPolicyType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает политику маршрутивки для правила трафика VPN.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Политика маршрутивки не указана.|
|splitTunnel|1|Сетевой трафик указанного приложения будет проходить через VPN.|
|forceTunnel|2|Весь сетевой трафик будет проходить через VPN.|



