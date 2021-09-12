---
title: тип enum androidDeviceOwnerAppAutoUpdatePolicyType
description: Владелец Android Device возможные значения для состояния политики автоматического обновления приложения на устройстве.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9dcb3b22bd1a58f846ea696cfe88566478814a58
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017564"
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



