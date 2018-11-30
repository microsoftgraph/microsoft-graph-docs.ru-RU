---
title: Тип перечисления deviceEnrollmentType
description: Возможные способы добавления мобильного устройства для управления.
ms.openlocfilehash: d65c66d47e48f750d515fc6ce43b67b3b27b7238
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024659"
---
# <a name="deviceenrollmenttype-enum-type"></a>Тип перечисления deviceEnrollmentType

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные способы добавления мобильного устройства для управления.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Тип регистрации значения по умолчанию не собираются.|
|userEnrollment|1|Регистрация управляемых пользователя по каналу BYOD.|
|deviceEnrollmentManager|2|Регистрация пользователя с учетной записью диспетчера устройств заявок через Интернет.|
|appleBulkWithUser|3|Регистрация массового Apple с задачей пользователя (DEP, Apple Configurator).|
|appleBulkWithoutUser|4|Apple массового заявок через Интернет без запроса пользователя (Config Mobile DEP конфигуратора Apple).|
|windowsAzureADJoin|5|Присоединение к Windows Azure AD 10.|
|windowsBulkUserless|6|Массовое 10 Windows подачи заявок через ICD с сертификатом.|
|windowsAutoEnrollment|7|Windows 10 автоматической подачи заявок. (Добавление учетной записи работы)|
|windowsBulkAzureDomainJoin|8|Windows 10 в пакетном режиме присоединиться к Azure AD.|
|windowsCoManagement|9|Windows 10 совместного управления, вызванные автопилот или групповой политики.|



