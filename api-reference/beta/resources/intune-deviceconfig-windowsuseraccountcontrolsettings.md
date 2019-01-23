---
title: Тип перечисления windowsUserAccountControlSettings
description: Возможные значения для параметров контроля учетных записей пользователей Windows.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ff348fd33e6bbc8370378783cf0a517a205ea101
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399817"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a>Тип перечисления windowsUserAccountControlSettings

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для параметров контроля учетных записей пользователей Windows.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|User Defined, значение по умолчанию, без цели.|
|alwaysNotify|1|Всегда уведомите.|
|notifyOnAppChanges|2|Уведомление об изменениях приложения.|
|notifyOnAppChangesWithoutDimming|3|Уведомления на изменения в приложении без затемнение рабочего стола.|
|neverNotify|4|Никогда не уведомлять.|




