---
title: тип enum deviceManagementConfigurationTechnologies
description: Описывает, какую технологию можно развернуть с помощью этого параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d79bf933623e94d48013d3259326fdd45a9115bf
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806238"
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



