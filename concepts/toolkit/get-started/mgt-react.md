---
title: Компоненты React набор средств Microsoft Graph
description: Компоненты React набор средств Microsoft Graph ( ) позволяют разработчикам React использовать microsoft `mgt-react` Graph набор средств в своих приложениях React.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 6781a894e451e2c4751f151beddcacf4e0cdb608
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658258"
---
# <a name="microsoft-graph-toolkit-react-components"></a>Компоненты React набор средств Microsoft Graph

Компоненты React набор средств Microsoft Graph ( ) позволяют разработчикам React использовать microsoft `mgt-react` Graph набор средств в своих приложениях React. Библиотека обтекает все компоненты Microsoft Graph набор средств и экспортирует их как компоненты React.

## <a name="what-components-can-i-use"></a>Какие компоненты можно использовать?

Библиотека автоматически выдержана из веб-набор средств Microsoft Graph, а все компоненты доступны как компоненты React.

Имена компонентов React содержатся в PascalCase и не содержат `Mgt` префикса. Например, компонент `mgt-person` доступен как , а компонент доступен как `Person` `mgt-people-picker` `PeoplePicker` .

## <a name="installation"></a>Установка 

Для установки используйте одну из следующих команд.

```bash
npm install @microsoft/mgt-react
```

или

```bash
yarn add @microsoft/mgt-react
```

## <a name="usage"></a>Применение

Все компоненты доступны через пакет npm и именуются с помощью PascalCase. Чтобы использовать компонент, сначала импортировать его вверху.

```tsx
import { Person } from '@microsoft/mgt-react';
```

Теперь вы можете использовать `Person` любой элемент JSX в качестве обычного компонента React.

```tsx
<Person personQuery="me" />
```

Все свойства и события со картой точно так же, как они определены в документации по компонентам.

Например, можно установить для свойства `personDetails` объект:

```jsx
const App = (props) => {
  const personDetails = {
    displayName: 'Bill Gates',
  };

  return <Person personDetails={personDetails}></Person>;
};
```

Или зарегистрируйте обработок событий:

```jsx
import { PeoplePicker, People } from '@microsoft/mgt-react';

const App = (props) => {
  const [people, setPeople] = useState([]);

  const handleSelectionChanged = (e) => {
    setPeople(e.target.selectedPeople);
  };

  return
    <div>
      <PeoplePicker selectionChanged={handleSelectionChanged} />
      Selected People: <People people={people} />
    </div>;
};
```

## <a name="templates"></a>Шаблоны

Большинство компонентов набор средств Microsoft Graph [](../customize-components/templates.md) поддерживают шаблоны и позволяют использовать `mgt-react` React для записи шаблонов.

Например, чтобы создать шаблон, который будет использоваться для отображения событий в компоненте, сначала определите компонент, который будет использоваться для `mgt-agenda` отображения события:

```tsx
import { MgtTemplateProps } from '@microsoft/mgt-react';

const MyEvent = (props: MgtTemplateProps) => {
  const { event } = props.dataContext;
  return <div>{event.subject}</div>;
};
```

Затем используйте его в качестве потомка компонента-оболочки и установите для шаблона реквизит `event` .

```tsx
import { Agenda } from '@microsoft/mgt-react';

const App = (props) => {
  return <Agenda>
    <MyEvent template="event">
  </Agenda>
}
```

Этот `template` реквизит позволяет указать шаблон, который необходимо переписать. В этом случае компонент повторяется для каждого события, а объект передается в составе `MyEvent` `event` `dataContext` реквизита.

## <a name="see-also"></a>См. также

* [Начало работы с microsoft Graph набор средств React](./use-toolkit-with-react.md)
* [Узнайте о поставщиках проверки подлинности](../providers/providers.md)
