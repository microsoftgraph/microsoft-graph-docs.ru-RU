---
title: тип enum automaticUpdateMode
description: Возможные значения для режима автоматического обновления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d1a3aa7050342d370f8bc5b575303b2f036a71d9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820466"
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



