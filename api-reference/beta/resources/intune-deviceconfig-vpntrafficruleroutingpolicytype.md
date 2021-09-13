---
title: тип enum vpnTrafficRuleRoutingPolicyType
description: Указывает политику маршрутивки для правила трафика VPN.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: be93dbef587a897d10d13b54bddbd738418b12bf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026968"
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



