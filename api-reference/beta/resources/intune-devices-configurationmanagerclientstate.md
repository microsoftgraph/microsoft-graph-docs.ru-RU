---
title: Тип перечисления configurationManagerClientState
description: Состояние клиента диспетчер конфигурации
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82f4b677001346f9bd32c1bc54bed6e7fbac253d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425787"
---
# <a name="configurationmanagerclientstate-enum-type"></a>Тип перечисления configurationManagerClientState

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние клиента диспетчер конфигурации

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Диспетчер конфигурации агента старше 1806 или не установлена или это устройство не возвращенных в Intune старше 30 дней.|
|установлен|1|Агент диспетчера конфигурации установлен, но может быть отображаются в консоли диспетчера конфигурации еще. Подождите несколько часов для ее обновление.|
|работоспособны|7|Это устройство удалось успешно проверить с помощью службы диспетчера конфигурации.|
|installFailed|8|Не удается установить агент диспетчер конфигурации.|
|updateFailed|11|Не удалось обновить версии x в y версия агента диспетчер конфигурации. |
|communicationError|19|Агент диспетчера конфигурации удалось для доступа к службе Диспетчер конфигурации в прошлом, но теперь больше не является возможность. |




