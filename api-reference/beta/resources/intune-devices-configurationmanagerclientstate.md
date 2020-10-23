---
title: тип перечисления Конфигуратионманажерклиентстате
description: Состояние клиента Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: de8f2af7c6d35b28154f00a4eac3bb20a4bdf64d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690233"
---
# <a name="configurationmanagerclientstate-enum-type"></a>тип перечисления Конфигуратионманажерклиентстате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние клиента Configuration Manager

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|нуль|Агент диспетчера конфигурации старше 1806 или не установлен, или это устройство не проверялось в Intune более 30 дней.|
|устанавлива|1,1|Агент Configuration Manager установлен, но он еще не отображается в консоли Configuration Manager. Подождите несколько часов, пока оно не будет обновлено.|
|рабочее|7 |Этому устройству удалось успешно вернуть службу Configuration Manager.|
|инсталлфаилед|8 |Не удалось установить агент диспетчера конфигураций.|
|упдатефаилед|-11:00|Ошибка обновления от версии x до версии y агента Configuration Manager. |
|коммуникатионеррор|19|Агенту диспетчера конфигураций удалось подключиться к службе Configuration Manager ранее, но теперь она больше не может. |





