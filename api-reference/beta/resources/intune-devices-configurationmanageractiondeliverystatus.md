---
title: тип перечисления Конфигуратионманажерактионделиверистатус
description: Состояние доставки действия устройства Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ab437ff9a7945b4bdd61b4e3e3a103e72b780e04
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465123"
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



