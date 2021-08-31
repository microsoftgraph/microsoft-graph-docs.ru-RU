---
title: тип enum windowsAutopilotProfileAssignmentDetailedStatus
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6334c94a89b22a0cd2a02d2e8abfd92e97f21313
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788432"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a>тип enum windowsAutopilotProfileAssignmentDetailedStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Подробный статус назначения не|
|hardwareRequirementsNotMet|1|Требования к оборудованию не выполнены. Это может произойти, если на устройстве без TPM 2.0 будет назначен саморазверяющийся профиль АвтоПилота.|
|surfaceHubProfileNotSupported|2|Это может произойти, если профиль автопилота SurfaceHub назначен устройству, которое не SurfaceHub.|
|holoLensProfileNotSupported|3|Это может произойти, HoloLens профиль автопилота назначен устройству, которое не HoloLens.|
|windowsPcProfileNotSupported|4 |Это может произойти, если профиль автопилота WindowsPc назначен устройству, которое не является WindowsPc.|



