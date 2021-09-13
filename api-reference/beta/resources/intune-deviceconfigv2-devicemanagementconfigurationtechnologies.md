---
title: тип enum deviceManagementConfigurationTechnologies
description: Описывает, какую технологию можно развернуть с помощью этого параметра
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d7766d88b7670a4cd0a96a3e4a52a462478a9a41
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148188"
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



