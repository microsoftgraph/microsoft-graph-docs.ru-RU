---
title: Компонент "Повестка дня" в microsoft Graph набор средств
description: Веб-компонент mgt-agenda используется для представления событий в календаре пользователя или группы.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e66ffed1f10de5c4c9b9b322d9070074ec707000
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659550"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a>Компонент "Повестка дня" в microsoft Graph набор средств

`mgt-agenda`Веб-компонент представляет события в календаре пользователя или группы. По умолчанию в календаре отображаются текущие события, в которые были вписались пользователи за текущий день. Компонент также может использовать любую конечную точку, которая возвращает события из Microsoft Graph.

## <a name="example"></a>Пример

В следующем примере показаны события календаря пользователя, выписав его с помощью `mgt-agenda` компонента. С помощью редактора кода можно [увидеть,](#properties) как свойства изменяют поведение компонента.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[Откройте этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a>Свойства

По умолчанию компонент получает события из конечной точки и отображает события `mgt-agenda` `/me/calendarview` за текущий день. Существует несколько свойств, которые можно использовать для изменения этого поведения.

| Атрибут | Свойство | Описание |
| --- | --- | --- |
| дата | date | Строка, представляючная дату начала событий, извлекаемой из Microsoft Graph. Значение должно быть в формате, который может быть разбор с помощью конструктора [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) — значение не имеет эффекта, если `event-query` атрибут установлен. |
| days | days | Количество дней, за которые необходимо получить данные из Microsoft Graph (значение по умолчанию — 3), не влияет на значение, если `event-query` за установлен атрибут. |
| show-max | showMax | Число, чтобы указать максимальное число событий для показа. Значение по умолчанию не за установлено (не максимальное значение). |
| group-id | groupId | ИД строки для календаря группы вместо текущего календаря пользователя, выписав его. |
| event-query | eventQuery | Строка, представляютив альтернативный запрос, используемый при извлечении событий из Microsoft Graph. При желании добавьте делегированную область в конце строки, делегированием ее с `|` помощью ( `/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all` ). |
| events | events | Массив событий, чтобы получить или установить список событий, отрисовки компонента . Используйте это свойство для доступа к событиям, загруженным компонентом. Установите это значение для загрузки собственных событий — если значение за установлено разработчиком, атрибуты `date` , или не имеют `days` `event-query` эффекта. |
| группировка по дням | groupByDay | Boolean value to group events by day - by default events are not grouped. |
| preferred-timezone | preferredTimezone | Имя предпочтительного часового пояса, используемого при искомом событиях из Microsoft Graph; например, `Pacific Standard Time` . По умолчанию этот атрибут использует часовой пояс UTC. Предпочтительный часовой пояс для текущего пользователя можно получить, вызывая конечную точку и считывая значение `me/mailboxSettings` **свойства timeZone.** |

В следующем примере изменяется поведение компонента для получения данных за определенную дату и до трех дней.

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

В следующем примере изменяется поведение компонента для получения данных из определенного запроса.

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="methods"></a>Методы
| Метод | Описание |
| --- | --- |
| reload() | Вызовите метод, чтобы перезагрузить компонент с потенциальными новыми данными на основе его свойств. |

## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

Компонент `mgt-agenda` определяет эти настраиваемые свойства CSS

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

Дополнительные узнать см. [в компонентах стиля.](../customize-components/style.md)

## <a name="templates"></a>Шаблоны

Компонент `mgt-agenda` поддерживает несколько [шаблонов,](../customize-components/templates.md) которые позволяют заменить определенные части компонента. Чтобы указать шаблон, включив элемент в компонент и заключив в него одно `<template>` `data-type` из следующих значений:

| Тип данных | Контекст данных | Описание |
| --- | --- | --- |
| `default` | `events`: список объектов событий | Шаблон по умолчанию заменяет весь компонент на собственный. |
| `event` | `event`: объект event | Шаблон, используемый для отображения каждого события. |
| `event-other` | `event`: объект event | Шаблон, используемый для отображения дополнительного содержимого для каждого события. |
| `header` | `header`: string | Шаблон, используемый для отображения загона для каждого дня. |
| `loading` | Контекст данных не передается | Шаблон, используемый при загрузке данных. |
| `no-data` | Контекст данных не передается | Шаблон, используемый, когда события недоступны. |

В следующих примерах показано, как использовать `event` шаблон:

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

Дополнительные узнать см. [в шаблонах.](../customize-components/templates.md)

## <a name="events"></a>События

Из этого управления и происходят следующие события.

| Событие | Описание |
| --- | --- |
| eventClick | Пользователь щелкает или кжимает событие.|

## <a name="permissions"></a>Разрешения

Этот компонент использует следующие API Microsoft Graph и разрешения:

| Ресурс | Разрешение |
| - | - |
| [/me/calendarview](/graph/api/calendar-list-calendarview) | Calendars.Read |

Компонент позволяет указать другой запрос Microsoft Graph для вызова `/groups/{id}/calendar/calendarView` (например, ). В этом случае примените разрешение в конец строки с делегированный по `|` .

При использовании шаблона по умолчанию и шаблона по умолчанию требуются дополнительные API и `renderAttendees` разрешения. Шаблон по умолчанию для этого компонента использует компонент [mgt-people](people.md) для событий с участниками, для чего требуется следующее.

| Ресурс | Разрешение |
| - | - |
| [/users](/graph/api/user-list) | Users.ReadBasic.All |
| [/me/calendarview](/graph/api/user-list-people) | People.Read |
| [/me/calendarview](/graph/api/user-list-contacts) | Contacts.Read |

## <a name="authentication"></a>Проверка подлинности

Для управления входом используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности.](../providers/providers.md)

## <a name="extend-for-more-control"></a>Расширение для большего контроля

Для более сложных сценариев или по-настоящему настраиваемого пользовательского пользовательского управления этот компонент предоставляет несколько методов render* для переопределения `protected` в расширениях компонентов.

| Метод | Описание |
| - | - |
| renderLoading | Отрисовка состояния загрузки во время загрузки компонента. |
| renderNoData | Отрисовка пустого состояния данных. |
| renderGroups | Сортировать данные событий по группам и отрисовки их с помощью заглавных групп. |
| renderHeader | Отрисовка загона группы. |
| renderEvents | Отрисовка списка объектов событий. |
| renderEvent | Отрисовка события в единственном числе и всех его частей.
| renderTitle | Отрисовка части заголовка события. |
| renderLocation | Отрисовка части расположения события. |
| renderAttendees | Отрисовка части участников события. |
| renderOther | Отрисовка дополнительного содержимого события. |
