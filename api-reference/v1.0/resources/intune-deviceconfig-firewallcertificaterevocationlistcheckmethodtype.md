---
title: Тип перечисления firewallCertificateRevocationListCheckMethodType
description: Возможные значения для firewallCertificateRevocationListCheckMethod
author: tfitzmac
ms.openlocfilehash: ab496b5deb8f096bdc48a2b50a1af994c8ec8d5b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353664"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>Тип перечисления firewallCertificateRevocationListCheckMethodType

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для firewallCertificateRevocationListCheckMethod
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию|
|none|1|Не проверять списка отзыва сертификатов|
|Попытка|2|Попытайтесь проверки списка отзыва Сертификатов и разрешить сертификат только в том случае, если сертификат подтверждается при проверке|
|Требовать|3|Требовать успешной проверки списка отзыва Сертификатов, перед тем как разрешить сертификата|



