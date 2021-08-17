---
title: тип enum edgeTelemetryMode
description: Тип данных просмотра, отправленных в Microsoft 365 аналитики
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 16efa834cf2a3a8089cd2975cb4f1c539f5114941fc307e3fe8da61dc6e390ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54142052"
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
|интрасеть|1 |Разрешить отправку только истории интрасети: только отправлять данные истории просмотра для сайтов интрасети|
|Интернет|2|Разрешить отправку только истории Интернета: отправлять только данные истории просмотра для веб-сайтов|
|intranetAndInternet|3 |Разрешить отправку и интрасети, и истории Интернета: отправка данных истории просмотра для интрасети и сайтов в Интернете|




