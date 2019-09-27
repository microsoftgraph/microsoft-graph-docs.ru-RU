---
title: Компонент "Выбор людей"
description: Вы можете использовать веб-компонент "центр управления", чтобы выполнить поиск указанного числа людей и отобразить список результатов с помощью Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: d77c6578d79edb60fbba08200dc033f032b39282
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275851"
---
# <a name="people-picker-component"></a>Компонент "Выбор людей"

Вы можете использовать поиск `mgt-people-picker` в веб-компоненте для указанного числа людей и отобразить список результатов с помощью Microsoft Graph. По умолчанию компонент будет выполнять поиск всех пользователей; Кроме того, можно определить свойство Group, чтобы отфильтровать результаты.

Если количество отображаемых людей превышает `show-max` значение, в списке поиска будут отображаться не все возвращенные пользователи.

## <a name="example"></a>Пример

[Пример жсфиддле](https://jsfiddle.net/metulev/jdv38fg0/)

```html
<mgt-people-picker></mgt-people-picker>
```

![Центр управления "Выбор людей"](./images/mgt-people-picker-image.png)

## <a name="properties"></a>Свойства

По умолчанию `mgt-people-picker` компонент получает события от `/me/people` конечной точки. Используйте следующие атрибуты, чтобы изменить это поведение.

| Свойство | Атрибут | Описание                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| шовмакс  | Show — Max  | Числовое значение, указывающее максимальное число людей для отображения. значение по умолчанию — 6.                                                                                             |
| people   | people    | Массив пользователей, который получает или задает список людей, отображаемых компонентом. Используйте это свойство для доступа к пользователям, загруженным компонентом. Присвойте этому параметру значение загрузка собственных пользователей. |
| group    | group     | Строковое значение, принадлежащее определенной группе Microsoft Graph для дальнейшей фильтрации результатов поиска.                                                                            |

Ниже приведен пример.

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

`mgt-people-picker` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот компонент использует указанные ниже API и разрешения Microsoft Graph.

| API                                                                                                              | Разрешение  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/ме/пеопле](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0)                    | People.Read |
| [/граупс/\${groupId}/мемберс](https://docs.microsoft.com/en-us/graph/api/group-list-members?view=graph-rest-1.0) | People.Read |

## <a name="authentication"></a>Проверка подлинности

Элемент управления использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).
