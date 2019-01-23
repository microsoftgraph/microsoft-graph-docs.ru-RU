---
title: Тип перечисления deviceEnrollmentType
description: Возможные способы добавления мобильного устройства для управления.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aed1f40604a765b1a434bca35dbb356e65e8ccd5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399292"
---
# <a name="deviceenrollmenttype-enum-type"></a>Тип перечисления deviceEnrollmentType

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные способы добавления мобильного устройства для управления.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Тип регистрации значения по умолчанию не собираются.|
|userEnrollment|1|Регистрация управляемых пользователя по каналу BYOD.|
|deviceEnrollmentManager|2|Регистрация пользователя с учетной записью диспетчера устройств заявок через Интернет.|
|appleBulkWithUser|3|Регистрация массового Apple с запрос пользователя. (DEP конфигуратора Apple)|
|appleBulkWithoutUser|4|Apple массового заявок через Интернет без запроса пользователя. (DEP конфигуратора Apple мобильных Config)|
|windowsAzureADJoin|5|Присоединение к Windows Azure AD 10.|
|windowsBulkUserless|6|Массовое 10 Windows подачи заявок через ICD с сертификатом.|
|windowsAutoEnrollment|7|Windows 10 автоматической подачи заявок. (Добавление учетной записи работы)|
|windowsBulkAzureDomainJoin|8|Windows 10 в пакетном режиме присоединиться к Azure AD.|
|windowsCoManagement|9|10 совместного управления Windows активировать по автопилот или групповой политики.|




