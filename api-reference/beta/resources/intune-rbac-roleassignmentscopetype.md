---
title: Тип перечисления roleAssignmentScopeType
description: Указывает тип области для назначения ролей.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b815cf7eb396aa82f49df792ceee0612678077c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419893"
---
# <a name="roleassignmentscopetype-enum-type"></a>Тип перечисления roleAssignmentScopeType

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает тип области для назначения ролей.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|resourceScope|0|Разрешить назначения для указанного ResourceScopes.|
|allDevices|1|Разрешить назначений на все устройства Intune.|
|allLicensedUsers|2|Разрешить назначения для всех пользователей с корпоративным лицензированием Intune.|
|allDevicesAndLicensedUsers|3|Разрешить назначения для всех устройств Intune и лицензированных пользователей.|




