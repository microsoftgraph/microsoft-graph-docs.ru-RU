---
title: тип enum configurationManagerClientState
description: Состояние клиента Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2cd31d7d2cde3e3e22a13bdfae3c7ed47b4fcbaa
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58757960"
---
# <a name="configurationmanagerclientstate-enum-type"></a>тип enum configurationManagerClientState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние клиента Configuration Manager

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Агент диспетчера конфигурации старше 1806 или не установлен, или это устройство не проверялось в Intune более 30 дней.|
|установлено|1|Агент диспетчера конфигурации установлен, но может еще не появиться на консоли диспетчера конфигурации. Подождите несколько часов, пока она не будет обновлена.|
|здоровый|7 |Это устройство удалось успешно проверить с помощью службы диспетчера конфигурации.|
|installFailed|8 |Агент диспетчера конфигурации не удалось установить.|
|updateFailed|11 |Обновление от версии x до версии y агента диспетчера конфигурации не удалось. |
|communicationError|19|Агенту диспетчера конфигурации удалось достичь службы диспетчера конфигурации в прошлом, но теперь это не удалось. |



