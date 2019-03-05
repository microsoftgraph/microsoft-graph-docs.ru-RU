---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), поддерживающих несколько рабочих процессов для организации клиента.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 6436f134ae9e95623b073f6e645f0737d45d540e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158312"
---
# <a name="shared-resources-in-microsoft-intune"></a>Общие ресурсы в Microsoft Intune

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.

Эти конечные точки используются в нескольких ИНТЕРФЕЙСах API Microsoft Graph для рабочих процессов Intune.  Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.  Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.

Рабочие процессы Intune совместно работают со следующими ресурсами Graph:

- [Состояние действия](intune-shared-actionstate.md)
- [Объект назначения всех устройств](intune-shared-alldevicesassignmenttarget.md)
- [Объект назначения всех лицензированных пользователей](intune-shared-alllicensedusersassignmenttarget.md)
- [Состояние соответствия](intune-shared-compliancestatus.md)
- [Объект назначения для управления устройствами и приложениями](intune-shared-deviceandappmanagementassignmenttarget.md)
- [Управление приложениями для устройств](intune-shared-deviceappmanagement.md)
- [Категория устройств](intune-shared-devicecategory.md)
- [Тип регистрации устройства](intune-shared-deviceenrollmenttype.md)
- [Управление устройствами](intune-shared-devicemanagement.md)
- [Тип платформы устройства](intune-shared-deviceplatformtype.md)
- [Тип устройства](intune-shared-devicetype.md)
- [Включение](intune-shared-enablement.md)
- [Объект назначения группы исключения](intune-shared-exclusiongroupassignmenttarget.md)
- [Объект назначения группы](intune-shared-groupassignmenttarget.md)
- [Намерение установки](intune-shared-installintent.md)
- [Диапазон IP-адресов](intune-shared-iprange.md)
- [Диапазон IPv4-адресов](intune-shared-ipv4range.md)
- [Диапазон IPv6-адресов](intune-shared-ipv6range.md)
- [Пара "ключ-значение"](intune-shared-keyvaluepair.md)
- [Содержимое MIME](intune-shared-mimecontent.md)
- [Устранение неполадок с мобильным приложением: событие](intune-shared-mobileapptroubleshootingevent.md)
- [Проксируемый домен](intune-shared-proxieddomain.md)
- [Report](intune-shared-report.md)
- [Корневая папка отчета](intune-shared-reportroot.md)
- [Итоговое состояние приложения](intune-shared-resultantappstate.md)
- [Цвет RGB](intune-shared-rgbcolor.md)
- [Тип учетной записи, от имени которой запускается приложение](intune-shared-runasaccounttype.md)
- [Состояние выполнения](intune-shared-runstate.md)
- [Сохраненные параметры создания состояния пользовательского интерфейса](intune-shared-saveduistategenerationoptions.md)
- [URI](intune-shared-uri.md)
- [user](intune-shared-user.md)
- [Тип учетной записи токена VPP](intune-shared-vpptokenaccounttype.md)
- [Причина сбоя действия с токеном VPP](intune-shared-vpptokenactionfailurereason.md)
- [Конфигурация присоединения к домену Windows](intune-shared-windowsdomainjoinconfiguration.md)
