---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dea5f5a1bb84d139389416990bbbd4bd96ee9eba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060743"
---
# <a name="compliancestate-enum-type"></a>тип перечисления Комплианцестате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние соответствия требованиям.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|нуль|Найден.|
|совместимо|1 |Совместимо.|
|несоответствующих|2 |Устройство не совместимо и заблокировано из корпоративных ресурсов.|
|противоречивы|4|Конфликт с другими правилами.|
|error|4 |Ошибка|
|инграцепериод|254|Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам|
|конфигманажер|255|Управление с помощью диспетчера конфигураций|






