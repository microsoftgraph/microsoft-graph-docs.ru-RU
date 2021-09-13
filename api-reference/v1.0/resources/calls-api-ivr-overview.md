---
title: Сценарии IVR в звонках
description: 'Ниже приводится сценарий интерактивного голосового ответа (IVR), поддерживаемый службами API Graph Microsoft:'
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: d8b08455e417b228fa22faf6083f721d342ee7ed
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59053141"
---
# <a name="ivr-scenarios-in-calls"></a>Сценарии IVR в звонках

Пространство имен: microsoft.graph

Ниже приводится сценарий интерактивного голосового ответа (IVR), поддерживаемый службами API Graph Microsoft:

- Воспроизведение звуковой подсказки , например, при размещении вызова в очереди агента по обслуживанию клиентов.
- Запись ответа , например, для записи звука вызываемого, как правило, после того, как они услышали запрос с вариантами.
- Подписка на тона — например, если вы хотите знать, какие DTMF тонизирует выбранный вызывающий, как правило, после того, как выслушали звуковой запрос.
- Отмена обработки мультимедиа — например, при отмене любых операций playPrompt или recordResponse, которые могут быть в процессе.
