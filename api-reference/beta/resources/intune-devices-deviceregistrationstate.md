---
title: Тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 90f2dc7f8c11940fa01047d8c61f23c8f0389ed8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396758"
---
# <a name="deviceregistrationstate-enum-type"></a>Тип перечисления deviceRegistrationState

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние регистрации устройства.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notRegistered|0|Устройство не зарегистрирован.|
|зарегистрирована|2|Зарегистрированные устройства.|
|отменено|3|Устройства был заблокирован, очистить или не поддерживается.|
|keyConflict|4|Устройство имеет конфликты ключа.|
|approvalPending|5|Устройство ожидает утверждения.|
|certificateReset|6|Устройство сертификат был изменен.|
|notRegisteredPendingEnrollment|7|Устройства не зарегистрирована и ожидающие заявок через Интернет.|
|unknown|8|Состояние регистрации устройства неизвестно.|




