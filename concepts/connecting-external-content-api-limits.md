---
title: Ограничения API соединителей Microsoft Graph
description: Реализация и эксплуатационные ограничения для соединителей Microsoft Graph.
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 88cd4d08db4b903e188c82dd38c8d5b89131887f
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247338"
---
# <a name="microsoft-graph-connectors-api-limits"></a>Ограничения API соединителей Microsoft Graph

В этой статье описаны реализация и эксплуатационные ограничения для соединителей Microsoft Graph. При разработке соединителей помните об этих ограничениях.

## <a name="connection-limits"></a>Ограничения подключений

| **Ограничение** | **Описание** |
| --------- | --------------- |
| **10 подключений** | Максимальное количество ресурсов [подключений](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-1.0&preserve-view=true) на клиента Microsoft 365. |
| **700 000 элементов** | Максимальное количество [элементов](/graph/api/resources/externalconnectors-externalitem?view=graph-rest-1.0&preserve-view=true) на подключение. |
| **70 ГБ** | Максимальное количество байтов подключения. |

## <a name="schema-limits"></a>Ограничения схемы

| **Ограничение** | **Описание** |
| --------- | --------------- |
| **128 свойств** | Максимальное количество свойств, которые можно определить в [схеме](/graph/api/resources/externalconnectors-schema?view=graph-rest-1.0&preserve-view=true), характеризующих данные, полученные через подключение. |

## <a name="group-limits"></a>Ограничения для групп

| **Ограничение** | **Описание** |
| --------- | --------------- |
| **100,000** | Максимальное количество [внешних групп](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-1.0&preserve-view=true) на клиента Microsoft 365. |
| **1000 запросов/с** | Максимальное количество запросов, разрешенных в секунду в пороге[регулирования](#throttling) администрирования группы. |

## <a name="item-ingestion"></a>Прием элементов

| **Ограничение** | **Описание** |
| --------- | --------------- |
| **4 элемента/с (250 МБ в час)** | Ограничение пропускной способности для приема элементов через подключение. |
| **4 МБ** | Максимальный размер элемента; это ограничение применяется к телу запроса при [приеме и индексации элемента](/graph/api/externalconnectors-externalconnection-put-items?view=graph-rest-beta&preserve-view=true&tabs=http&viewFallbackFrom=graph-rest-1.0). |
| **Н/Д** | Максимальный размер свойства. |

## <a name="throttling"></a>Регулирование

При превышении порога [регулирования](throttling.md) Microsoft Graph ограничивает любые дальнейшие запросы от этого клиента в течение определенного периода времени. При регулировании Microsoft Graph возвращает код состояния HTTP 429 (слишком много запросов), и запросы завершаются сбоем. Предлагаемое время ожидания возвращается в заголовке отклика неудачного запроса.

Поведение регулирования может зависеть от типа и количества запросов. Например, если у вас большой объем запросов, все типы запросов регулируются. Пороговые ограничения зависят от типа запроса. Таким образом, вы можете столкнуться со сценарием, в котором записи регулируются, но чтение по-прежнему разрешено.
