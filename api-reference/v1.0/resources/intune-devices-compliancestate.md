---
title: тип из переумыка complianceState
description: Состояние соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b371969e349340264b2a3ccd81ce008a1716b0c3
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60450209"
---
# <a name="compliancestate-enum-type"></a>тип из переумыка complianceState

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние соответствия требованиям.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестно.|
|совместимый|1|Совместимый.|
|нескомплиентные|2|Устройство не соответствует требованиям и блокируется из корпоративных ресурсов.|
|конфликт|3|Конфликт с другими правилами.|
|error|4 |Ошибка|
|inGracePeriod|254|Устройство не соответствует требованиям, но по-прежнему имеет доступ к корпоративным ресурсам|
|configManager|255|Управление менеджером Config|



