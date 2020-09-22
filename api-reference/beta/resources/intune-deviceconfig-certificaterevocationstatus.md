---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0698e527a75c414b714f9b00f61f2c2f7c036388
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081568"
---
# <a name="certificaterevocationstatus-enum-type"></a>тип перечисления Цертификатеревокатионстатус

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние отзыва сертификата.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|нуль|Не отозван.|
|закончен|1 |Отзыв ожидается.|
|опубликован|2 |Выдана команда отзыва.|
|сбоев|4|Не удалось выполнить отзыв.|
|отозван|4 |Отозван.|






