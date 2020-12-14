---
title: Использование microsoft Graph набор средств Angular
description: Начало работы с microsoft Graph набор средств в приложении Angular.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: a1c0ebc252545491dc57d8910eb283db6d227ccd
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49664046"
---
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a>Использование microsoft Graph набор средств Angular

Компоненты набор средств Microsoft Graph отлично работают с веб-платформами, например Angular, в дополнение к javaScript и HTML. В этом разделе описывается, как использовать microsoft Graph набор средств Angular. Пошаговые пошаговые описания создания нового приложения Angular и использования microsoft Graph набор средств см. в статье [Набор средств Microsoft Graph с Angular.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)

## <a name="add-the-microsoft-graph-toolkit"></a>Добавление учетной записи Microsoft Graph набор средств

Сначала необходимо включить настраиваемые элементы в приложении Angular, добавив в `CUSTOM_ELEMENT_SCHEMA` `@NgModule() decorator` него элемент `app.module.ts` . В следующем примере показано, как это сделать:
```ts
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
Затем добавьте в проект набор средств Microsoft Graph, установив пакет npm с помощью:
```bash
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a>Инициализация поставщика

Поставщики набор средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Дополнительные см. [в этой теме.](../providers/providers.md) Используемый поставщик зависит от контекста, в котором будет использоваться ваше решение.

В следующем примере показано, как добавить [поставщика MSAL,](../providers/msal.md)но вы можете использовать ту же модель с любым из поставщиков. Импорт поставщика и его инициализация при инициализации приложения. Замените `<YOUR-CLIENT-ID>` его на ИД клиента для вашего приложения.

```ts
import { Component, OnInit } from '@angular/core';
import { Providers, MsalProvider } from '@microsoft/mgt';

@Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css']
})
export class AppComponent implements OnInit {

    ngOnInit()
    {
        Providers.globalProvider = new MsalProvider({
            clientId: '<YOUR-CLIENT-ID>'
        });
    }
}
```
### <a name="create-an-appclient-id"></a>Создание приложения или ИД клиента
Чтобы получить ИД клиента, необходимо зарегистрировать приложение [в](../../auth-register-app-v2.md) Azure AD. 
>**Примечание.** MSAL поддерживает только неявный поток для OAuth. Обязательно включите неявный поток в приложении на портале Azure (по умолчанию он не включен). В **разделе "Проверка подлинности"** найдите раздел неявного предоставления и выберите для маркеров **доступа** и **маркеров ID** свои почтовые ящики. 

## <a name="add-components"></a>Добавление компонентов

Теперь вы можете использовать любой из компонентов microsoft Graph набор средств, как обычно в htmL-шаблонах. Например, чтобы добавить компонент [Person,](../components/person.md)добавьте в шаблон следующее:

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a>Настройка компонентов с помощью Angular

Все набор средств Microsoft Graph [поддерживают](../customize-components/templates.md)настраиваемые шаблоны, которые позволяют изменять содержимое компонента. Синтаксис по умолчанию для настройки компонентов — использование двойных скобок для ссылки на данные свойств для каждого из возвращенных элементов, как показано ниже.

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

Однако в Angular для привязки данных используются двойные скобки, и компилятор Angular при попытке использовать синтаксис двойных скобок выдает ошибку.

Вы можете избежать этих ошибок, изменив используемые по умолчанию символы набор средств на что-то, кроме двойных скобок, с помощью `TemplateHelper` . Лучше всего это сделать в компоненте приложения верхнего уровня, чтобы оно применялось глобально.

Импортировать `TemplateHelper` и использовать метод для настройки `.setBindingSyntax()` пользовательского синтаксиса привязки.

```ts
import { Component, OnInit } from '@angular/core';
import { Providers, MsalProvider, TemplateHelper } from '@microsoft/mgt';

@Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css']
})
export class AppComponent implements OnInit {

    ngOnInit()
    {
        Providers.globalProvider = new MsalProvider({ clientId: '<YOUR-CLIENT-ID>'})
        TemplateHelper.setBindingSyntax('[[',']]');
    }
}
```
Теперь можно использовать пользовательский синтаксис привязки для определения настраиваемой шаблонов.

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с пошагами в этом пошаговом руководстве по [построению приложения Angular.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)
- Попробуйте компоненты в игровой [области.](https://mgt.dev)
- Задайте вопрос на [сайте Stack Overflow.](https://aka.ms/mgt-question)
- Сообщать об ошибках или оставлять запросы на функции на [GitHub.](https://aka.ms/mgt)