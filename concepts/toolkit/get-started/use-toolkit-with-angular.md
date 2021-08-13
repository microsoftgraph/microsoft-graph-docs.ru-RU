---
title: Использование Microsoft Graph Toolkit с Angular
description: Начало использования Microsoft Graph Toolkit в приложении Angular
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 8cd4c8039111dbc5f764cd4e698cf02c9aa0e1e621982e13947cb62846e1ea52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54159661"
---
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a>Использование Microsoft Graph Toolkit с Angular

Компоненты Microsoft Graph Toolkit хорошо взаимодействуют с такими веб-платформами, как Angular, в дополнение к обычным JavaScript и HTML. В этой статье описано использование Microsoft Graph Toolkit с Angular. Пошаговое руководство с описанием способа создания приложения Angular и использования Microsoft Graph Toolkit см. в статье [Использование Microsoft Graph Toolkit с Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).

## <a name="add-the-microsoft-graph-toolkit"></a>Добавление Microsoft Graph Toolkit

Сначала вам нужно включить настраиваемые элементы в приложении Angular, добавив `CUSTOM_ELEMENT_SCHEMA` к `@NgModule() decorator` в `app.module.ts`. В следующем примере показано, как это сделать.
```TypeScript
import { BrowserModule } from '@angular/platform-browser';
import { NgModule, CUSTOM_ELEMENTS_SCHEMA } from '@angular/core';

import { AppComponent } from './app.component';

@NgModule({
  declarations: [AppComponent],
  imports: [BrowserModule],
  schemas: [CUSTOM_ELEMENTS_SCHEMA],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule {}
```
Затем добавьте Microsoft Graph Toolkit в свой проект, установив пакет npm:
```Command Line
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a>Инициализация поставщика

Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md). Применяемый поставщик зависит от контекста, в котором будет использоваться ваше решение.

В следующем примере показано, как добавить [поставщика MSAL 2,](../providers/msal2.md)но вы можете следовать той же модели с любым из поставщиков.
>[!NOTE] 
>Если вы в настоящее время используете поставщика MSAL и хотите обновить поставщика MSAL 2, выполните действия в статье [поставщика MSAL 2.](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)

Импортируйте поставщика и настройте его для инициализации при запуске приложения. Замените `<YOUR-CLIENT-ID>` на идентификатор клиента для своего приложения.

```TypeScript
import { Component, OnInit } from '@angular/core';
import { Providers, Msal2Provider } from '@microsoft/mgt';

@Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css']
})
export class AppComponent implements OnInit {

    ngOnInit()
    {
        Providers.globalProvider = new Msal2Provider({
            clientId: '<YOUR-CLIENT-ID>'
        });
    }
}
```
### <a name="create-an-appclient-id"></a>Создание идентификатора клиента/приложения
Чтобы получить идентификатор клиента, вам нужно [зарегистрировать свое приложение](../../auth-register-app-v2.md) в Azure AD. 

## <a name="add-components"></a>Добавление компонентов

Теперь вы можете использовать любые компоненты Microsoft Graph Toolkit, как при обычной работе с HTML-шаблонами. Например, чтобы добавить компонент [Person](../components/person.md), добавьте в шаблон следующее:

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a>Настройка компонентов с использованием Angular

Все компоненты Microsoft Graph Toolkit поддерживают [настраиваемые шаблоны](../customize-components/templates.md), позволяющие изменять содержимое компонента. По умолчанию синтаксис для настройки компонентов предусматривает использование двойных фигурных скобок, чтобы ссылаться на данные свойств для каждого из возвращаемых элементов, как показано ниже.

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

Однако в Angular двойные фигурные скобки используются для привязки данных, и в компиляторе Angular возникнет ошибка, если вы попытаетесь использовать синтаксис с двойными фигурными скобками.

Вы можете избежать этих ошибок, изменив стандартные символы, применяемые в Toolkit, на символы, отличающиеся от двойных фигурных скобок, используя `TemplateHelper`. Лучше всего выполнять это в компоненте приложения верхнего уровня, чтобы применять это глобально.

Импортируйте `TemplateHelper` и используйте метод `.setBindingSyntax()`, чтобы настроить собственный синтаксис привязки.

```TypeScript
import { Component, OnInit } from '@angular/core';
import { Providers, Msal2Provider, TemplateHelper } from '@microsoft/mgt';

@Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css']
})
export class AppComponent implements OnInit {

    ngOnInit()
    {
        Providers.globalProvider = new Msal2Provider({ clientId: '<YOUR-CLIENT-ID>'})
        TemplateHelper.setBindingSyntax('[[',']]');
    }
}
```
Теперь вы можете использовать собственный синтаксис привязки для определения настраиваемых шаблонов.

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с пошаговыми инструкциями для [создания приложения Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).
- Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).
- Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).
- Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).
