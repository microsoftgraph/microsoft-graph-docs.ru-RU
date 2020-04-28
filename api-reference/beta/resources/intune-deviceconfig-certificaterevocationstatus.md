---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8d449fc723fd4c3a03c9a72bdbc74768b7db698c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402233"
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
|закончен|1,1|Отзыв ожидается.|
|опубликован|2|Выдана команда отзыва.|
|сбоев|4|Не удалось выполнить отзыв.|
|отозван|4 |Отозван.|



