---
title: Использование набора средств Microsoft Graph с угловой страницей
description: Приступите к работе с набором инструментов Microsoft Graph в приложении в угловом приложении.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: be84107314a9696486b377f09dc399d6e15c44cf
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288506"
---
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a>Использование набора средств Microsoft Graph с угловой страницей

Компоненты набора инструментов Microsoft Graph отлично работают с веб-платформами, такими как радиальные, в дополнение к Ванилла JavaScript и HTML. В этом разделе описывается, как использовать набор средств Microsoft Graph с помощью раздела "Радиальный". Пошаговое руководство, в котором описывается создание нового приложения и использование набора инструментов Microsoft Graph, представлено в разделе [Использование набора средств Microsoft Graph с](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)помощью пункта "Радиальный".

## <a name="add-the-microsoft-graph-toolkit"></a>Добавление набора средств Microsoft Graph

Для начала необходимо включить настраиваемые элементы в угловом приложении, добавив элемент `CUSTOM_ELEMENT_SCHEMA` `@NgModule() decorator` in `app.module.ts` . В приведенном ниже примере показано, как это сделать.
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
Затем добавьте в свой проект набор инструментов Microsoft Graph, установив пакет NPM с:
```bash
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a>Инициализация поставщика

Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов. Чтобы узнать больше, ознакомьтесь со статьей [Использование поставщиков](../providers.md). Используемый поставщик зависит от контекста, в котором будет использоваться решение.

В приведенном ниже примере показано, как добавить [поставщик MSAL](../providers/msal.md), но вы можете использовать ту же модель со всеми поставщиками. Импортируйте поставщик и присвойте ему значение Initialize при инициализации приложения. Замените `<YOUR-CLIENT-ID>` идентификатором клиента для вашего приложения.

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
### <a name="create-an-appclient-id"></a>Создание идентификатора приложения или клиента
Чтобы получить идентификатор клиента, необходимо [зарегистрировать приложение](../../auth-register-app-v2.md) в Azure AD. 
>**Note**: MSAL поддерживает только неявный поток для OAuth. Не забудьте включить неявный поток в приложении на портале Azure (по умолчанию он не включен). В разделе **Проверка подлинности**найдите раздел **неявный предоставление** и установите флажки для **маркеров доступа** и **маркеров ID**.

## <a name="add-components"></a>Добавление компонентов

Теперь вы можете использовать любые компоненты набора инструментов Microsoft Graph, как и в случае шаблонов HTML. Например, чтобы добавить [компонент Person](../components/person.md), добавьте в шаблон следующий код:

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a>Настройка компонентов с помощью угловой

Все компоненты набора инструментов Microsoft Graph поддерживают [Настраиваемые шаблоны](../templates.md), которые позволяют изменять содержимое компонента. По умолчанию для настройки компонентов используются двойные фигурные скобки, указывающие на данные свойства для каждого возвращенного элемента, как показано ниже:

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

Однако в угловых скобках для привязки данных используются двойные скобки, а при попытке использовать синтаксис двойной скобки будет выдаваться сообщение об ошибке.

Эти ошибки можно избежать, изменив символы по умолчанию, используемые в наборе инструментов, на другие, кроме двойных фигурных скобок, с помощью параметра `TemplateHelper` . Это лучше всего сделать в компоненте приложения верхнего уровня, чтобы он применялся глобально.

Импортируйте `TemplateHelper` метод и используйте его `.setBindingSyntax()` для установки пользовательского синтаксиса привязки.

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
Теперь можно использовать пользовательский синтаксис привязки для определения пользовательских шаблонов.

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с пошаговыми руководствами по [созданию углового приложения](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).
- Опробуйте компоненты в [интерактивная среда](https://mgt.dev).
- Задайте вопрос о [переполнении стека](https://aka.ms/mgt-question).
- Сообщать об ошибках или оставлять запрос на функцию в [GitHub](https://aka.ms/mgt).