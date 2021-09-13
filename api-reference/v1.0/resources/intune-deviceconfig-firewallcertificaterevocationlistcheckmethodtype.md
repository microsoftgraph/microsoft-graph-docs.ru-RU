---
title: тип списка firewallCertificateRevocationListCheckMethodType
description: Возможные значения брандмауэраCertificateRevocationListCheckMethod
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9bc65e8f210d3d2a7cba2754e2d73ea2a448206e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139837"
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




