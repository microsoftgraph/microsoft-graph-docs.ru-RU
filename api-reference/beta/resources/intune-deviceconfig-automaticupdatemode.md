---
title: тип enum automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 510b28d926a70f0777ba559d9062e88de4099b11
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146753"
---
# <a name="automaticupdatemode-enum-type"></a>тип enum automaticUpdateMode

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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
|windowsDefault|6 |Сброс значения Windows по умолчанию.|



