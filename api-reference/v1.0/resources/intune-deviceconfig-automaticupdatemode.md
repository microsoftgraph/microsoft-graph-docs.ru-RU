---
title: тип enum automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e3a076fcc88cb64ddeebddcb7f97c3e77c2b34ec
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136483"
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
|autoInstallAndRebootWithoutEndUserControl|5 |Автоматическая установка и перезапуск без управления конечным пользователем|




