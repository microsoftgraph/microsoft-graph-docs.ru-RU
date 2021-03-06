---
title: 'Управление затратами на телекоммуникации в Microsoft Intune : API Microsoft Graph'
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), связанных с управлением затратами на телекоммуникации для организации клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 471bd6315c35b713bb022cc9872f96ac70fcd050
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159474"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a>Управление затратами на телекоммуникации в Microsoft Intune

Пространство имен: microsoft.graph

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Используя Saaswedo (службу управления затратами на телекоммуникации), которая интегрируется с Intune, вы можете ограничить использование данных и роуминг на корпоративных устройствах. Эта служба позволяет настроить и применить ограничения на использование, а также отправлять пользователям оповещения при превышении настроенного порогового значения. Кроме того, вы можете настроить эту службу на выполнение различных действий, таких как отключение роуминга при превышении порогового значения. Отчеты об использовании данных и сведения о мониторинге доступны в консоли Saaswedo. Прежде чем использовать службу управления затратами на телекоммуникации Saaswedo с Intune, необходимо настроить параметры в консоли Saaswedo и в Intune. Нужно включить соединение как для службы Saaswedo, так и для Intune. Если соединение активировано только со стороны службы Saaswedo, Intune примет соединение, но проигнорирует его.

Для управления затратами на телекоммуникации в Intune используются перечисленные ниже ресурсы Graph.

- [Партнер по управлению затратами на телекоммуникации](intune-tem-telecomexpensemanagementpartner.md)