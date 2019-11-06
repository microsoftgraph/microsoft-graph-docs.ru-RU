---
title: Сценарии IVR в вызовах
description: Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 094b0677e243696a1dfe81a3916a863c09e73b92
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006735"
---
# <a name="ivr-scenarios-in-calls"></a>Сценарии IVR в вызовах

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.

- Воспроизведение звуковых запросов, например, при поступлении вызова в очередь агента обслуживания клиентов.
- Запись — например, для записи звука вызывающего абонента, как правило, после того, как он слышал приглашение с параметрами.
- Подпишитесь на тон — например, если вы хотите узнать, какие звуки DTMF выбрал абонент, как правило, после проявления звукового приглашения.
- Отмена обработки мультимедиа — например, если вы хотите отменить все операции Плайпромпт или Record, которые могут быть в процессе.
