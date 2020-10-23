---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22d2c3ff02af919ddc2f843e12d4a04aec974c13
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695063"
---
# <a name="certificaterevocationstatus-enum-type"></a>тип перечисления Цертификатеревокатионстатус

Пространство имен: microsoft.graph

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





