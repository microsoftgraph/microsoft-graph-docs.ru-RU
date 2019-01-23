---
title: Тип перечисления windowsPrivacyDataAccessLevel
description: Определите уровень доступа к определенной категории конфиденциальности данных Windows.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5d6fed0897b22a6a6b478dc5d2b7954faca42b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410625"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>Тип перечисления windowsPrivacyDataAccessLevel

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определите уровень доступа к определенной категории конфиденциальности данных Windows.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Уровень доступа не указан, не целей. Устройство может работать либо как и UserInControl или ForceAllow. Он может зависеть от конфиденциальности данных были обращении к ним версий Windows и других факторов.|
|forceAllow|1|Приложения смогут получить доступ к данным указанного конфиденциальности.|
|forceDeny|2|Приложения будет запрещен доступ к данным указанного конфиденциальности.|
|userInControl|3|При попытке получить доступ к данным указанного конфиденциальности приложения будет предложено пользователей.|




