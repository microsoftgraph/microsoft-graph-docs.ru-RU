---
title: тип перечисления Конфигуратионманажерактионделиверистатус
description: Состояние доставки действия устройства Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1751f4e53c3df3b3a27d759ff9f747ead5360211
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060694"
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
|пендингделивери|1 |Ожидание для доставки действия в Конфигуратионманажер|
|деливередтоконнекторсервице|2 |Действие отправляется в службу соединителя Конфигуратионманажер (Cloud)|
|фаиледтоделивертоконнекторсервице|4|Не удалось отправить действие службе соединителя Конфигуратионманажер (Cloud)|
|деливередтунпремисессервер|4 |Действие доставляется на локальный сервер Конфигуратионманажер|






