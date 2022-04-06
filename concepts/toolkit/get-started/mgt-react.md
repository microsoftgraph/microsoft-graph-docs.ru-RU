---
title: Компоненты Microsoft Graph Toolkit в React
description: Компоненты Microsoft Graph Toolkit в React (`mgt-react`) позволяют разработчикам React использовать Microsoft Graph Toolkit в приложениях React.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 4dff722faf3f61b4ed9832c2389b674d9bf1a444
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589004"
---
# <a name="microsoft-graph-toolkit-react-components"></a>Компоненты Microsoft Graph Toolkit в React

Компоненты Microsoft Graph Toolkit в React (`mgt-react`) позволяют разработчикам React использовать Microsoft Graph Toolkit в приложениях React. Библиотека упаковывает все компоненты Microsoft Graph Toolkit и экспортирует их как компоненты React.

## <a name="what-components-can-i-use"></a>Какие компоненты можно использовать?

Библиотека создается автоматически из веб-компонентов Microsoft Graph Toolkit, и все ее компоненты доступны как компоненты React.

Имена компонентов React приводятся в PascalCase и не включают префикс `Mgt`. Например, компонент `mgt-person` доступен как `Person`, а `mgt-people-picker` — как `PeoplePicker`.

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

Все компоненты доступны через пакет NPM и названы с использованием PascalCase. Чтобы использовать компонент, сначала импортируйте его вверх.

```tsx
import { Person } from '@microsoft/mgt-react';
```

Теперь вы можете использовать `Person` где угодно в JSX как регулярный компонент React.

```tsx
<Person personQuery="me" />
```

Все свойства и события точно соответствуют своему определению в документации по компонентам.

Например, вы можете настроить свойство `personDetails` для объекта:

```jsx
const App = (props) => {
  const personDetails = {
    displayName: 'Bill Gates',
  };

  return <Person personDetails={personDetails}></Person>;
};
```

Вы также можете зарегистрировать обработчик событий:

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

Большинство компонентов Microsoft Graph Toolkit [поддерживают шаблоны](../customize-components/templates.md), а `mgt-react` позволяет использовать React для создания шаблонов.

Например, чтобы создать шаблон для представления событий в компоненте `mgt-agenda`, сначала определите компонент, который следует использовать для представления события:

```tsx
import { MgtTemplateProps } from '@microsoft/mgt-react';

const MyEvent = (props: MgtTemplateProps) => {
  const { event } = props.dataContext;
  return <div>
    {event.subject}<br />
    {event.attendees
      .map((attendee: any) => attendee.emailAddress.name)
      .join(', ')}
  </div>;
};
```

Затем используйте его как дочерний элемент упакованного компонента и задайте для свойства template значение `event`.

```tsx
import { Agenda } from '@microsoft/mgt-react';

const App = (props) => {
  return <Agenda>
    <MyEvent template="event">
  </Agenda>
}
```

Свойство `template` позволяет указать, какой шаблон следует перезаписать. В этом случае компонент `MyEvent` будет повторяться для каждого события, а объект `event` будет передаваться в составе свойства `dataContext`.

## <a name="see-also"></a>См. также

* [Начало работы с Microsoft Graph Toolkit в React](./use-toolkit-with-react.md)
* [Сведения о поставщиках проверки подлинности](../providers/providers.md)
