---
title: Регистрация устройств для управления в Intune
description: " Регистрации (BYOD) позволяет пользователям регистрации своих личных телефоны, планшетные ПК или ПК. Регистрация по программе \"Корпоративное устройство\" (COD) обеспечивает такие сценарии управления, как удаленная очистка, использование общих устройств или сходство пользователя для устройства."
ms.openlocfilehash: a0658051733d202f4074217746882081a29ecd12
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027718"
---
# <a name="enroll-devices-for-management-in-intune"></a>Регистрация устройств для управления в Intune

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.

Вы можете зарегистрировать устройства, в том числе компьютеры с Windows, включив управление мобильными устройствами (MDM) с помощью Microsoft Intune. В этой статье описано несколько способов регистрации мобильных устройств для управления в Intune. Способ регистрации устройств зависит от типа устройства, его владельца и необходимого уровня управления. По программе "принеси свое устройство" (BYOD) пользователи могут зарегистрировать личные телефоны, планшеты или компьютеры. Регистрация по программе "Корпоративное устройство" (COD) обеспечивает такие сценарии управления, как удаленная очистка, использование общих устройств или сходство пользователя для устройства.

Для управления регистрацией в Intune используются перечисленные ниже ресурсы Graph.  

- [Настройка регистрации устройств](intune-onboarding-deviceenrollmentconfiguration.md)
- [Настройка ограничения регистрации устройств](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [Ограничение платформы для регистрации устройств](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [Настройка ограничений для платформы регистрации устройств](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [Настройка регистрации устройств в Windows Hello для бизнеса](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [Соединитель Exchange для управления устройствами](intune-onboarding-devicemanagementexchangeconnector.md)
- [Состояние соединителя устройства управления exchange](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [Тип синхронизации устройства управления exchange соединителя](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [Тип соединителя устройства управления exchange](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [Партнер по управлению устройствами](intune-onboarding-devicemanagementpartner.md)
- [Тип приложения партнера управления устройства](intune-onboarding-devicemanagementpartnerapptype.md)
- [Состояние устройства управления партнера клиента](intune-onboarding-devicemanagementpartnertenantstate.md)
- [Включение](intune-onboarding-enablement.md)
- [Назначение конфигураций регистрации](intune-onboarding-enrollmentconfigurationassignment.md)
- [Торговая марка Intune](intune-onboarding-intunebrand.md)
- [MDM центра сертификации](intune-onboarding-mdmauthority.md)
- [Соединитель Mobile Threat Defense](intune-onboarding-mobilethreatdefenseconnector.md)
- [Состояние клиента мобильных threat партнера](intune-onboarding-mobilethreatpartnertenantstate.md)
- [Настройка локального условного доступа](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [Организация](intune-onboarding-organization.md)
- [Цвет RGB](intune-onboarding-rgbcolor.md)
- [Маркер VPP](intune-onboarding-vpptoken.md)
- [Состояние VPP маркеров](intune-onboarding-vpptokenstate.md)
- [Состояние VPP маркеров синхронизации](intune-onboarding-vpptokensyncstatus.md)
- [Windows Hello для использования business ПИН-кода](intune-onboarding-windowshelloforbusinesspinusage.md)
