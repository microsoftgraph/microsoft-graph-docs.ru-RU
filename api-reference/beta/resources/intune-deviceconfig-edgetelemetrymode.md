---
title: Тип перечисления edgeTelemetryMode
description: Тип просмотра данных, отправляемых Microsoft 365 аналитики
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 81d429f7629a5d6a6f2593785605902065d9f1c7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430740"
---
# <a name="edgetelemetrymode-enum-type"></a>Тип перечисления edgeTelemetryMode

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип просмотра данных, отправляемых Microsoft 365 аналитики

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|По умолчанию — без данных телеметрии собраны или отправки|
|интрасеть|1|Разрешить отправку только журнал интрасети: только отправка, просмотр данных журнала для сайтов интрасети|
|internet|2|Разрешить отправку только журнал Интернета: только отправка, просмотр данных журнала для веб-сайтов|
|intranetAndInternet|3|Разрешить отправку интрасеть и Интернет журнала: отправка, просмотр данных журнала для сайтов Интернета и интрасети|




