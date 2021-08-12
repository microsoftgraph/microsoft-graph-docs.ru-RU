---
title: Сценарии IVR в звонках
description: 'Ниже приводится сценарий интерактивного голосового ответа (IVR), поддерживаемый службами API Graph Microsoft:'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: cbf46e81d537c704e6225a6d756140dd3ce8221fc70a7e86f188cead4ec9d3e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54238190"
---
# <a name="ivr-scenarios-in-calls"></a>Сценарии IVR в звонках

Пространство имен: microsoft.graph

Ниже приводится сценарий интерактивного голосового ответа (IVR), поддерживаемый службами API Graph Microsoft:

- Воспроизведение звуковой подсказки , например, при размещении вызова в очереди агента по обслуживанию клиентов.
- Запись ответа , например, для записи звука вызываемого, как правило, после того, как они услышали запрос с вариантами.
- Подписка на тона — например, если вы хотите знать, какие DTMF тонизирует выбранный вызывающий, как правило, после того, как выслушали звуковой запрос.
- Отмена обработки мультимедиа — например, при отмене любых операций playPrompt или recordResponse, которые могут быть в процессе.
