---
title: тип enum windowsUpdateStatus
description: Windows для состояния устройств конфигурации бизнеса
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 73404f8d01ab6ea047cb94ecc3b21939e4fb3a6c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803807"
---
# <a name="windowsupdatestatus-enum-type"></a>тип enum windowsUpdateStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows для состояния устройств конфигурации бизнеса

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|upToDate|0|Не существует ожидающих обновлений, ожидающих перезагрузки и не сбоя обновлений.|
|pendingInstallation|1|Есть обновления, ожидающих установки, которые включают обновления, которые не утверждены. Не существует ожидающих обновлений перезагрузки, не сбойных обновлений.|
|pendingReboot|2|Есть обновления, которые требуют перезагрузки. Обновления не являются сбойными.|
|не удалось|3|На устройстве не удалось установить обновления.|



