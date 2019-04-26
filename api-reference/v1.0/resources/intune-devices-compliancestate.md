---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d578417c616fc2dbf30b8fe95d2f58ede5fd3df2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568140"
---
# <a name="compliancestate-enum-type"></a>тип перечисления Комплианцестате

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние соответствия требованиям.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|нуль|Найден.|
|совместимо|1 |Совместимо.|
|несоответствующих|2 |Устройство не совместимо и заблокировано из корпоративных ресурсов.|
|противоречивы|3 |Конфликт с другими правилами.|
|error|4 |Ошибка|
|Инграцепериод|254|Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам|
|Конфигманажер|255|Управление с помощью диспетчера конфигураций|



