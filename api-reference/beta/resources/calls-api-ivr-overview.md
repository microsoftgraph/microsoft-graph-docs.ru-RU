---
title: Сценарии IVR в вызовах
description: Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 3b33a673218238f861e7122de8320d6c8a20e435
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042732"
---
# <a name="ivr-scenarios-in-calls"></a>Сценарии IVR в вызовах

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.

- Воспроизведение звуковых запросов, например, при поступлении вызова в очередь агента обслуживания клиентов.
- Запись ответа, например, для записи звука вызывающего абонента, как правило, после того, как он слышал приглашение с параметрами.
- Подписываться на звуки, например, если вы хотите узнать, какие звуки DTMF выбрал абонент, обычно после проявления звукового приглашения.
- Отмена обработки мультимедиа — например, если вы хотите отменить все операции Плайпромпт или Рекордреспонсе, которые могут быть в процессе выполнения.


