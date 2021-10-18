---
title: тип enum automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 55f706fb15ab2c6f40800ea9b2170977de8b3c65
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60455746"
---
# <a name="automaticupdatemode-enum-type"></a>тип enum automaticUpdateMode

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для режима автоматического обновления.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Значение User Defined, значение по умолчанию, без намерения.|
|notifyDownload|1|Уведомление о загрузке.|
|autoInstallAtMaintenanceTime|2|Автоматическая установка во время обслуживания.|
|autoInstallAndRebootAtMaintenanceTime|3|Автоматическая установка и перезагрузка во время обслуживания.|
|autoInstallAndRebootAtScheduledTime|4 |Автоматическая установка и перезагрузка в запланированное время.|
|autoInstallAndRebootWithoutEndUserControl|5|Автоматическая установка и перезапуск без управления конечным пользователем|



