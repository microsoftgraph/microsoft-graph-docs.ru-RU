---
title: тип перечисления Ремотеассистанцеонбоардингстатус
description: Текущее состояние соединителя TeamViewer Connector
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 68e5a8bff7f1753540a2716a00fd9148e188d7ea
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772939"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>тип перечисления Ремотеассистанцеонбоардингстатус

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Текущее состояние соединителя TeamViewer Connector

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|нотонбоардед|нуль|Состояние, указанное при отсутствии активного соединителя TeamViewer Connector, настроенного или активного|
|входящей миграции|1,1|Сведения о состоянии, когда система инициировала подключение TeamViewer, но служба еще не выполнила подтверждение соединителя|
|подключены|2|Состояние, полученное в отчете, когда система успешно выполнила обмен сведениями об учетной записи с TeamViewer, и теперь может инициировать сеансы удаленного помощника с клиентами|



