---
title: тип enum windowsUpdateType
description: Какие устройства филиала будут получать обновления от
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9d6ab79b8d0320a3830948ef1e2973f158338310849618c47b45cbcc9c20253f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244891"
---
# <a name="windowsupdatetype-enum-type"></a>тип enum windowsUpdateType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Какие устройства филиала будут получать обновления от

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Разрешить пользователю установить.|
|все|1 |Semi-annual Channel (Targeted). Устройство получает все применимые обновления функций из Semi-annual Channel (Targeted).|
|businessReadyOnly|2|Полугодовой канал. Устройство получает обновления функций из Semi-annual Channel.|
|windowsInsiderBuildFast|3 |Windows Сборка инсайдеров — быстрая|
|windowsInsiderBuildSlow|4 |Windows Сборка инсайдеров - Slow|
|windowsInsiderBuildRelease|5 |Сборка Windows insider|




