---
title: тип enum deviceEnrollmentConfigurationType
description: Описывает объект TemplateFamily для объекта Template
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 85ffeb3b0d8215309b0667be4e0ba874aad66bfa
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63378775"
---
# <a name="deviceenrollmentconfigurationtype-enum-type"></a>тип enum deviceEnrollmentConfigurationType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает объект TemplateFamily для объекта Template

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Значение, используемое по умолчанию. Установить неизвестно, не удается ли определить тип конфигурации.|
|limit|1|Указывает, что конфигурация имеет ограничение типа, которое относится к числу устройств, которые разрешено зарегистрировать пользователю.|
|platformRestrictions|2|Указывает, что конфигурация — это ограничение платформы типа, которое относится к типам устройств, которые разрешено зарегистрировать пользователю.|
|windowsHelloForBusiness|3|Указывает, что конфигурация имеет тип Windows Hello, который относится к устройствам метода проверки подлинности.|
|defaultLimit|4|Указывает, что конфигурация имеет ограничение по умолчанию типа, которое относится к типам устройств, которые пользователь может зарегистрироваться по умолчанию.|
|defaultPlatformRestrictions|5|Указывает, что конфигурация является ограничением платформы типа по умолчанию, которое относится к типам устройств, которые пользователь может зарегистрироваться по умолчанию.|
|defaultWindowsHelloForBusiness|6 |Указывает, что конфигурация имеет тип Windows Hello, который относится к устройствам метода проверки подлинности, которые будут использовать по умолчанию.|
|defaultWindows10EnrollmentCompletionPageConfiguration|7 |Указывает, что конфигурация — это страница состояния состояния типа по умолчанию, которая относится к странице запуска, отображаемой во время OOBE в устройствах Автопилота по умолчанию.|
|windows10EnrollmentCompletionPageConfiguration|8 |Указывает, что конфигурация — это страница состояния регистрации типа, которая относится к странице запуска, отображаемой во время OOBE на устройствах Автопилота.|
|deviceComanagementAuthorityConfiguration|9 |Указывает, что конфигурация имеет тип Comanagement Authority, который относится к политикам, применяемым Co-Managed устройствам.|
|singlePlatformRestriction|10 |Указывает, что конфигурация имеет ограничение одной платформы типа, которое относится к типам устройств, которые разрешено зарегистрировать пользователю.|
|unknownFutureValue|11|Неизвестное будущее значение|




