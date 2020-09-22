---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 916e41c84b2c5ec740522c19b73f0c598f42184f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095102"
---
# <a name="managementagenttype-enum-type"></a>тип перечисления Манажементаженттипе

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип агента управления.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|атрибутов|1 |Управление устройством осуществляется с помощью Exchange Server.|
|Корпоратив|2 |Управление устройством осуществляется с помощью Intune MDM.|
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






