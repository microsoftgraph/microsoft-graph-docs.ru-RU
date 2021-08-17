---
title: тип enum windowsUpdateStatus
description: Windows для состояния устройств конфигурации бизнеса
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7da061fafd5ed59c215031b2e2626c8d0d42a50661089e9646455ae6d96c4668
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54213160"
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
|pendingInstallation|1 |Есть обновления, ожидающих установки, которые включают обновления, которые не утверждены. Не существует ожидающих обновлений перезагрузки, не сбойных обновлений.|
|pendingReboot|2|Есть обновления, которые требуют перезагрузки. Обновления не являются сбойными.|
|не удалось|3 |На устройстве не удалось установить обновления.|




