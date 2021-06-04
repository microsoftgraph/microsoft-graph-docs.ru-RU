---
title: Защита данных корпоративных приложений с помощью Microsoft Intune
description: Политики защиты приложений в Microsoft Intune помогают защитить корпоративные данные и предотвратить потерю данных.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 33e814dc754d564dd3921d7f4369f0112b7a8ec0
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732835"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>Защита данных корпоративных приложений с помощью Microsoft Intune

Пространство имен: microsoft.graph

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.

Политики защиты приложений в Microsoft Intune помогают защитить корпоративные данные и предотвратить потерю данных.

Политики защиты приложений в Intune используются для защиты корпоративных данных. Так как эти политики можно использовать вне зависимости от любого решения для управления мобильными устройствами (MDM), защита корпоративных данных обеспечивается как с регистрацией устройства в решении по управлению устройствами, так и без нее. Внедрив политики уровня приложения, вы можете ограничить доступ к корпоративным ресурсам и оставить данные в поле зрения ИТ-отдела.

Для управления политиками защиты приложений в Intune используются перечисленные ниже ресурсы Graph.  

- [Защита управляемых приложений для Android](intune-mam-androidmanagedappprotection.md)
- [Регистрация управляемых приложений для Android](intune-mam-androidmanagedappregistration.md)
- [Идентификатор мобильных приложений для Android](intune-mam-androidmobileappidentifier.md)
- [Тип приложения](intune-wip-applicationtype.md)
- [Защита управляемых приложений по умолчанию](intune-mam-defaultmanagedappprotection.md)
- [Защита управляемых приложений для iOS](intune-mam-iosmanagedappprotection.md)
- [Регистрация управляемых приложений для iOS](intune-mam-iosmanagedappregistration.md)
- [Идентификатор мобильных приложений для iOS](intune-mam-iosmobileappidentifier.md)
- [Диапазон IP-адресов](intune-mam-iprange.md)
- [Диапазон IPv4-адресов](intune-mam-ipv4range.md)
- [Диапазон IPv6-адресов](intune-mam-ipv6range.md)
- [JSON](intune-mam-json.md)
- [Пара "ключ-значение"](intune-mam-keyvaluepair.md)
- [Уровень совместного доступа к буферу обмена управляемого приложения](intune-mam-managedappclipboardsharinglevel.md)
- [Конфигурация управляемых приложений](intune-mam-managedappconfiguration.md)
- [Тип шифрования данных управляемого приложения](intune-mam-managedappdataencryptiontype.md)
- [Место хранения данных управляемого приложения](intune-mam-managedappdatastoragelocation.md)
- [Уровень передачи данных управляемого приложения](intune-mam-managedappdatatransferlevel.md)
- [Состояние диагностики управляемых приложений](intune-mam-managedappdiagnosticstatus.md)
- [Причина пометки управляемого приложения](intune-mam-managedappflaggedreason.md)
- [Операция управляемых приложений](intune-mam-managedappoperation.md)
- [Набор символов ПИН-кода управляемого приложения](intune-mam-managedapppincharacterset.md)
- [Политика управляемых приложений](intune-mam-managedapppolicy.md)
- [Сводка по развертыванию политик для управляемых приложений](intune-mam-managedapppolicydeploymentsummary.md)
- [Сводка по развертыванию политик для отдельных управляемых приложений](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [Защита управляемых приложений](intune-mam-managedappprotection.md)
- [Регистрация управляемых приложений](intune-mam-managedappregistration.md)
- [Состояние управляемых приложений](intune-mam-managedappstatus.md)
- [Необработанные данные о состоянии управляемых приложений](intune-mam-managedappstatusraw.md)
- [Управляемое мобильное приложение](intune-mam-managedmobileapp.md)
- [Политика Windows Information Protection для MDM](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [Идентификатор мобильных приложений](intune-mam-mobileappidentifier.md)
- [Проксируемый домен](intune-mam-proxieddomain.md)
- [Целевая конфигурация управляемых приложений](intune-mam-targetedmanagedappconfiguration.md)
- [Назначение целевой политики для управляемых приложений](intune-mam-targetedmanagedapppolicyassignment.md)
- [Целевая защита управляемых приложений](intune-mam-targetedmanagedappprotection.md)
- [Windows Information Protection](intune-mam-windowsinformationprotection.md)
- [Приложение Windows Information Protection](intune-mam-windowsinformationprotectionapp.md)
- [Сводка по обучению приложения Windows Information Protection](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [Файл AppLocker для Windows Information Protection](intune-mam-windowsinformationprotectionapplockerfile.md)
- [Сертификат восстановления данных Windows Information Protection](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [Классическое приложение Windows Information Protection](intune-mam-windowsinformationprotectiondesktopapp.md)
- [Уровень применения Windows Information Protection](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [Коллекция диапазонов IP-адресов Windows Information Protection](intune-mam-windowsinformationprotectioniprangecollection.md)
- [Сводка по обучению сети Windows Information Protection](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [Требования к символам ПИН-кода Windows Information Protection](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [Политика Windows Information Protection](intune-mam-windowsinformationprotectionpolicy.md)
- [Коллекция проксируемых доменов Windows Information Protection](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [Коллекция ресурсов Windows Information Protection](intune-mam-windowsinformationprotectionresourcecollection.md)
- [Приложение из магазина Windows Information Protection](intune-mam-windowsinformationprotectionstoreapp.md)






