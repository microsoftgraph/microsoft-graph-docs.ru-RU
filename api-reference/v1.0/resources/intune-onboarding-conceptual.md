---
title: Регистрация устройств для управления в Intune
description: " (BYOD) регистрация позволяет пользователям записать свои личные телефоны, планшеты или компьютеры. Регистрация по программе \"Корпоративное устройство\" (COD) обеспечивает такие сценарии управления, как удаленная очистка, использование общих устройств или сходство пользователя для устройства."
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 7e435246df7b2f57ab5f7d18d90ada3c56ec6579
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098673"
---
# <a name="enroll-devices-for-management-in-intune"></a>Регистрация устройств для управления в Intune

Пространство имен: microsoft.graph

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.

Вы можете зарегистрировать устройства, в том числе компьютеры с Windows, включив управление мобильными устройствами (MDM) с помощью Microsoft Intune. В этой статье описано несколько способов регистрации мобильных устройств для управления в Intune. Способ регистрации устройств зависит от типа устройства, его владельца и необходимого уровня управления. По программе "принеси свое устройство" (BYOD) пользователи могут зарегистрировать личные телефоны, планшеты или компьютеры. Регистрация по программе "Корпоративное устройство" (COD) обеспечивает такие сценарии управления, как удаленная очистка, использование общих устройств или сходство пользователя для устройства.

Для управления регистрацией в Intune используются перечисленные ниже ресурсы Graph.  

- [Партнер по управлению соответствием требованиям](intune-onboarding-compliancemanagementpartner.md)
- [Назначение партнера по управлению соответствием требованиям](intune-onboarding-compliancemanagementpartnerassignment.md)
- [Управление приложениями для устройств](intune-onboarding-deviceappmanagement.md)
- [Категория устройств](intune-onboarding-devicecategory.md)
- [Настройка регистрации устройств](intune-onboarding-deviceenrollmentconfiguration.md)
- [Настройка ограничения регистрации устройств](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [Ограничение платформы для регистрации устройств](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [Настройка ограничений для платформы регистрации устройств](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [Настройка регистрации устройств в Windows Hello для бизнеса](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [Управление устройствами](intune-onboarding-devicemanagement.md)
- [Соединитель Exchange для управления устройствами](intune-onboarding-devicemanagementexchangeconnector.md)
- [Состояние соединителя Exchange для управления устройствами](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [Тип синхронизации соединителя Exchange для управления устройствами](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [Тип соединителя Exchange для управления устройствами](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [Партнер по управлению устройствами](intune-onboarding-devicemanagementpartner.md)
- [Тип партнерского приложения для управления устройствами](intune-onboarding-devicemanagementpartnerapptype.md)
- [Состояние клиента партнера по управлению устройствами](intune-onboarding-devicemanagementpartnertenantstate.md)
- [Включение](intune-onboarding-enablement.md)
- [Назначение конфигураций регистрации](intune-onboarding-enrollmentconfigurationassignment.md)
- [Торговая марка Intune](intune-onboarding-intunebrand.md)
- [Центр MDM](intune-onboarding-mdmauthority.md)
- [Соединитель Mobile Threat Defense](intune-onboarding-mobilethreatdefenseconnector.md)
- [Состояние клиента партнера Mobile Threat Defense](intune-onboarding-mobilethreatpartnertenantstate.md)
- [Настройка локального условного доступа](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [Организация](intune-onboarding-organization.md)
- [Цвет RGB](intune-onboarding-rgbcolor.md)
- [Пользователь](intune-onboarding-user.md)
- [Маркер VPP](intune-onboarding-vpptoken.md)
- [Состояние токена VPP](intune-onboarding-vpptokenstate.md)
- [Состояние синхронизации токена VPP](intune-onboarding-vpptokensyncstatus.md)
- [Использование ПИН-кода в Windows Hello для бизнеса](intune-onboarding-windowshelloforbusinesspinusage.md)
