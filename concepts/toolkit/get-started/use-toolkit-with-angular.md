---
title: Использование Microsoft Graph Toolkit с Angular
description: Начало использования Microsoft Graph Toolkit в приложении Angular
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: b1985598985f85c0f33676fee49656324c65c7c5
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813189"
---
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a><span data-ttu-id="1a344-103">Использование Microsoft Graph Toolkit с Angular</span><span class="sxs-lookup"><span data-stu-id="1a344-103">Use the Microsoft Graph Toolkit with Angular</span></span>

<span data-ttu-id="1a344-104">Компоненты Microsoft Graph Toolkit хорошо взаимодействуют с такими веб-платформами, как Angular, в дополнение к обычным JavaScript и HTML.</span><span class="sxs-lookup"><span data-stu-id="1a344-104">Microsoft Graph Toolkit components work great with web frameworks like Angular in addition to vanilla JavaScript and HTML.</span></span> <span data-ttu-id="1a344-105">В этой статье описано использование Microsoft Graph Toolkit с Angular.</span><span class="sxs-lookup"><span data-stu-id="1a344-105">This topic describes how to use the Microsoft Graph Toolkit with Angular.</span></span> <span data-ttu-id="1a344-106">Пошаговое руководство с описанием способа создания приложения Angular и использования Microsoft Graph Toolkit см. в статье [Использование Microsoft Graph Toolkit с Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span><span class="sxs-lookup"><span data-stu-id="1a344-106">For a step-by-step walkthrough that describes how to create a new Angular application and use the Microsoft Graph Toolkit, see [Using Microsoft Graph Toolkit with Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="1a344-107">Добавление Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="1a344-107">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="1a344-108">Сначала вам нужно включить настраиваемые элементы в приложении Angular, добавив `CUSTOM_ELEMENT_SCHEMA` к `@NgModule() decorator` в `app.module.ts`.</span><span class="sxs-lookup"><span data-stu-id="1a344-108">First, you need to enable custom elements in your Angular application by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator` in `app.module.ts`.</span></span> <span data-ttu-id="1a344-109">В следующем примере показано, как это сделать.</span><span class="sxs-lookup"><span data-stu-id="1a344-109">The following example shows how to do this:</span></span>
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
<span data-ttu-id="1a344-110">Затем добавьте Microsoft Graph Toolkit в свой проект, установив пакет npm:</span><span class="sxs-lookup"><span data-stu-id="1a344-110">Next, add the Microsoft Graph Toolkit to your project by installing the npm package with:</span></span>
```Command Line
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a><span data-ttu-id="1a344-111">Инициализация поставщика</span><span class="sxs-lookup"><span data-stu-id="1a344-111">Initialize a provider</span></span>

<span data-ttu-id="1a344-112">Поставщики Microsoft Graph Toolkit обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="1a344-112">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="1a344-113">Дополнительные сведения см. в статье [Использование поставщиков](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="1a344-113">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="1a344-114">Применяемый поставщик зависит от контекста, в котором будет использоваться ваше решение.</span><span class="sxs-lookup"><span data-stu-id="1a344-114">The provider you use depends on the context in which your solution will be used.</span></span>

<span data-ttu-id="1a344-115">В следующем примере показано, как добавить [поставщика MSAL 2,](../providers/msal2.md)но вы можете следовать той же модели с любым из поставщиков.</span><span class="sxs-lookup"><span data-stu-id="1a344-115">The following example shows how to add the [MSAL 2 Provider](../providers/msal2.md), but you can follow the same model with any of the providers.</span></span>
>[!NOTE] 
><span data-ttu-id="1a344-116">Если вы в настоящее время используете поставщика MSAL и хотите обновить поставщика MSAL 2, выполните действия в статье [поставщика MSAL 2.](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)</span><span class="sxs-lookup"><span data-stu-id="1a344-116">If you are currently using the MSAL Provider and would like to update to the MSAL 2 Provider, follow the steps in the [MSAL 2 provider](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider) article.</span></span>

<span data-ttu-id="1a344-117">Импортируйте поставщика и настройте его для инициализации при запуске приложения.</span><span class="sxs-lookup"><span data-stu-id="1a344-117">Import the provider and set it to initialize when the application initializes.</span></span> <span data-ttu-id="1a344-118">Замените `<YOUR-CLIENT-ID>` на идентификатор клиента для своего приложения.</span><span class="sxs-lookup"><span data-stu-id="1a344-118">Replace `<YOUR-CLIENT-ID>` with the client ID for your application.</span></span>

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
### <a name="create-an-appclient-id"></a><span data-ttu-id="1a344-119">Создание идентификатора клиента/приложения</span><span class="sxs-lookup"><span data-stu-id="1a344-119">Create an app/client ID</span></span>
<span data-ttu-id="1a344-120">Чтобы получить идентификатор клиента, вам нужно [зарегистрировать свое приложение](../../auth-register-app-v2.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1a344-120">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> 

## <a name="add-components"></a><span data-ttu-id="1a344-121">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="1a344-121">Add components</span></span>

<span data-ttu-id="1a344-122">Теперь вы можете использовать любые компоненты Microsoft Graph Toolkit, как при обычной работе с HTML-шаблонами.</span><span class="sxs-lookup"><span data-stu-id="1a344-122">Now, you can use any of the Microsoft Graph Toolkit components as you normally would in your HTML templates.</span></span> <span data-ttu-id="1a344-123">Например, чтобы добавить компонент [Person](../components/person.md), добавьте в шаблон следующее:</span><span class="sxs-lookup"><span data-stu-id="1a344-123">For example, to add the [Person component](../components/person.md),  add the following to your template:</span></span>

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a><span data-ttu-id="1a344-124">Настройка компонентов с использованием Angular</span><span class="sxs-lookup"><span data-stu-id="1a344-124">Customizing components with Angular</span></span>

<span data-ttu-id="1a344-125">Все компоненты Microsoft Graph Toolkit поддерживают [настраиваемые шаблоны](../customize-components/templates.md), позволяющие изменять содержимое компонента.</span><span class="sxs-lookup"><span data-stu-id="1a344-125">All Microsoft Graph Toolkit components support [custom templates](../customize-components/templates.md), which allow you to modify the content of a component.</span></span> <span data-ttu-id="1a344-126">По умолчанию синтаксис для настройки компонентов предусматривает использование двойных фигурных скобок, чтобы ссылаться на данные свойств для каждого из возвращаемых элементов, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="1a344-126">The default syntax for customizing the components is to use double braces to refer to the property data for each of the returned items, as shown:</span></span>

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

<span data-ttu-id="1a344-127">Однако в Angular двойные фигурные скобки используются для привязки данных, и в компиляторе Angular возникнет ошибка, если вы попытаетесь использовать синтаксис с двойными фигурными скобками.</span><span class="sxs-lookup"><span data-stu-id="1a344-127">In Angular, however, double braces are used for data binding and the Angular compiler will throw an error if you try to use the double brace syntax.</span></span>

<span data-ttu-id="1a344-128">Вы можете избежать этих ошибок, изменив стандартные символы, применяемые в Toolkit, на символы, отличающиеся от двойных фигурных скобок, используя `TemplateHelper`.</span><span class="sxs-lookup"><span data-stu-id="1a344-128">You can avoid these errors by changing the default characters used by the Toolkit to something other than double braces by using the `TemplateHelper`.</span></span> <span data-ttu-id="1a344-129">Лучше всего выполнять это в компоненте приложения верхнего уровня, чтобы применять это глобально.</span><span class="sxs-lookup"><span data-stu-id="1a344-129">It is best to do this in your top-level App component so that it applies globally.</span></span>

<span data-ttu-id="1a344-130">Импортируйте `TemplateHelper` и используйте метод `.setBindingSyntax()`, чтобы настроить собственный синтаксис привязки.</span><span class="sxs-lookup"><span data-stu-id="1a344-130">Import the `TemplateHelper` and use the `.setBindingSyntax()` method to set your custom binding syntax.</span></span>

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
<span data-ttu-id="1a344-131">Теперь вы можете использовать собственный синтаксис привязки для определения настраиваемых шаблонов.</span><span class="sxs-lookup"><span data-stu-id="1a344-131">Now, you can use your custom binding syntax to define custom templates.</span></span>

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a><span data-ttu-id="1a344-132">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1a344-132">Next steps</span></span>
- <span data-ttu-id="1a344-133">Ознакомьтесь с пошаговыми инструкциями для [создания приложения Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span><span class="sxs-lookup"><span data-stu-id="1a344-133">Check out this step-by-step tutorial on [building an Angular app](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>
- <span data-ttu-id="1a344-134">Воспользуйтесь компонентами в [интерактивной среде](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="1a344-134">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="1a344-135">Задавайте вопросы на сайте [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="1a344-135">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="1a344-136">Сообщайте об ошибках и оставляйте запросы на создание функций в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="1a344-136">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
