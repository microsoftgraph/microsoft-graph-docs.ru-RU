---
title: тип enum windowsUpdateType
description: Какие устройства филиала будут получать обновления от
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c49f12452beaf2097381975f40314abbee03ffce
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59015569"
---
# <a name="windowsupdatetype-enum-type"></a>тип enum windowsUpdateType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Какие устройства филиала будут получать обновления от

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Разрешить пользователю установить.|
|все|1|Semi-annual Channel (Targeted). Устройство получает все применимые обновления функций из Semi-annual Channel (Targeted).|
|businessReadyOnly|2|Полугодовой канал. Устройство получает обновления функций из Semi-annual Channel.|
|windowsInsiderBuildFast|3|Windows Сборка инсайдеров — быстрая|
|windowsInsiderBuildSlow|4 |Windows Сборка инсайдеров - Slow|
|windowsInsiderBuildRelease|5 |Сборка Windows insider|




