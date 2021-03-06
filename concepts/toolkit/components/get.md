---
title: Компонент Get в Microsoft Graph Toolkit
description: С помощью компонента Get можно создавать любые GET-запросы из Microsoft Graph непосредственно в HTML-коде.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 4ef24d5b5eac0b53029c67dd723ba80c7d0f5bff
ms.sourcegitcommit: d02c438bcd58e8f64bfcd5fba0b40e436b46570e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/04/2021
ms.locfileid: "50101876"
---
# <a name="get-component-in-the-microsoft-graph-toolkit"></a>Компонент Get в Microsoft Graph Toolkit

С помощью `mgt-get` можно создавать любые GET-запросы из Microsoft Graph непосредственно в HTML-коде. Компонент не предоставляет пользовательский интерфейс по умолчанию и требует создания шаблона.

## <a name="example"></a>Пример

В приведенном ниже примере показано использование компонента `mgt-get` для отображения электронной почты пользователя. Вы можете использовать редактор кода, чтобы узнать, как [свойства и атрибуты](#properties-and-attributes) изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-get--get-email&source=docs" height="500"></iframe>

[Открыть этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-get--get-email&source=docs)

## <a name="properties-and-attributes"></a>Свойства и атрибуты

Чтобы изменить поведение компонента, можно использовать несколько атрибутов. Единственным обязательным атрибутом является `resource`.

| Атрибут | Свойство  | Описание |
| --- | --- | --- |
| resource | resource | Ресурс, который требуется получить из Microsoft Graph (например, `/me`). |
| scopes | scopes | Необязательный массив строк, если используется свойство либо область с разделителями-запятыми, при использовании атрибута. Эти области используются компонентом (с поддерживаемым поставщиком), чтобы убедиться в том, что пользователь дал согласие на нужное разрешение. |
| version | version | Необязательная версия API, используемая при выполнении GET-запроса. Значение по умолчанию: `v1.0`.  |
| max-pages | maxPages | Необязательное количество страниц (для ресурсов, поддерживающих разделение на страницы). Значение по умолчанию: 3. При установке значения 0 будут получены все страницы.  |
| polling-rate | pollingRate | Необязательное количество миллисекунд. При активации компонент будет опрашивать URI запроса на наличие обновлений в заданном интервале. При использовании разностного запроса запрос на API-интерфейс дельты будет отправлен в любом случае. Шаблон будет обновляться только при изменении данных. |
| cache-enabled | cacheEnabled | Необязательное логическое значение. При активации указывает на то, что ответ ресурса будет кэшироваться. Переопределяется, если вызывается `refresh()` или используется `pollingRate`. Значение по умолчанию: `false`. |
| cache-invalidation-period | cacheInvalidationPeriod | Необязательное количество миллисекунд. При активации в сочетании с `cacheEnabled`, задержка до окончания периода аннулирования кэша будет изменено этим значением. Значение по умолчанию `0`. Используется период аннулирования по умолчанию. |
| type | type | Необязательный тип ожидаемого ответа. Значение по умолчанию: `json`. Поддерживает `json` или `image` (поддерживаются только для конечных точек, заканчивающихся на `/photo/value$`). |
| Н/Д | response | Нередактируемый ответ в Microsoft Graph, если запрос был успешен.  |
| Н/Д |error| Нередактируемая ошибка в Microsoft Graph, если запрос завершился неудачей. |

## <a name="methods"></a>Методы
| Метод | Описание |
| --- | --- |
| refresh(force?:boolean) | Вызов метода для обновления данных. По умолчанию в пользовательском интерфейсе будет обновляться только в том случае, если данные изменяются. Передайте `true` для принудительного обновления компонента.  |


## <a name="events"></a>События
| Событие | Сведения | Описание |
| --- | --- | --- |
| dataChange | Сведения содержат объекты `response` и `error`. | Возникает при изменении ответа или ошибки. |

## <a name="templates"></a>Шаблоны

Компонент `mgt-get` поддерживает несколько [шаблонов](../customize-components/templates.md), с помощью которых можно определить внешний вид и удобство использования. Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.

| Тип данных | Контекст данных | Описание |
| --- | --- | --- |
| default | Ответ от Microsoft Graph. | Для отображения данных, поступающих из Microsoft Graph, требуется шаблон по умолчанию. |
| value | Элемент данных из возвращаемого `value` массива | Используйте шаблон `value`, а не шаблон `default`, когда ожидается, что в ответе от графа будет указан массив элементов, например, **сообщений**, **файлов** или **пользователей**. Шаблон `value` будет автоматически повторяться для каждого элемента, возвращенного ресурсом. Шаблон `value` также начнет отрисовку элементов сразу после их готовности (в отличие от шаблона по умолчанию).|
| error | Ошибка из Microsoft Graph. | Этот шаблон будет использоваться при ошибке при создании запроса. |
| loading | Н/Д | Этот шаблон используется во время выполнения запроса. |

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Дополнительные сведения о разрешениях см. в [справочнике по разрешениям Microsoft Graph](../../permissions-reference.md). 

## <a name="authentication"></a>Проверка подлинности

Для получения требуемых данных в средстве управления используется глобальный поставщик проверки подлинности, указанный в [документации по проверке подлинности](../providers/providers.md).
