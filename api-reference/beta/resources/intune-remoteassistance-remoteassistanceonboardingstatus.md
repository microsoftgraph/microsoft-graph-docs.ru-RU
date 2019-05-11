---
title: тип перечисления Ремотеассистанцеонбоардингстатус
description: Текущее состояние соединителя TeamViewer Connector
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8011908e08249d915261208d9615ef627519d40c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940122"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>тип перечисления Ремотеассистанцеонбоардингстатус

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Текущее состояние соединителя TeamViewer Connector

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нотонбоардед|нуль|Состояние, указанное при отсутствии активного соединителя TeamViewer Connector, настроенного или активного|
|входящей миграции|1,1|Сведения о состоянии, когда система инициировала подключение TeamViewer, но служба еще не выполнила подтверждение соединителя|
|подключены|2|Состояние, полученное в отчете, когда система успешно выполнила обмен сведениями об учетной записи с TeamViewer, и теперь может инициировать сеансы удаленного помощника с клиентами|




