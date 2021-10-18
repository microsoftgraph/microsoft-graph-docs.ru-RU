---
title: тип списка firewallCertificateRevocationListCheckMethodType
description: Возможные значения брандмауэраCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1942fbbe5088e73d648740d7d8a7cb2c86aa7da8
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60446640"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>тип списка firewallCertificateRevocationListCheckMethodType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения брандмауэраCertificateRevocationListCheckMethod

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Нет значения, настроенного Intune, не переопределять настроенное пользователем значение по умолчанию устройства|
|Нет|1|Не проверяйте список отзывов сертификатов|
|попытка|2|Попытка проверки CRL и разрешить сертификат только в том случае, если сертификат подтвержден проверкой|
|требовать|3|Требуется успешная проверка CRL перед разрешением сертификата|



