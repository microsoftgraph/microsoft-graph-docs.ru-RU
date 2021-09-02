---
title: тип enum androidDeviceOwnerAppAutoUpdatePolicyType
description: Владелец Android Device возможные значения для состояния политики автоматического обновления приложения на устройстве.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bc427cb78e3a008f1fb2cc856217648bbb670015
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58779202"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a>тип enum androidDeviceOwnerAppAutoUpdatePolicyType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Владелец Android Device возможные значения для состояния политики автоматического обновления приложения на устройстве.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Не настроен; это значение игнорируется.|
|userChoice|1|Пользователь может управлять автоматическими обновлениями.|
|никогда|2|Приложения никогда не обновляются автоматически.|
|wiFiOnly|3|Приложения обновляются автоматически только Wi-Fi.|
|всегда|4 |Приложения обновляются автоматически в любое время. Могут применяться сборы за данные.|



