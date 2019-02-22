---
title: тип перечисления Конфигуратионманажерклиентстате
description: Состояние клиента Configuration Manager
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe8474e6886c1312fde4ce3afde3c3fe0185574c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170702"
---
# <a name="configurationmanagerclientstate-enum-type"></a>тип перечисления Конфигуратионманажерклиентстате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние клиента Configuration Manager

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|нуль|Агент диспетчера конфигурации старше 1806 или не установлен, или это устройство не проверялось в Intune более 30 дней.|
|устанавлива|1,1|Агент Configuration Manager установлен, но он еще не отображается в консоли Configuration Manager. Подождите несколько часов, пока оно не будет обновлено.|
|рабочее|7|Этому устройству удалось успешно вернуть службу Configuration Manager.|
|Инсталлфаилед|8,5|Не удалось установить агент диспетчера конфигураций.|
|Упдатефаилед|-11:00|Ошибка обновления от версии x до версии y агента Configuration Manager. |
|Коммуникатионеррор|19|Агенту диспетчера конфигураций удалось подключиться к службе Configuration Manager ранее, но теперь она больше не может. |




