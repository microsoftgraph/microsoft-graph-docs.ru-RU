---
title: тип enum windowsUpdateType
description: Какие устройства филиала будут получать обновления от
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d052a6f746fb37e936c2eb37126efd31cd74a7d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796855"
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
|все|1|Semi-annual Channel (Targeted). Устройство получает все применимые обновления функций из Semi-annual Channel (Targeted).|
|businessReadyOnly|2|Полугодовой канал. Устройство получает обновления функций из Semi-annual Channel.|
|windowsInsiderBuildFast|3|Windows Сборка инсайдеров — быстрая|
|windowsInsiderBuildSlow|4 |Windows Сборка инсайдеров - Slow|
|windowsInsiderBuildRelease|5 |Сборка Windows insider|



