---
title: тип enum windowsUpdateStatus
description: Windows для состояния устройств конфигурации бизнеса
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b07580a4057ba79e932a442d38bac323936df751
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075391"
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



