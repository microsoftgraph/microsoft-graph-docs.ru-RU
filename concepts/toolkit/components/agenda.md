---
title: Компонент "Повестка дня" в Microsoft Graph Toolkit
description: Веб-компонент mgt-agenda используется для представления событий в календаре пользователя или группы.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b4c9f41f347e8a392d7d751f16f9168a4d66d1c4
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266577"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a>Компонент "Повестка дня" в Microsoft Graph Toolkit

Веб-компонент `mgt-agenda` отображает события в календаре пользователя или группы. По умолчанию в календаре отображаются текущие события вошедшего пользователя, запланированные на текущий день. Компонент также может использовать любую конечную точку, возвращающую события из Microsoft Graph.

## <a name="example"></a>Пример

В следующем примере показаны события календаря вошедшего пользователя, отображаемые с помощью компонента `mgt-agenda`. Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[Открыть этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a>Свойства

По умолчанию компонент `mgt-agenda` извлекает события из конечной точки `/me/calendarview` и отображает события, запланированные на текущий день. Это поведение можно изменить с помощью нескольких свойств.

| Атрибут | Свойство | Описание |
| --- | --- | --- |
| дата | date | Строка, представляющая дату начала событий, извлекаемых из Microsoft Graph. Значение должно быть в формате, который может быть проанализирован [конструктором дат](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date). Значение не оказывает влияния, если установлен атрибут `event-query`. |
| days | days | Количество дней, извлекаемых из Microsoft Graph (по умолчанию — 3 дня). Значение не оказывает влияния, если установлен атрибут `event-query`. |
| show-max | showMax | Число, указывающее максимальное количество отображаемых событий. Значение по умолчанию не установлено (не ограничено). |
| group-id | groupId | Идентификатор строки для группового календаря, используемого вместо текущего календаря вошедшего пользователя. |
| event-query | eventQuery | Строка, представляющая альтернативный запрос, используемый при извлечении событий из Microsoft Graph. При необходимости добавьте делегированную область в конец строки, разделив ее с помощью символа `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`). |
| events | events | Массив событий для получения или установки списка событий, отображаемых компонентом. Используйте это свойство для доступа к событиям, загружаемым компонентом. Установите это значение, чтобы загрузить свои собственные события. Если значение установлено разработчиком, атрибуты `date`, `days` и `event-query` не оказывают влияния. |
| group-by-day | groupByDay | Логическое значение для группировки событий по дням (по умолчанию события не группируются). |
| preferred-timezone | preferredTimezone | Имя предпочтительного часового пояса, используемого при извлечении событий из Microsoft Graph. Например, `Pacific Standard Time`. По умолчанию этот атрибут использует время в формате UTC. Предпочтительный часовой пояс для текущего пользователя можно получить, вызвав конечную точку `me/mailboxSettings` и прочитав значение свойства **timeZone**. |

Следующий пример демонстрирует изменение поведения компонента для извлечения данных за определенную дату и до трех дней.

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

Следующий пример демонстрирует изменение поведения компонента для извлечения данных из определенного запроса.

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="methods"></a>Методы
| Метод | Описание |
| --- | --- |
| reload() | Вызывает метод для перезагрузки компонента с потенциальными новыми данными на основе его свойств. |

## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

Компонент `mgt-agenda` определяет следующие настраиваемые свойства CSS.

```css
mgt-agenda {
  --event-box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.092);
  --event-margin: 0px 10px 14px 10px;
  --event-padding: 8px 0px;
  --event-background-color: #ffffff;
  --event-border: solid 2px rgba(0, 0, 0, 0);

  --agenda-header-margin: 40px 10px 14px 10px;
  --agenda-header-font-size: 24px;
  --agenda-header-color: #333333;

  --event-time-font-size: 12px;
  --event-time-color: #000000;

  --event-subject-font-size: 19px;
  --event-subject-color: #333333;

  --event-location-font-size: 12px;
  --event-location-color: #000000;
}
```

Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).

## <a name="templates"></a>Шаблоны

Компонент `mgt-agenda` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить его определенные части. Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.

| Тип данных | Контекст данных | Описание |
| --- | --- | --- |
| `default` | `events`: список объектов события | Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом. |
| `event` | `event`: объект события | Шаблон, используемый для отображения каждого события. |
| `event-other` | `event`: объект события | Шаблон, используемый для отображения дополнительного содержимого для каждого события. |
| `header` | `header`: строка | Шаблон, используемый для отображения заголовка для каждого дня. |
| `loading` | Контекст данных не передается | Шаблон, используемый при загрузке данных. |
| `no-data` | Контекст данных не передается | Шаблон, используемый при отсутствии событий. |

В следующих примерах показано, как использовать шаблон `event`.

```html
<mgt-agenda>
  <template data-type="event">
    <button class="eventButton">
      <div class="event-subject">{{ event.subject }}</div>
      <div data-for="attendee in event.attendees">
        <mgt-person
          person-query="{{ attendee.emailAddress.name }}"
          view="twolines">
        </mgt-person>
      </div>
    </button>
  </template>
  <template data-type="no-data">
    There are no events found!
  </template>
</mgt-agenda>
```

Дополнительные сведения см. в статье [Шаблоны](../customize-components/templates.md).

## <a name="events"></a>События

Из элемента управления инициируются следующие события.

| Событие | Описание |
| --- | --- |
| eventClick | Пользователь щелкает или нажимает событие.|

## <a name="permissions"></a>Разрешения

Этот компонент использует следующие API и разрешения Microsoft Graph.

| Ресурс | Разрешение |
| - | - |
| [/me/calendarview](/graph/api/calendar-list-calendarview) | Calendars.Read |

Компонент позволяет указать другой запрос Microsoft Graph для вызова (например, `/groups/{id}/calendar/calendarView`). В этом случае добавьте разрешение в конец строки, разделенной символом `|`.

При использовании шаблона по умолчанию и шаблона по умолчанию `renderAttendees`, требуются дополнительные API и разрешения. Шаблон по умолчанию для этого компонента использует компонент [mgt-people](people.md) для событий с участниками, для которого требуется следующие элементы.

| Ресурс | Разрешение |
| - | - |
| [/users](/graph/api/user-list) | Users.ReadBasic.All |
| [/me/calendarview](/graph/api/user-list-people) | People.Read |
| [/me/calendarview](/graph/api/user-list-contacts) | Contacts.Read |

## <a name="authentication"></a>Проверка подлинности

В элементе управления входом используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).

## <a name="cache"></a>Кэш

Компонент `mgt-agenda` не кэшет данных.

## <a name="extend-for-more-control"></a>Расширение для дополнительного управления

В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected` render* для переопределения в расширениях компонента.

| Метод | Описание |
| - | - |
| renderLoading | Отображает состояние загрузки во время загрузки компонента. |
| renderNoData | Отображает пустое состояние данных. |
| renderGroups | Сортирует данные событий по группам и отображает их с заголовками групп. |
| renderHeader | Отображает заголовок группы. |
| renderEvents | Отображает список объектов события. |
| renderEvent | Отображает одно событие и все его части.
| renderTitle | Отображает название события. |
| renderLocation | Отображает расположение события. |
| renderAttendees | Отображает участников события. |
| renderOther | Отображает дополнительное содержимое события. |
