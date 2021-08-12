---
title: Регистрация корпоративных устройств с помощью Intune - Microsoft Graph API
description: Перечисляет API Graph Microsoft для конечных точек Intune (REST), которые регистрировать устройства для организации-клиента.
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 35fd75cd054bace77f1559670e667f40f09dd82bdfad9e52196228ae135fde95
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169503"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>Регистрация корпоративных устройств с помощью Intune

Пространство имен: microsoft.graph

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Вы можете зарегистрировать устройства, которые принадлежат организации или компании, чтобы управлять устройством в Intune рядом способов в зависимости от его типа устройства и потребностей организации, а также того, как было приобретено устройство. Кроме того, для регистрации корпоративных устройств и управления ими (как в сценарии BYOD, или "принеси свое устройство") можно установить приложение "Корпоративный портал".

Для управления корпоративными устройствами в Intune используются перечисленные ниже ресурсы Graph.

- [Управление устройствами](intune-enrollment-devicemanagement.md)
- [Состояние регистрации](intune-enrollment-enrollmentstate.md)
- [Импортированное удостоверение устройства с Windows Autopilot](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [Состояние импорта удостоверения устройства с Windows Autopilot](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [Состояние импортированного удостоверения устройства с Windows Autopilot](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [Статус загрузки импортированного удостоверения устройства Windows AutoPilot](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [Удостоверение устройства с Windows Autopilot](intune-enrollment-windowsautopilotdeviceidentity.md)