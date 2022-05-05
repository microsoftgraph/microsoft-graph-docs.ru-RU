---
title: Тип перечисления deviceEnrollmentConfigurationType
description: Описывает TemplateFamily для сущности Template
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 98fef8c27ca10a613c02132a4cd80fb8ab909205
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211321"
---
# <a name="deviceenrollmentconfigurationtype-enum-type"></a>Тип перечисления deviceEnrollmentConfigurationType

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает TemplateFamily для сущности Template

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Значение, используемое по умолчанию. Задайте значение unknown, если не удается определить тип конфигурации.|
|limit|1|Указывает, что конфигурация имеет ограничение типа, которое относится к количеству устройств, которые пользователь может зарегистрировать.|
|platformRestrictions|2|Указывает, что конфигурация имеет ограничение платформы типа, которое относится к типам устройств, которые пользователь может зарегистрировать.|
|windowsHelloForBusiness|3|Указывает, что конфигурация имеет тип Windows Hello, который ссылается на метод проверки подлинности, который будут использовать устройства.|
|defaultLimit|4|Указывает, что конфигурация имеет ограничение по умолчанию типа, которое относится к типам устройств, которые пользователь может зарегистрировать по умолчанию.|
|defaultPlatformRestrictions|5|Указывает, что конфигурация имеет ограничение платформы по умолчанию, которое относится к типам устройств, которые пользователь может зарегистрировать по умолчанию.|
|defaultWindowsHelloForBusiness|6 |Указывает, что конфигурация имеет тип по умолчанию Windows Hello который ссылается на метод проверки подлинности, используемый устройствами по умолчанию.|
|defaultWindows10EnrollmentCompletionPageConfiguration|7 |Указывает, что конфигурация имеет тип страницы состояния регистрации по умолчанию, которая ссылается на страницу запуска, отображаемую во время запуска при первом включении в устройствах Autopilot по умолчанию.|
|windows10EnrollmentCompletionPageConfiguration|8 |Указывает, что конфигурация имеет тип страницы состояния регистрации, которая ссылается на страницу запуска, отображаемую во время запуска при первом включении в устройствах Autopilot.|
|deviceComanagementAuthorityConfiguration|9 |Указывает, что конфигурация имеет тип "Comanagement Authority", который ссылается на политики, применяемые к Co-Managed устройствам.|
|singlePlatformRestriction|10|Указывает, что конфигурация относится к типу ограничения одной платформы, которое относится к типам устройств, которые пользователь может зарегистрировать.|
|unknownFutureValue|11|Неизвестное будущее значение|
|enrollmentNotificationsConfiguration|12 |Указывает, что конфигурация относится к типам уведомлений о регистрации, которые ссылается на типы уведомлений, получаемые пользователем во время регистрации.|




