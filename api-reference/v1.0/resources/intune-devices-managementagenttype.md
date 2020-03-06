---
title: тип перечисления Манажементаженттипе
description: Тип агента управления.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a5835a0a8ca83cef2d5590679ce8aa4e77b0859
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530289"
---
# <a name="managementagenttype-enum-type"></a>тип перечисления Манажементаженттипе

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип агента управления.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|атрибутов|1 |Управление устройством осуществляется с помощью Exchange Server.|
|Корпоратив|2 |Управление устройством осуществляется с помощью Intune MDM.|
|еасмдм|3 |Устройство управляется как в Exchange Server, так и в Intune MDM.|
|интунеклиент|4 |Управление клиентом Intune.|
|еасинтунеклиент|5 |Устройство — это EAS и двойное управление клиентом Intune.|
|конфигуратионманажерклиент|8 |Управление устройством осуществляется с помощью Configuration Manager.|
|конфигуратионманажерклиентмдм|10 |Управление устройством осуществляется с помощью Configuration Manager и MDM.|
|конфигуратионманажерклиентмдмеас|-11:00|Управление устройством осуществляется с помощью Configuration Manager, MDM и EAS.|
|unknown|16 |Неизвестный тип агента управления.|
|жамф|32|Атрибуты устройства извлекаются из Жамф.|
|гуглеклауддевицеполициконтроллер|64|Управление устройством осуществляется с помощью Клауддпк Google.|




