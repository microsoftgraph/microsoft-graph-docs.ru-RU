---
title: Тип перечисления windowsUpdateStatus
description: Для бизнеса конфигурации устройства состояний центра обновления Windows
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74493359eeccdbc6df1c351ecec771b5990649b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431744"
---
# <a name="windowsupdatestatus-enum-type"></a>Тип перечисления windowsUpdateStatus

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Для бизнеса конфигурации устройства состояний центра обновления Windows

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|upToDate|0|Отсутствуют ожидающие обновления, не ожидающие обновления перезагрузку и не сбоя обновления.|
|pendingInstallation|1|Существует обновлений, ожидающих установки, включающий обновлений, которые не утверждено. Существует обновления не ожидается перезагрузка, не сбоя обновления.|
|pendingReboot|2|Существует обновлений, которые необходимо перезагрузить компьютер. Не неудачных обновлений.|
|failed|3|Есть обновления не удается установить на устройстве.|




