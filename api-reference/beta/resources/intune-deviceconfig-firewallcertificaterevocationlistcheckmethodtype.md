---
title: тип списка firewallCertificateRevocationListCheckMethodType
description: Возможные значения брандмауэраCertificateRevocationListCheckMethod
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 36810f72095d955b40e6e1c288f8d175d24de88b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075475"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>тип списка firewallCertificateRevocationListCheckMethodType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения брандмауэраCertificateRevocationListCheckMethod

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Нет значения, настроенного Intune, не переопределять настроенное пользователем значение по умолчанию устройства|
|Нет|1|Не проверяйте список отзывов сертификатов|
|попытка|2|Попытка проверки CRL и разрешить сертификат только в том случае, если сертификат подтвержден проверкой|
|требовать|3|Требуется успешная проверка CRL перед разрешением сертификата|



