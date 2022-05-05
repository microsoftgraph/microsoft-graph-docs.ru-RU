---
title: Тип перечисления zebraFotaUpdateType
description: Представляет различные типы обновлений для развертывания Zebra FOTA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5bd17423e3a158a2010ae0afac18b56e406e1651
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213550"
---
# <a name="zebrafotaupdatetype-enum-type"></a>Тип перечисления zebraFotaUpdateType

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет различные типы обновлений для развертывания Zebra FOTA.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Пользовательские|0|Настраиваемое обновление, в котором пользователь выбирает определенный BSP, версию ОС и номер исправления для обновления.|
|Последнее|1|Последнее выпущенное обновление становится целевой ОС. Последняя версия может обновить устройство до новой версии Android.|
|Авто|2|Устройство всегда ищет последний пакет, доступный в репозитории, и пытается обновить его каждый раз, когда доступен новый пакет. Это продолжается до тех пор, пока администратор не отменит автоматическое обновление.|
|unknownFutureValue|99|Неизвестное значение перечисления в будущем.|




