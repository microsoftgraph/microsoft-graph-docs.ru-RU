---
title: тип из переумыка complianceState
description: Состояние соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d2b33b8d82f3b6683617247c702219928c2ff2fde7f9fdd73f7b193325e432ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218585"
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




