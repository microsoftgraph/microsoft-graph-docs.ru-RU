---
title: Подключение управляемых устройств с Intune — Microsoft API Graph
description: Список microsoft API Graph для Intune конечных точек (REST), используемых для подключения (настройки и инициализации) устройств для организации клиента.
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
ms.openlocfilehash: e005cc667656b5620778dc80bd80ffe65736b08e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211328"
---
# <a name="enroll-devices-for-management-in-intune"></a>Регистрация устройств для управления в Intune

Пространство имен: microsoft.graph

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Вы можете зарегистрировать устройства, в том числе компьютеры с Windows, включив управление мобильными устройствами (MDM) с помощью Microsoft Intune. В этой статье описано несколько способов регистрации мобильных устройств для управления в Intune. Способ регистрации устройств зависит от типа устройства, его владельца и необходимого уровня управления. По программе "принеси свое устройство" (BYOD) пользователи могут зарегистрировать личные телефоны, планшеты или компьютеры. Регистрация по программе "Корпоративное устройство" (COD) обеспечивает такие сценарии управления, как удаленная очистка, использование общих устройств или сходство пользователя для устройства.

Для управления регистрацией в Intune используются перечисленные ниже ресурсы Graph.

- [Параметр соединителя сертификатов](intune-onboarding-certificateconnectorsetting.md)
- [Партнер по управлению соответствием требованиям](intune-onboarding-compliancemanagementpartner.md)
- [Назначение партнера по управлению соответствием требованиям](intune-onboarding-compliancemanagementpartnerassignment.md)
- [Данные об управлении устройствами и приложениями](intune-onboarding-deviceandappmanagementdata.md)
- [Конфигурация центра совместного управления устройствами](intune-onboarding-devicecomanagementauthorityconfiguration.md)
- [Тип конфигурации регистрации устройства](intune-onboarding-deviceenrollmentconfigurationtype.md)
- [Настройка ограничения регистрации устройств](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [Настройка уведомлений о регистрации устройств](intune-onboarding-deviceenrollmentnotificationconfiguration.md)
- [Ограничение платформы для регистрации устройств](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [Конфигурация ограничений платформы регистрации устройств](intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)
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
- [Назначение партнера по управлению устройствами](intune-onboarding-devicemanagementpartnerassignment.md)
- [Состояние клиента партнера по управлению устройствами](intune-onboarding-devicemanagementpartnertenantstate.md)
- [Тип платформы устройства](intune-onboarding-deviceplatformtype.md)
- [Назначение конфигураций регистрации](intune-onboarding-enrollmentconfigurationassignment.md)
- [Параметры фирменной символики уведомлений о регистрации](intune-onboarding-enrollmentnotificationbrandingoptions.md)
- [Тип шаблона уведомления о регистрации](intune-onboarding-enrollmentnotificationtemplatetype.md)
- [Тип платформы ограничений регистрации](intune-onboarding-enrollmentrestrictionplatformtype.md)
- [Торговая марка Intune](intune-onboarding-intunebrand.md)
- [MDM authority](intune-onboarding-mdmauthority.md)
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
