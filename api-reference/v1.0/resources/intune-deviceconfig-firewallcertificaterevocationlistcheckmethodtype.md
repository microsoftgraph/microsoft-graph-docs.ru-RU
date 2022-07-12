---
title: Тип перечисления firewallCertificateRevocationListCheckMethodType
description: Возможные значения для firewallCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 37087d4a29d53c57cd2262dd1c3c427f0ee1c714
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66733859"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>Тип перечисления firewallCertificateRevocationListCheckMethodType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для firewallCertificateRevocationListCheckMethod

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Значение, настроенное Intune, не переопределяйте значение по умолчанию для пользовательского устройства.|
|none|1|Не проверяйте список отзыва сертификатов|
|Попытка|2|Попробуйте проверить список отзыва сертификатов и разрешить сертификат только в том случае, если сертификат подтвержден проверкой.|
|Требуют|3|Требовать успешной проверки списка отзыва сертификатов перед разрешением сертификата|





