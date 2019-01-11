---
title: Тип перечисления appLockerApplicationControlType
description: Возможные значения элемента управления типов AppLocker приложений
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 241387f34a64b4b58d974fc21e2aa5d3af696736
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871983"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>Тип перечисления appLockerApplicationControlType

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения элемента управления типов AppLocker приложений
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Значение по умолчанию устройства, тип элемента управления приложениями, не выбран.|
|enforceComponentsAndStoreApps|1|Принудительное применение компонента и хранилища приложений Windows.|
|auditComponentsAndStoreApps|2|Аудит компонента и хранилища приложений Windows.|
|enforceComponentsStoreAppsAndSmartlocker|3|Принудительное применение компонентов Windows, хранилища приложений и смарт-корзины.|
|auditComponentsStoreAppsAndSmartlocker|4|Аудит компонентов Windows, хранилища приложений и смарт-корзины.|



