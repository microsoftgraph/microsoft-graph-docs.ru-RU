---
title: Тип перечисления appLockerApplicationControlType
description: Возможные значения элемента управления типов AppLocker приложений
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 258a98b9ec4945c807a6aae2b34a178628952ac4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937959"
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



