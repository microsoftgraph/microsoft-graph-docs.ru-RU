---
title: Сценарии IVR в вызовах
description: Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 4ebb278981ef066aae409d3cc276046a04f79806
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870934"
---
# <a name="ivr-scenarios-in-calls"></a>Сценарии IVR в вызовах

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.

- Воспроизведение звуковых запросов, например, при поступлении вызова в очередь агента обслуживания клиентов.
- Запись ответа, например, для записи звука вызывающего абонента, как правило, после того, как он слышал приглашение с параметрами.
- Подписываться на звуки, например, если вы хотите узнать, какие звуки DTMF выбрал абонент, обычно после проявления звукового приглашения.
- Отмена обработки мультимедиа — например, если вы хотите отменить все операции Плайпромпт или Рекордреспонсе, которые могут быть в процессе выполнения.
