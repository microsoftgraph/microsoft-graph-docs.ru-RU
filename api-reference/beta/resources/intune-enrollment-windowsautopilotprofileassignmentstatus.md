---
title: тип enum windowsAutopilotProfileAssignmentStatus
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 724da31643ccc971d405c224e309bd11d49f8334
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054249"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a>тип enum windowsAutopilotProfileAssignmentStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние неизвестного назначения|
|assignedInSync|1|Успешно назначено в Intune и синхронизируется с Windows пилотной программой|
|назначеноOutOfSync|2|Назначено успешно в Intune и не синхронизируется с Windows автопилотом|
|assignedUnkownSyncState|3|Успешно назначено в Intune и синхронизируется или не синхронизируется с Windows автопилотом|
|notAssigned|4 |Не назначено|
|ожидание|5 |Ожидающих назначения|
|не удалось|6 | Задание не удалось|



