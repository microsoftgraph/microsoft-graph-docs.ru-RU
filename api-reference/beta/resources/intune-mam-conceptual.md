---
title: Управление мобильными приложениями с Microsoft Intune - API Graph Microsoft
description: Списки API Graph Microsoft для конечных точек Intune (REST), связанных с управлением мобильными приложениями (MAM) для организации-клиента.
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: de457279a525e74855ce9c05d98ff72beb1546dc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796490"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>Защита данных корпоративных приложений с помощью Microsoft Intune

Пространство имен: microsoft.graph

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политики защиты приложений в Microsoft Intune помогают защитить корпоративные данные и предотвратить потерю данных.

Политики защиты приложений в Intune используются для защиты корпоративных данных. Так как политики защиты приложений Intune можно использовать независимо от любого решения управления мобильными устройствами (MDM), его можно использовать для защиты данных вашей компании с помощью или без регистрации устройств в решении управления устройствами. Внедрив политики уровня приложения, вы можете ограничить доступ к корпоративным ресурсам и оставить данные в поле зрения ИТ-отдела.

Для управления политиками защиты приложений в Intune используются перечисленные ниже ресурсы Graph.

- [Регистрация управляемых приложений для Android](intune-mam-androidmanagedappregistration.md)
- [Тип проверки приложений системы безопасности для управляемых приложений для Android](intune-mam-androidmanagedappsafetynetappsverificationtype.md)
- [Тип аттестации устройства системы безопасности для управляемых приложений для Android](intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)
- [Тип оценки сети безопасности управляемых приложений для Android](intune-mam-androidmanagedappsafetynetevaluationtype.md)
- [Идентификатор мобильных приложений для Android](intune-mam-androidmobileappidentifier.md)
- [Уровень управления приложениями](intune-mam-appmanagementlevel.md)
- [Тип приложения](intune-wip-applicationtype.md)
- [Защита управляемых приложений по умолчанию](intune-mam-defaultmanagedappprotection.md)
- [Тип платформы устройства](intune-wip-deviceplatformtype.md)
- [Профиль фирменной символики Intune](intune-wip-intunebrandingprofile.md)
- [Назначение профиля фирменной символики Intune](intune-wip-intunebrandingprofileassignment.md)
- [Регистрация управляемых приложений для iOS](intune-mam-iosmanagedappregistration.md)
- [Идентификатор мобильных приложений для iOS](intune-mam-iosmobileappidentifier.md)
- [JSON](intune-mam-json.md)
- [Пара "ключ-значение"](intune-mam-keyvaluepair.md)
- [Идентификатор приложения Mac](intune-mam-macappidentifier.md)
- [Уровень совместного доступа к буферу обмена управляемого приложения](intune-mam-managedappclipboardsharinglevel.md)
- [Конфигурация управляемых приложений](intune-mam-managedappconfiguration.md)
- [Тип шифрования данных управляемого приложения](intune-mam-managedappdataencryptiontype.md)
- [Расположение управляемого прогона данных приложения](intune-mam-managedappdataingestionlocation.md)
- [Место хранения данных управляемого приложения](intune-mam-managedappdatastoragelocation.md)
- [Уровень передачи данных управляемого приложения](intune-mam-managedappdatatransferlevel.md)
- [Уровень угрозы управляемого устройства приложения](intune-mam-managedappdevicethreatlevel.md)
- [Состояние диагностики управляемых приложений](intune-mam-managedappdiagnosticstatus.md)
- [Причина пометки управляемого приложения](intune-mam-managedappflaggedreason.md)
- [Ограничение уведомлений об управляемом приложении](intune-mam-managedappnotificationrestriction.md)
- [Операция управляемых приложений](intune-mam-managedappoperation.md)
- [Уровень перенаправления номеров управляемых приложений](intune-mam-managedappphonenumberredirectlevel.md)
- [Набор символов ПИН-кода управляемого приложения](intune-mam-managedapppincharacterset.md)
- [Политика управляемых приложений](intune-mam-managedapppolicy.md)
- [Сводка по развертыванию политик для управляемых приложений](intune-mam-managedapppolicydeploymentsummary.md)
- [Сводка по развертыванию политик для отдельных управляемых приложений](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [Защита управляемых приложений](intune-mam-managedappprotection.md)
- [Регистрация управляемых приложений](intune-mam-managedappregistration.md)
- [Действие исправления для управляемого приложения](intune-mam-managedappremediationaction.md)
- [Состояние управляемых приложений](intune-mam-managedappstatus.md)
- [Необработанные данные о состоянии управляемых приложений](intune-mam-managedappstatusraw.md)
- [Тип управляемого браузера](intune-mam-managedbrowsertype.md)
- [Управляемое мобильное приложение](intune-mam-managedmobileapp.md)
- [Идентификатор мобильных приложений](intune-mam-mobileappidentifier.md)
- [Целевой тип группы управляемых приложений](intune-mam-targetedmanagedappgrouptype.md)
- [Назначение целевой политики для управляемых приложений](intune-mam-targetedmanagedapppolicyassignment.md)
- [Целевая защита управляемых приложений](intune-mam-targetedmanagedappprotection.md)
- [Windows приложения](intune-mam-windowsappidentifier.md)
- [Windows Information Protection](intune-mam-windowsinformationprotection.md)
- [Приложение Windows Information Protection](intune-mam-windowsinformationprotectionapp.md)
- [Сводка по обучению приложения Windows Information Protection](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [Файл AppLocker для Windows Information Protection](intune-mam-windowsinformationprotectionapplockerfile.md)
- [Сертификат восстановления данных Windows Information Protection](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [Классическое приложение Windows Information Protection](intune-mam-windowsinformationprotectiondesktopapp.md)
- [Регистрация устройства Windows information protection](intune-mam-windowsinformationprotectiondeviceregistration.md)
- [Уровень применения Windows Information Protection](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [Коллекция диапазонов IP-адресов Windows Information Protection](intune-mam-windowsinformationprotectioniprangecollection.md)
- [Сводка по обучению сети Windows Information Protection](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [Требования к символам ПИН-кода Windows Information Protection](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [Политика Windows Information Protection](intune-mam-windowsinformationprotectionpolicy.md)
- [Коллекция проксируемых доменов Windows Information Protection](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [Коллекция ресурсов Windows Information Protection](intune-mam-windowsinformationprotectionresourcecollection.md)
- [Приложение из магазина Windows Information Protection](intune-mam-windowsinformationprotectionstoreapp.md)
- [Действие wipe для Windows Information Protection](intune-mam-windowsinformationprotectionwipeaction.md)
