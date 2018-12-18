---
title: Тип перечисления appLockerApplicationControlType
description: Возможные значения элемента управления типов AppLocker приложений
author: tfitzmac
ms.openlocfilehash: 0d6190170d6f6695a3303047f9ccb193afd248f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330207"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>Тип перечисления appLockerApplicationControlType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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





