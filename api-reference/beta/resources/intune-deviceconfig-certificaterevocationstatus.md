---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f0e0342924faf166e6daf0a66149e841b88d6d0c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795696"
---
# <a name="certificaterevocationstatus-enum-type"></a>тип перечисления Цертификатеревокатионстатус

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние отзыва сертификата.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|none|нуль|Не отозван.|
|закончен|1,1|Отзыв ожидается.|
|опубликован|2|Выдана команда отзыва.|
|сбоев|4|Не удалось выполнить отзыв.|
|отозван|4 |Отозван.|



