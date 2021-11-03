---
title: тип enum windowsAutopilotProfileAssignmentDetailedStatus
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bd81c03006349bf3401c736c092dbab25e7ca0ac
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696310"
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
|surfaceHubProfileNotSupported|2|Указывает, что Surface Hub автопилота назначен устройству, которое не Surface Hub (Aruba).|
|holoLensProfileNotSupported|3|Указывает, что HoloLens автопилота назначен устройству, которое не HoloLens.|
|windowsPcProfileNotSupported|4 |Указывает, что Windows pc AutoPilot-профиль назначен устройству, которое не Windows ПК.|
|surfaceHub2SProfileNotSupported|5|Указывает, что профиль surface Hub 2S AutoPilot назначен устройству, которое не является surface Hub 2S.|
|unknownFutureValue|99|Местообладатель для эволюционирующего переумыка, но этот переумыватель никогда не возвращается вызываемой, поэтому она не должна быть обязательной.|



