---
title: тип перечисления Еджетелеметримоде
description: Тип данных просмотра, отправляемых в Microsoft 365 Analytics
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b48840debffcc7aedf1454d9cee11b6c0ab9edc1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172473"
---
# <a name="edgetelemetrymode-enum-type"></a>тип перечисления Еджетелеметримоде

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип данных просмотра, отправляемых в Microsoft 365 Analytics

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|нуль|По умолчанию — данные телеметрии не собраны и не отправляются|
|Внутренняя|1,1|Разрешить отправку только журнала интрасети: Отправка только данных журнала браузера для сайтов интрасети|
|internet|2|Разрешить отправку только журнала Интернета: Отправка только данных журнала браузера для Интернет-сайтов|
|Интранетандинтернет|4|Разрешить отправку журнала интрасети и Интернета: отправка данных журнала браузера для интрасети и веб-сайтов|




