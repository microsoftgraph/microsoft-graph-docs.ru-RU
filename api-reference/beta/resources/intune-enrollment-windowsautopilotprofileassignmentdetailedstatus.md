---
title: тип enum windowsAutopilotProfileAssignmentDetailedStatus
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ceb929b2200c5f47b7aefd421feb1a7f19100228
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054270"
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



