---
title: тип перечисления Конфигуратионманажерактионделиверистатус
description: Состояние доставки действия устройства Configuration Manager
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58dca2b1ecb5419a3f56889a55c0816f492af430
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785093"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a>тип перечисления Конфигуратионманажерактионделиверистатус

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



