---
title: тип enum deviceManagementConfigurationTechnologies
description: Описывает, какую технологию можно развернуть с помощью этого параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a87452e3f00887895e8a89a2b845e077a25f7bf7
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60485172"
---
# <a name="devicemanagementconfigurationtechnologies-enum-type"></a>тип enum deviceManagementConfigurationTechnologies

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает, какую технологию можно развернуть с помощью этого параметра

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Настройка не может быть развернута по любому каналу|
|mdm|1|Параметр можно развернуть через канал MDM|
|windows10XManagement|2|Параметр можно развернуть через канал Windows10XManagement|
|configManager|4 |Параметр можно развернуть через канал ConfigManager|
|MicrosoftSense|128|Настройка может быть развернута через канал агента SENSE|
|exchangeOnline|256|Параметр можно развернуть через канал Exchange Online агента|
|LinuxMdm|1024|Параметр можно развернуть через канал Linux Mdm|
|unknownFutureValue|1073741824|Член Sentinel для случаев, когда клиент не может обрабатывать новые значения в переуме.|



