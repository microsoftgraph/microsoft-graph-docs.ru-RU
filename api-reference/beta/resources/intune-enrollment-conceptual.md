---
title: Регистрация корпоративных устройств с помощью Intune-API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), которые регистрируют устройства для организации клиента.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 506f85ae59330757f4c6f12cf80795c6678b125e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366373"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>Регистрация корпоративных устройств с помощью Intune

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Вы можете зарегистрировать устройства, которые принадлежат организации или компании, чтобы управлять устройством в Intune рядом способов в зависимости от его типа устройства и потребностей организации, а также того, как было приобретено устройство. Кроме того, для регистрации корпоративных устройств и управления ими (как в сценарии BYOD, или "принеси свое устройство") можно установить приложение "Корпоративный портал".

Для управления корпоративными устройствами в Intune используются перечисленные ниже ресурсы Graph.

- [Профиль Windows AutoPilot Deployment для Active Directory](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [Профиль Windows AutoPilot Deployment для Azure AD](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [Базовые профиль регистрации DEP](intune-enrollment-depenrollmentbaseprofile.md)
- [Профиль регистрации DEP](intune-enrollment-depenrollmentprofile.md)
- [Профиль регистрации iOS DEP](intune-enrollment-depiosenrollmentprofile.md)
- [Профиль регистрации macOS DEP](intune-enrollment-depmacosenrollmentprofile.md)
- [Параметр подключения DEP](intune-enrollment-deponboardingsetting.md)
- [Тип маркера DEP](intune-enrollment-deptokentype.md)
- [Источник обнаружения](intune-enrollment-discoverysource.md)
- [Профиль регистрации](intune-enrollment-enrollmentprofile.md)
- [Состояние регистрации](intune-enrollment-enrollmentstate.md)
- [Импортированное удостоверение устройства Apple](intune-enrollment-importedappledeviceidentity.md)
- [Результат импорта удостоверения устройства Apple](intune-enrollment-importedappledeviceidentityresult.md)
- [Импортированное удостоверение устройства](intune-enrollment-importeddeviceidentity.md)
- [Результат импорта удостоверения устройства](intune-enrollment-importeddeviceidentityresult.md)
- [Тип импортированного удостоверения устройства](intune-enrollment-importeddeviceidentitytype.md)
- [Импортированное удостоверение устройства с Windows Autopilot](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [Состояние импорта удостоверения устройства с Windows Autopilot](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [Состояние импортированного удостоверения устройства с Windows Autopilot](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [Статус загрузки импортированного удостоверения устройства Windows AutoPilot](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [Режим связывания с iTunes](intune-enrollment-itunespairingmode.md)
- [Сертификат управления с отпечатком](intune-enrollment-managementcertificatewiththumbprint.md)
- [Параметры запуска при первом включении компьютера](intune-enrollment-outofboxexperiencesettings.md)
- [Платформа](intune-enrollment-platform.md)
- [Профиль Windows AutoPilot Deployment](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [Назначение профиля Windows Autopilot Deployment](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [Удостоверение устройства с Windows Autopilot](intune-enrollment-windowsautopilotdeviceidentity.md)
- [Тип устройства с Windows Autopilot](intune-enrollment-windowsautopilotdevicetype.md)
- [Полное состояние назначения профиля Windows AutoPilot](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [Состояние назначения профиля Windows AutoPilot](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [Параметры Windows AutoPilot](intune-enrollment-windowsautopilotsettings.md)
- [Состояние синхронизации Windows Autopilot](intune-enrollment-windowsautopilotsyncstatus.md)
- [Тип использования устройства Windows](intune-enrollment-windowsdeviceusagetype.md)
- [Параметры экрана состояния регистрации Windows](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [Тип пользователя Windows](intune-enrollment-windowsusertype.md)
