---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 34783f2c586e192d62cdeb0018b82e2df100c958
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466245"
---
# <a name="managementagenttype-enum-type"></a>тип перечисления Манажементаженттипе

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип агента управления.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|атрибутов|1,1|Управление устройством осуществляется с помощью Exchange Server.|
|Корпоратив|2|Управление устройством осуществляется с помощью Intune MDM.|
|еасмдм|4|Устройство управляется как в Exchange Server, так и в Intune MDM.|
|интунеклиент|4 |Управление клиентом Intune.|
|еасинтунеклиент|5 |Устройство — это EAS и двойное управление клиентом Intune.|
|конфигуратионманажерклиент|8 |Управление устройством осуществляется с помощью Configuration Manager.|
|конфигуратионманажерклиентмдм|10 |Управление устройством осуществляется с помощью Configuration Manager и MDM.|
|конфигуратионманажерклиентмдмеас|11 |Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.|
|unknown|16 |Неизвестный тип агента управления.|
|жамф|32|Атрибуты устройства извлекаются из Жамф.|
|гуглеклауддевицеполициконтроллер|64|Управление устройством осуществляется с помощью Клауддпк Google.|
|microsoft365ManagedMdm|258|Это устройство управляется Microsoft 365 с помощью Intune.|
|виндовсманажементклаудапи|512|Это устройство управляется Cloud API управления Windows.|



