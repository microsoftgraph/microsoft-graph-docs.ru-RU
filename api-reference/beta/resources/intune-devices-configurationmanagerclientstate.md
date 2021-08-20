---
title: тип enum configurationManagerClientState
description: Состояние клиента Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3bcac417f0a0a156a998bd65a50a6baf9697b801a3c8484398fc57ad59fc3f53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251290"
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
|установлено|1 |Агент диспетчера конфигурации установлен, но может еще не появиться на консоли диспетчера конфигурации. Подождите несколько часов, пока она не будет обновлена.|
|здоровый|7 |Это устройство удалось успешно проверить с помощью службы диспетчера конфигурации.|
|installFailed|8 |Агент диспетчера конфигурации не удалось установить.|
|updateFailed|11 |Обновление от версии x до версии y агента диспетчера конфигурации не удалось. |
|communicationError|19|Агенту диспетчера конфигурации удалось достичь службы диспетчера конфигурации в прошлом, но теперь это не удалось. |




