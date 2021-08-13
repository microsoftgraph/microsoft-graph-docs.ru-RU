---
title: тип списка firewallCertificateRevocationListCheckMethodType
description: Возможные значения брандмауэраCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4cc592c2213cef70af497c9f3f4779bcae88e5694599a5d0f3fff50ac7d8b56e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189585"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>тип списка firewallCertificateRevocationListCheckMethodType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения брандмауэраCertificateRevocationListCheckMethod

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Нет значения, настроенного Intune, не переопределять настроенное пользователем значение по умолчанию устройства|
|нет|1|Не проверяйте список отзывов сертификатов|
|попытка|2|Попытка проверки CRL и разрешить сертификат только в том случае, если сертификат подтвержден проверкой|
|требовать|3|Требуется успешная проверка CRL перед разрешением сертификата|




