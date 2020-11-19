---
title: тип перечисления Ремотеассистанцеонбоардингстатус
description: Текущее состояние соединителя TeamViewer Connector
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ccb04964c7608c24ec8822bac7832aaf77bdfd7f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287790"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>тип перечисления Ремотеассистанцеонбоардингстатус

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Текущее состояние соединителя TeamViewer Connector

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|нотонбоардед|нуль|Состояние, указанное при отсутствии активного соединителя TeamViewer Connector, настроенного или активного|
|входящей миграции|1,1|Сведения о состоянии, когда система инициировала подключение TeamViewer, но служба еще не выполнила подтверждение соединителя|
|подключены|2|Состояние, полученное в отчете, когда система успешно выполнила обмен сведениями об учетной записи с TeamViewer, и теперь может инициировать сеансы удаленного помощника с клиентами|




