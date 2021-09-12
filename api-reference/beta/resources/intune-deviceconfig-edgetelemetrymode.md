---
title: тип enum edgeTelemetryMode
description: Тип данных просмотра, отправленных в Microsoft 365 аналитики
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0e81e7ccb58db94851e2c56b269dc25050a8c35d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59009177"
---
# <a name="edgetelemetrymode-enum-type"></a>тип enum edgeTelemetryMode

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип данных просмотра, отправленных в Microsoft 365 аналитики

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|По умолчанию — данные телеметрии не собираются и не отправляются|
|интрасеть|1|Разрешить отправку только истории интрасети: только отправлять данные истории просмотра для сайтов интрасети|
|Интернет|2|Разрешить отправку только истории Интернета: отправлять только данные истории просмотра для веб-сайтов|
|intranetAndInternet|3|Разрешить отправку и интрасети, и истории Интернета: отправка данных истории просмотра для интрасети и сайтов в Интернете|



