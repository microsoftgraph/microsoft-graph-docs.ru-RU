---
title: тип списка firewallCertificateRevocationListCheckMethodType
description: Возможные значения брандмауэраCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: eccba100b33e902bc7704a6f0fa3ff080b74b4aa8288b8d848b0eb0d229c43d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54232785"
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
|Нет|1 |Не проверяйте список отзывов сертификатов|
|попытка|2|Попытка проверки CRL и разрешить сертификат только в том случае, если сертификат подтвержден проверкой|
|требовать|3 |Требуется успешная проверка CRL перед разрешением сертификата|




