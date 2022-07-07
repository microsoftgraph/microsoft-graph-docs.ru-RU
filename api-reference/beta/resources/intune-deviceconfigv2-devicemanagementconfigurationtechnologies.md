---
title: Тип перечисления deviceManagementConfigurationTechnologies
description: Описывает технологию, с помощью которой можно развернуть этот параметр
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d9d65d7e2bb44f6886be35362d2de07386ec84b
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670543"
---
# <a name="devicemanagementconfigurationtechnologies-enum-type"></a>Тип перечисления deviceManagementConfigurationTechnologies

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает технологию, с помощью которой можно развернуть этот параметр

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|none|0|Параметр не может быть развернут по любому каналу|
|Mdm|1|Параметр можно развернуть через канал MDM|
|windows10XManagement|2|Параметр можно развернуть через канал Windows10XManagement|
|configManager|4|Параметр можно развернуть через канал ConfigManager|
|appleRemoteManagement|64|Параметр можно развернуть через канал AppleRemoteManagement|
|microsoftSense|128|Параметр можно развернуть через канал агента SENSE|
|exchangeOnline|256|Параметр можно развернуть через канал Exchange Online агента|
|linuxMdm|1024|Параметр можно развернуть через канал Linux Mdm.|
|Регистрации|4096|Параметр можно развернуть с помощью регистрации устройства.|
|unknownFutureValue|1073741824|Член Sentinel в случаях, когда клиент не может обработать новые значения перечисления.|




