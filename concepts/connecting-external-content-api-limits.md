---
title: Ограничения API соединителей Microsoft Graph
description: Реализация и эксплуатационные ограничения для соединителей Microsoft Graph.
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: e50085b8c59e304c852f8f75c326fca2967a54f9
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296467"
---
# <a name="microsoft-graph-connectors-api-limits"></a>Ограничения API соединителей Microsoft Graph

В этой статье описаны реализация и эксплуатационные ограничения для соединителей Microsoft Graph. При разработке соединителей помните об этих ограничениях.

## <a name="connection-limits"></a>Ограничения подключений

| Тип ограничения | Ограничение |
| ---------- | ----- |
| Ресурсы [подключения](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-1.0&preserve-view=true) для каждого клиента Microsoft 365 | 10 |
| [Элементов](/graph/api/resources/externalconnectors-externalitem?view=graph-rest-1.0&preserve-view=true) на соединение | 700 000 |
| Размер соединения в байтах | 70 ГБ |

## <a name="schema-limits"></a>Ограничения схемы

| Тип ограничения | Ограничение |
| ---------- | ----- |
| Свойства, которые можно определить в [схеме](/graph/api/resources/externalconnectors-schema?view=graph-rest-1.0&preserve-view=true), характеризующие данные, получаемые через соединение. | 128 |

## <a name="group-limits"></a>Ограничения для групп

| Тип ограничения | Ограничение |
| ---------- | ----- |
| [Внешние группы](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-1.0&preserve-view=true) на каждого клиента Microsoft 365 | 100,000 | 
| Разрешенные запросы в секунду (запросы/сек) в пороге [регулирования количества запросов](#throttling) группового администрирования | 1 000 |

## <a name="item-ingestion"></a>Прием элементов

| Тип ограничения | Ограничение |
| ---------- | ----- |
| Ограничение пропускной способности для приема элементов через соединение | 4 элемента/с <br> (250 МБ/ч) |
| Размер элемента; это ограничение применяется к телу запроса при [приеме и индексировании элемента](/graph/api/externalconnectors-externalconnection-put-items?view=graph-rest-beta&preserve-view=true&tabs=http&viewFallbackFrom=graph-rest-1.0). | 4 МБ |
| Размер свойства | Недоступно |

## <a name="throttling"></a>Регулирование

При превышении порога [регулирования](throttling.md) Microsoft Graph ограничивает любые дальнейшие запросы от этого клиента в течение определенного периода времени. При регулировании Microsoft Graph возвращает код состояния HTTP 429 (слишком много запросов), и запросы завершаются сбоем. Предлагаемое время ожидания возвращается в заголовке отклика неудачного запроса.

Поведение регулирования может зависеть от типа и количества запросов. Например, если у вас большой объем запросов, все типы запросов регулируются. Пороговые ограничения зависят от типа запроса. Таким образом, вы можете столкнуться со сценарием, в котором записи регулируются, но чтение по-прежнему разрешено.
