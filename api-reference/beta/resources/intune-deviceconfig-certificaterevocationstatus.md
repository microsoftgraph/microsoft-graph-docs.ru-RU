---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 870cf8a59dc2f7a8ae26f3e7a76dd49249b0e008
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526981"
---
# <a name="certificaterevocationstatus-enum-type"></a>тип перечисления Цертификатеревокатионстатус

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние отзыва сертификата.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|нет|нуль|Не отозван.|
|закончен|1 |Отзыв ожидается.|
|опубликован|2 |Выдана команда отзыва.|
|сбоев|3 |Не удалось выполнить отзыв.|
|отозван|4 |Отозван.|



