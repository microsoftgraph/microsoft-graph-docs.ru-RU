---
title: Встроенные управляемые устройства с помощью API Intune-Microsoft Graph
description: Перечисление API Microsoft Graph для конечных точек Intune (REST), используемых для встроенных устройств (Настройка и инициализация) для организации клиента.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: d03cd932386b4b36af2f43beefee5cf59d21395c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196499"
---
# <a name="enroll-devices-for-management-in-intune"></a>Регистрация устройств для управления в Intune

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Вы можете зарегистрировать устройства, в том числе компьютеры с Windows, включив управление мобильными устройствами (MDM) с помощью Microsoft Intune. В этой статье описано несколько способов регистрации мобильных устройств для управления в Intune. Способ регистрации устройств зависит от типа устройства, его владельца и необходимого уровня управления. По программе "принеси свое устройство" (BYOD) пользователи могут зарегистрировать личные телефоны, планшеты или компьютеры. Регистрация по программе "Корпоративное устройство" (COD) обеспечивает такие сценарии управления, как удаленная очистка, использование общих устройств или сходство пользователя для устройства.

Для управления регистрацией в Intune используются перечисленные ниже ресурсы Graph.

- [Параметр соединителя сертификатов](intune-onboarding-certificateconnectorsetting.md)
- [Данные об управлении устройствами и приложениями](intune-onboarding-deviceandappmanagementdata.md)
- [Настройка ограничения регистрации устройств](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [Ограничение платформы для регистрации устройств](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [Настройка ограничений для платформы регистрации устройств](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [Настройка регистрации устройств в Windows Hello для бизнеса](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [Уровень доступа к Exchange для управления устройствами](intune-onboarding-devicemanagementexchangeaccesslevel.md)
- [Правило доступа к Exchange для управления устройствами](intune-onboarding-devicemanagementexchangeaccessrule.md)
- [Тип правила доступа к Exchange для управления устройствами](intune-onboarding-devicemanagementexchangeaccessruletype.md)
- [Соединитель Exchange для управления устройствами](intune-onboarding-devicemanagementexchangeconnector.md)
- [Состояние соединителя Exchange для управления устройствами](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [Тип синхронизации соединителя Exchange для управления устройствами](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [Тип соединителя Exchange для управления устройствами](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [Класс устройства Exchange для управления устройствами](intune-onboarding-devicemanagementexchangedeviceclass.md)
- [Локальная политика Exchange для управления устройствами](intune-onboarding-devicemanagementexchangeonpremisespolicy.md)
- [Партнер по управлению устройствами](intune-onboarding-devicemanagementpartner.md)
- [Тип партнерского приложения для управления устройствами](intune-onboarding-devicemanagementpartnerapptype.md)
- [Состояние клиента партнера по управлению устройствами](intune-onboarding-devicemanagementpartnertenantstate.md)
- [Назначение конфигураций регистрации](intune-onboarding-enrollmentconfigurationassignment.md)
- [Торговая марка Intune](intune-onboarding-intunebrand.md)
- [Центр MDM](intune-onboarding-mdmauthority.md)
- [Опции выбора портала Microsoft store для бизнеса](intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)
- [Соединитель Mobile Threat Defense](intune-onboarding-mobilethreatdefenseconnector.md)
- [Состояние клиента партнера Mobile Threat Defense](intune-onboarding-mobilethreatpartnertenantstate.md)
- [Настройка локального условного доступа](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [Организация](intune-onboarding-organization.md)
- [Ключ для загрузки неопубликованных приложений](intune-onboarding-sideloadingkey.md)
- [Маркер VPP](intune-onboarding-vpptoken.md)
- [Результат действия с токеном VPP](intune-onboarding-vpptokenactionresult.md)
- [Сводка о лицензии для маркера VPP](intune-onboarding-vpptokenlicensesummary.md)
- [Результат действия "Отзыв лицензий с маркером VPP"](intune-onboarding-vpptokenrevokelicensesactionresult.md)
- [Состояние токена VPP](intune-onboarding-vpptokenstate.md)
- [Состояние синхронизации токена VPP](intune-onboarding-vpptokensyncstatus.md)
- [Настройка страницы завершения регистрации в Windows 10](intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)
- [Использование ПИН-кода в Windows Hello для бизнеса](intune-onboarding-windowshelloforbusinesspinusage.md)
