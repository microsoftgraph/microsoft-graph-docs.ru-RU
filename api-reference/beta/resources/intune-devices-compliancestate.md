---
title: Тип перечисления complianceState
description: Состояние соответствия требованиям.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 04f77da451970a302dbf249e8820aa5a2a8f0ebc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392740"
---
# <a name="compliancestate-enum-type"></a>Тип перечисления complianceState

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние соответствия требованиям.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестно.|
|спецификации|1|Спецификации.|
|несовместимый|2|Устройство не соответствует спецификации и запретом корпоративным ресурсам.|
|конфликта|3|Конфликт с другими правилами.|
|error|4|Ошибка|
|inGracePeriod|254|Устройство, не соответствует спецификации, но по-прежнему имеет доступ к корпоративным ресурсам|
|configManager|255|Управляет диспетчер конфигурации|




