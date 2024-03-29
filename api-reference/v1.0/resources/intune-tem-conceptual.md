---
title: Управление затратами на телекоммуникации в Microsoft Intune
description: Используя Saaswedo (службу управления затратами на телекоммуникации), которая интегрируется с Intune, вы можете ограничить использование данных и роуминг на корпоративных устройствах. Эта служба позволяет настроить и применить ограничения на использование, а также отправлять пользователям оповещения при превышении настроенного порогового значения. Кроме того, вы можете настроить эту службу на выполнение различных действий, таких как отключение роуминга при превышении порогового значения. Отчеты об использовании данных и сведения о мониторинге доступны в консоли Saaswedo. Прежде чем использовать службу управления затратами на телекоммуникации Saaswedo с Intune, необходимо настроить параметры в консоли Saaswedo и в Intune. Нужно включить соединение как для службы Saaswedo, так и для Intune. Если соединение активировано только со стороны службы Saaswedo, Intune примет соединение, но проигнорирует его.
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 547e0f56f06c83d0913047f2e5aa68b557ad9434
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60444800"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a>Управление затратами на телекоммуникации в Microsoft Intune

Пространство имен: microsoft.graph

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.

Используя Saaswedo (службу управления затратами на телекоммуникации), которая интегрируется с Intune, вы можете ограничить использование данных и роуминг на корпоративных устройствах. Эта служба позволяет настроить и применить ограничения на использование, а также отправлять пользователям оповещения при превышении настроенного порогового значения. Кроме того, вы можете настроить эту службу на выполнение различных действий, таких как отключение роуминга при превышении порогового значения. Отчеты об использовании данных и сведения о мониторинге доступны в консоли Saaswedo. Прежде чем использовать службу управления затратами на телекоммуникации Saaswedo с Intune, необходимо настроить параметры в консоли Saaswedo и в Intune. Нужно включить соединение как для службы Saaswedo, так и для Intune. Если соединение активировано только со стороны службы Saaswedo, Intune примет соединение, но проигнорирует его.

Для управления затратами на телекоммуникации в Intune используются перечисленные ниже ресурсы Graph.  

- [Управление устройствами](intune-tem-devicemanagement.md)
- [Партнер по управлению затратами на телекоммуникации](intune-tem-telecomexpensemanagementpartner.md)
