---
title: тип перечисления Конфигуратионманажерактионделиверистатус
description: Состояние доставки действия устройства Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 09c7b1be3a5fdfc33a064d2a9208daa68ba4263e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733988"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a>тип перечисления Конфигуратионманажерактионделиверистатус

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние доставки действия устройства Configuration Manager

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|нуль|Ожидание для доставки действия в Конфигуратионманажер|
|пендингделивери|1,1|Ожидание для доставки действия в Конфигуратионманажер|
|деливередтоконнекторсервице|2|Действие отправляется в службу соединителя Конфигуратионманажер (Cloud)|
|фаиледтоделивертоконнекторсервице|4|Не удалось отправить действие службе соединителя Конфигуратионманажер (Cloud)|
|деливередтунпремисессервер|4 |Действие доставляется на локальный сервер Конфигуратионманажер|





