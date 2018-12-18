---
title: Защита данных корпоративных приложений с помощью Microsoft Intune
description: Политики защиты приложений в Microsoft Intune помогают защитить корпоративные данные и предотвратить потерю данных.
author: tfitzmac
ms.openlocfilehash: dd47d1765d53cb8beed7c3b0e87b330b306f8b12
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334512"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>Защита данных корпоративных приложений с помощью Microsoft Intune

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.

Политики защиты приложений в Microsoft Intune помогают защитить корпоративные данные и предотвратить потерю данных.

Политики защиты приложений в Intune используются для защиты корпоративных данных. Так как политики в отношении защиты приложений Intune можно использовать вне зависимости от любого решения по управлению мобильных устройств (MDM), его можно использовать для защиты данных вашей компании с SharePoint и без подающего заявку устройств в решения для управления устройствами. Внедрив политики уровня приложения, вы можете ограничить доступ к корпоративным ресурсам и оставить данные в поле зрения ИТ-отдела.

Для управления политиками защиты приложений в Intune используются перечисленные ниже ресурсы Graph.

- [Защита управляемых приложений для Android](intune-mam-androidmanagedappprotection.md)
- [Регистрация управляемых приложений для Android](intune-mam-androidmanagedappregistration.md)
- [Идентификатор мобильных приложений для Android](intune-mam-androidmobileappidentifier.md)
- [Управление уровня приложения](intune-mam-appmanagementlevel.md)
- [Тип приложения](intune-wip-applicationtype.md)
- [Защита управляемых приложений по умолчанию](intune-mam-defaultmanagedappprotection.md)
- [Intune фирменной настройки профиля](intune-wip-intunebrandingprofile.md)
- [Защита управляемых приложений для iOS](intune-mam-iosmanagedappprotection.md)
- [Регистрация управляемых приложений для iOS](intune-mam-iosmanagedappregistration.md)
- [Идентификатор мобильных приложений для iOS](intune-mam-iosmobileappidentifier.md)
- [JSON](intune-mam-json.md)
- [Управляемые приложения буфер обмена, общий доступ к уровень](intune-mam-managedappclipboardsharinglevel.md)
- [Конфигурация управляемых приложений](intune-mam-managedappconfiguration.md)
- [Управляемый тип шифрования данных приложения](intune-mam-managedappdataencryptiontype.md)
- [Место хранения данных управляемых приложений](intune-mam-managedappdatastoragelocation.md)
- [Уровень передачи данных управляемых приложений](intune-mam-managedappdatatransferlevel.md)
- [Состояние диагностики управляемых приложений](intune-mam-managedappdiagnosticstatus.md)
- [Управляемые приложения отмеченные причине](intune-mam-managedappflaggedreason.md)
- [Операция управляемых приложений](intune-mam-managedappoperation.md)
- [Набор символов управляемых приложений ПИН-кода](intune-mam-managedapppincharacterset.md)
- [Политика управляемых приложений](intune-mam-managedapppolicy.md)
- [Сводка по развертыванию политик для управляемых приложений](intune-mam-managedapppolicydeploymentsummary.md)
- [Сводка по развертыванию политик для отдельных управляемых приложений](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [Защита управляемых приложений](intune-mam-managedappprotection.md)
- [Регистрация управляемых приложений](intune-mam-managedappregistration.md)
- [Действие исправлению управляемых приложений](intune-mam-managedappremediationaction.md)
- [Состояние управляемых приложений](intune-mam-managedappstatus.md)
- [Необработанные данные о состоянии управляемых приложений](intune-mam-managedappstatusraw.md)
- [Управляемое мобильное приложение](intune-mam-managedmobileapp.md)
- [Политика Windows Information Protection для MDM](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [Идентификатор мобильных приложений](intune-mam-mobileappidentifier.md)
- [Целевая конфигурация управляемых приложений](intune-mam-targetedmanagedappconfiguration.md)
- [Назначение целевой политики для управляемых приложений](intune-mam-targetedmanagedapppolicyassignment.md)
- [Целевая защита управляемых приложений](intune-mam-targetedmanagedappprotection.md)
- [Windows Information Protection](intune-mam-windowsinformationprotection.md)
- [Приложение Windows Information Protection](intune-mam-windowsinformationprotectionapp.md)
- [Сводка по обучению приложения Windows Information Protection](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [Файл AppLocker для Windows Information Protection](intune-mam-windowsinformationprotectionapplockerfile.md)
- [Сертификат восстановления данных Windows Information Protection](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [Классическое приложение Windows Information Protection](intune-mam-windowsinformationprotectiondesktopapp.md)
- [Уровень принудительное применение защиты сведения о Windows](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [Коллекция диапазонов IP-адресов Windows Information Protection](intune-mam-windowsinformationprotectioniprangecollection.md)
- [Сводка по обучению сети Windows Information Protection](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [Требования к символ Windows сведения защиты ПИН-кода](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [Политика Windows Information Protection](intune-mam-windowsinformationprotectionpolicy.md)
- [Коллекция проксируемых доменов Windows Information Protection](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [Коллекция ресурсов Windows Information Protection](intune-mam-windowsinformationprotectionresourcecollection.md)
- [Приложение из магазина Windows Information Protection](intune-mam-windowsinformationprotectionstoreapp.md)
