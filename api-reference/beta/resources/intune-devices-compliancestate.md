---
title: тип из переумыка complianceState
description: Состояние соответствия требованиям.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 051cc43f82dc1ed9a2e1155778eb111387219b86
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111021"
---
# <a name="compliancestate-enum-type"></a>тип из переумыка complianceState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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



