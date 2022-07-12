---
title: Тип перечисления windowsUpdateType
description: Какие устройства филиалов будут получать обновления от
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7f1417e59137dd67d0b9c757141e064d909b4c20
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734223"
---
# <a name="windowsupdatetype-enum-type"></a>Тип перечисления windowsUpdateType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Какие устройства филиалов будут получать обновления от

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Разрешить пользователю задавать параметры.|
|все|1|Semi-annual Channel (Targeted). Устройство получает все применимые обновления компонентов из Semi-Annual Channel (Targeted).|
|businessReadyOnly|2|Semi-annual Channel. Устройство получает обновления компонентов из Semi-Annual Channel.|
|windowsInsiderBuildFast|3|Сборка windows За кулисами — быстрая|
|windowsInsiderBuildSlow|4|Сборка За кулисами Windows — медленно|
|windowsInsiderBuildRelease|5|Выпуск сборки Windows За кулисами|





