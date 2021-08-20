---
title: тип enum deviceManagementConfigurationTechnologies
description: Описывает, какую технологию можно развернуть с помощью этого параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9c935c1f69e843940a9e4aa29199dbfd9b5a02aa3528f7612c72055ab3f2efbc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54185798"
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
|mdm|1 |Параметр можно развернуть через канал MDM|
|windows10XManagement|2|Параметр можно развернуть через канал Windows10XManagement|
|configManager|4 |Параметр можно развернуть через канал ConfigManager|
|MicrosoftSense|128|Настройка может быть развернута через канал агента SENSE|




