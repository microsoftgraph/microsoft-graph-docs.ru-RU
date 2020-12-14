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
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a><span data-ttu-id="b3cca-103">Использование microsoft Graph набор средств Angular</span><span class="sxs-lookup"><span data-stu-id="b3cca-103">Use the Microsoft Graph Toolkit with Angular</span></span>

<span data-ttu-id="b3cca-104">Компоненты набор средств Microsoft Graph отлично работают с веб-платформами, например Angular, в дополнение к javaScript и HTML.</span><span class="sxs-lookup"><span data-stu-id="b3cca-104">Microsoft Graph Toolkit components work great with web frameworks like Angular in addition to vanilla JavaScript and HTML.</span></span> <span data-ttu-id="b3cca-105">В этом разделе описывается, как использовать microsoft Graph набор средств Angular.</span><span class="sxs-lookup"><span data-stu-id="b3cca-105">This topic describes how to use the Microsoft Graph Toolkit with Angular.</span></span> <span data-ttu-id="b3cca-106">Пошаговые пошаговые описания создания нового приложения Angular и использования microsoft Graph набор средств см. в статье [Набор средств Microsoft Graph с Angular.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)</span><span class="sxs-lookup"><span data-stu-id="b3cca-106">For a step-by-step walkthrough that describes how to create a new Angular application and use the Microsoft Graph Toolkit, see [Using Microsoft Graph Toolkit with Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="b3cca-107">Добавление учетной записи Microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="b3cca-107">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="b3cca-108">Сначала необходимо включить настраиваемые элементы в приложении Angular, добавив в `CUSTOM_ELEMENT_SCHEMA` `@NgModule() decorator` него элемент `app.module.ts` .</span><span class="sxs-lookup"><span data-stu-id="b3cca-108">First, you need to enable custom elements in your Angular application by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator` in `app.module.ts`.</span></span> <span data-ttu-id="b3cca-109">В следующем примере показано, как это сделать:</span><span class="sxs-lookup"><span data-stu-id="b3cca-109">The following example shows how to do this:</span></span>
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
<span data-ttu-id="b3cca-110">Затем добавьте в проект набор средств Microsoft Graph, установив пакет npm с помощью:</span><span class="sxs-lookup"><span data-stu-id="b3cca-110">Next, add the Microsoft Graph Toolkit to your project by installing the npm package with:</span></span>
```bash
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a><span data-ttu-id="b3cca-111">Инициализация поставщика</span><span class="sxs-lookup"><span data-stu-id="b3cca-111">Initialize a provider</span></span>

<span data-ttu-id="b3cca-112">Поставщики набор средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="b3cca-112">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="b3cca-113">Дополнительные см. [в этой теме.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="b3cca-113">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="b3cca-114">Используемый поставщик зависит от контекста, в котором будет использоваться ваше решение.</span><span class="sxs-lookup"><span data-stu-id="b3cca-114">The provider you use depends on the context in which your solution will be used.</span></span>

<span data-ttu-id="b3cca-115">В следующем примере показано, как добавить [поставщика MSAL,](../providers/msal.md)но вы можете использовать ту же модель с любым из поставщиков.</span><span class="sxs-lookup"><span data-stu-id="b3cca-115">The following example shows how to add the [MSAL Provider](../providers/msal.md), but you can follow the same model with any of the providers.</span></span> <span data-ttu-id="b3cca-116">Импорт поставщика и его инициализация при инициализации приложения.</span><span class="sxs-lookup"><span data-stu-id="b3cca-116">Import the provider and set it to initialize when the application initializes.</span></span> <span data-ttu-id="b3cca-117">Замените `<YOUR-CLIENT-ID>` его на ИД клиента для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="b3cca-117">Replace `<YOUR-CLIENT-ID>` with the client ID for your application.</span></span>

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
### <a name="create-an-appclient-id"></a><span data-ttu-id="b3cca-118">Создание приложения или ИД клиента</span><span class="sxs-lookup"><span data-stu-id="b3cca-118">Create an app/client ID</span></span>
<span data-ttu-id="b3cca-119">Чтобы получить ИД клиента, необходимо зарегистрировать приложение [в](../../auth-register-app-v2.md) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b3cca-119">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> 
><span data-ttu-id="b3cca-120">**Примечание.** MSAL поддерживает только неявный поток для OAuth.</span><span class="sxs-lookup"><span data-stu-id="b3cca-120">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="b3cca-121">Обязательно включите неявный поток в приложении на портале Azure (по умолчанию он не включен).</span><span class="sxs-lookup"><span data-stu-id="b3cca-121">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="b3cca-122">В **разделе "Проверка подлинности"** найдите раздел неявного предоставления и выберите для маркеров **доступа** и **маркеров ID** свои почтовые ящики. </span><span class="sxs-lookup"><span data-stu-id="b3cca-122">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span>

## <a name="add-components"></a><span data-ttu-id="b3cca-123">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="b3cca-123">Add components</span></span>

<span data-ttu-id="b3cca-124">Теперь вы можете использовать любой из компонентов microsoft Graph набор средств, как обычно в htmL-шаблонах.</span><span class="sxs-lookup"><span data-stu-id="b3cca-124">Now, you can use any of the Microsoft Graph Toolkit components as you normally would in your HTML templates.</span></span> <span data-ttu-id="b3cca-125">Например, чтобы добавить компонент [Person,](../components/person.md)добавьте в шаблон следующее:</span><span class="sxs-lookup"><span data-stu-id="b3cca-125">For example, to add the [Person component](../components/person.md),  add the following to your template:</span></span>

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a><span data-ttu-id="b3cca-126">Настройка компонентов с помощью Angular</span><span class="sxs-lookup"><span data-stu-id="b3cca-126">Customizing components with Angular</span></span>

<span data-ttu-id="b3cca-127">Все набор средств Microsoft Graph [поддерживают](../customize-components/templates.md)настраиваемые шаблоны, которые позволяют изменять содержимое компонента.</span><span class="sxs-lookup"><span data-stu-id="b3cca-127">All Microsoft Graph Toolkit components support [custom templates](../customize-components/templates.md), which allow you to modify the content of a component.</span></span> <span data-ttu-id="b3cca-128">Синтаксис по умолчанию для настройки компонентов — использование двойных скобок для ссылки на данные свойств для каждого из возвращенных элементов, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="b3cca-128">The default syntax for customizing the components is to use double braces to refer to the property data for each of the returned items, as shown:</span></span>

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

<span data-ttu-id="b3cca-129">Однако в Angular для привязки данных используются двойные скобки, и компилятор Angular при попытке использовать синтаксис двойных скобок выдает ошибку.</span><span class="sxs-lookup"><span data-stu-id="b3cca-129">In Angular, however, double braces are used for data binding and the Angular compiler will throw an error if you try to use the double brace syntax.</span></span>

<span data-ttu-id="b3cca-130">Вы можете избежать этих ошибок, изменив используемые по умолчанию символы набор средств на что-то, кроме двойных скобок, с помощью `TemplateHelper` .</span><span class="sxs-lookup"><span data-stu-id="b3cca-130">You can avoid these errors by changing the default characters used by the Toolkit to something other than double braces by using the `TemplateHelper`.</span></span> <span data-ttu-id="b3cca-131">Лучше всего это сделать в компоненте приложения верхнего уровня, чтобы оно применялось глобально.</span><span class="sxs-lookup"><span data-stu-id="b3cca-131">It is best to do this in your top-level App component so that it applies globally.</span></span>

<span data-ttu-id="b3cca-132">Импортировать `TemplateHelper` и использовать метод для настройки `.setBindingSyntax()` пользовательского синтаксиса привязки.</span><span class="sxs-lookup"><span data-stu-id="b3cca-132">Import the `TemplateHelper` and use the `.setBindingSyntax()` method to set your custom binding syntax.</span></span>

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
<span data-ttu-id="b3cca-133">Теперь можно использовать пользовательский синтаксис привязки для определения настраиваемой шаблонов.</span><span class="sxs-lookup"><span data-stu-id="b3cca-133">Now, you can use your custom binding syntax to define custom templates.</span></span>

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a><span data-ttu-id="b3cca-134">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b3cca-134">Next steps</span></span>
- <span data-ttu-id="b3cca-135">Ознакомьтесь с пошагами в этом пошаговом руководстве по [построению приложения Angular.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)</span><span class="sxs-lookup"><span data-stu-id="b3cca-135">Check out this step-by-step tutorial on [building an Angular app](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>
- <span data-ttu-id="b3cca-136">Попробуйте компоненты в игровой [области.](https://mgt.dev)</span><span class="sxs-lookup"><span data-stu-id="b3cca-136">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="b3cca-137">Задайте вопрос на [сайте Stack Overflow.](https://aka.ms/mgt-question)</span><span class="sxs-lookup"><span data-stu-id="b3cca-137">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="b3cca-138">Сообщать об ошибках или оставлять запросы на функции на [GitHub.](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="b3cca-138">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>