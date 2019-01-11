---
title: Регистрация корпоративных устройств с помощью Intune
description: " Сценарий (BYOD)."
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07623c878ac3df9d8a171d7850868f2d7b84e56c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843941"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>Регистрация корпоративных устройств с помощью Intune

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.

Вы можете зарегистрировать устройства, которые принадлежат организации или компании, чтобы управлять устройством в Intune рядом способов в зависимости от его типа устройства и потребностей организации, а также того, как было приобретено устройство. Кроме того, для регистрации корпоративных устройств и управления ими (как в сценарии BYOD, или "принеси свое устройство") можно установить приложение "Корпоративный портал".

Для управления корпоративными устройствами в Intune используются перечисленные ниже ресурсы Graph.

- [Профиль развертывания автопилот windows Active directory](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [Azure AD windows автопилот развертывания профилей](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [Предотвращение выполнения данных регистрации основного профиля](intune-enrollment-depenrollmentbaseprofile.md)
- [Предотвращение выполнения данных регистрации профилей](intune-enrollment-depenrollmentprofile.md)
- [Предотвращение выполнения данных профилей регистрации операций ввода-вывода](intune-enrollment-depiosenrollmentprofile.md)
- [Предотвращение выполнения данных macOS регистрации профилей](intune-enrollment-depmacosenrollmentprofile.md)
- [Параметр DEP на использование доски](intune-enrollment-deponboardingsetting.md)
- [Тип токена DEP](intune-enrollment-deptokentype.md)
- [Обнаружение источника](intune-enrollment-discoverysource.md)
- [Профиль регистрации](intune-enrollment-enrollmentprofile.md)
- [State подачи заявок](intune-enrollment-enrollmentstate.md)
- [Импортированные идентификатор устройства Apple](intune-enrollment-importedappledeviceidentity.md)
- [Импортировать идентификатор устройства Apple результатов](intune-enrollment-importedappledeviceidentityresult.md)
- [Импортированные устройств удостоверений](intune-enrollment-importeddeviceidentity.md)
- [Импортированные результатов идентификатор устройства](intune-enrollment-importeddeviceidentityresult.md)
- [Импортировать тип удостоверения устройства](intune-enrollment-importeddeviceidentitytype.md)
- [Импортированные windows автопилот устройств удостоверений](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [Состояние импортированных windows автопилот устройства identity импорта](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [Состояние импортированных windows автопилот устройства удостоверения](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [Отправка identity устройства автопилот импортированных windows](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [Состояние передачи удостоверения устройства автопилот импортированных windows](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [режим связывания iTunes](intune-enrollment-itunespairingmode.md)
- [Управление сертификат с отпечатком](intune-enrollment-managementcertificatewiththumbprint.md)
- [Параметров качества](intune-enrollment-outofboxexperiencesettings.md)
- [Платформа](intune-enrollment-platform.md)
- [Windows автопилот развертывания профилей](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [Назначение профиля развертывания автопилот Windows](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [Удостоверения автопилот устройства Windows](intune-enrollment-windowsautopilotdeviceidentity.md)
- [Назначение профиля Windows автопилот подробное описание состояния](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [Состояние назначения профиля автопилот Windows](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [Параметры автопилот Windows](intune-enrollment-windowsautopilotsettings.md)
- [Состояние синхронизации автопилот Windows](intune-enrollment-windowsautopilotsyncstatus.md)
- [Тип использования устройства Windows](intune-enrollment-windowsdeviceusagetype.md)
- [Параметры экрана состояние регистрации Windows](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [Тип пользователя Windows](intune-enrollment-windowsusertype.md)
