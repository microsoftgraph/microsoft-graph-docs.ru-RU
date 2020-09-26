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
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a><span data-ttu-id="b3464-103">Использование набора средств Microsoft Graph с угловой страницей</span><span class="sxs-lookup"><span data-stu-id="b3464-103">Use the Microsoft Graph Toolkit with Angular</span></span>

<span data-ttu-id="b3464-104">Компоненты набора инструментов Microsoft Graph отлично работают с веб-платформами, такими как радиальные, в дополнение к Ванилла JavaScript и HTML.</span><span class="sxs-lookup"><span data-stu-id="b3464-104">Microsoft Graph Toolkit components work great with web frameworks like Angular in addition to vanilla JavaScript and HTML.</span></span> <span data-ttu-id="b3464-105">В этом разделе описывается, как использовать набор средств Microsoft Graph с помощью раздела "Радиальный".</span><span class="sxs-lookup"><span data-stu-id="b3464-105">This topic describes how to use the Microsoft Graph Toolkit with Angular.</span></span> <span data-ttu-id="b3464-106">Пошаговое руководство, в котором описывается создание нового приложения и использование набора инструментов Microsoft Graph, представлено в разделе [Использование набора средств Microsoft Graph с](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)помощью пункта "Радиальный".</span><span class="sxs-lookup"><span data-stu-id="b3464-106">For a step-by-step walkthrough that describes how to create a new Angular application and use the Microsoft Graph Toolkit, see [Using Microsoft Graph Toolkit with Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="b3464-107">Добавление набора средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b3464-107">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="b3464-108">Для начала необходимо включить настраиваемые элементы в угловом приложении, добавив элемент `CUSTOM_ELEMENT_SCHEMA` `@NgModule() decorator` in `app.module.ts` .</span><span class="sxs-lookup"><span data-stu-id="b3464-108">First, you need to enable custom elements in your Angular application by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator` in `app.module.ts`.</span></span> <span data-ttu-id="b3464-109">В приведенном ниже примере показано, как это сделать.</span><span class="sxs-lookup"><span data-stu-id="b3464-109">The following example shows how to do this:</span></span>
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
<span data-ttu-id="b3464-110">Затем добавьте в свой проект набор инструментов Microsoft Graph, установив пакет NPM с:</span><span class="sxs-lookup"><span data-stu-id="b3464-110">Next, add the Microsoft Graph Toolkit to your project by installing the npm package with:</span></span>
```bash
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a><span data-ttu-id="b3464-111">Инициализация поставщика</span><span class="sxs-lookup"><span data-stu-id="b3464-111">Initialize a provider</span></span>

<span data-ttu-id="b3464-112">Поставщики набора средств Microsoft Graph обеспечивают проверку подлинности и доступ к Microsoft Graph для компонентов.</span><span class="sxs-lookup"><span data-stu-id="b3464-112">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="b3464-113">Чтобы узнать больше, ознакомьтесь со статьей [Использование поставщиков](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="b3464-113">To learn more, see [Using the providers](../providers.md).</span></span> <span data-ttu-id="b3464-114">Используемый поставщик зависит от контекста, в котором будет использоваться решение.</span><span class="sxs-lookup"><span data-stu-id="b3464-114">The provider you use depends on the context in which your solution will be used.</span></span>

<span data-ttu-id="b3464-115">В приведенном ниже примере показано, как добавить [поставщик MSAL](../providers/msal.md), но вы можете использовать ту же модель со всеми поставщиками.</span><span class="sxs-lookup"><span data-stu-id="b3464-115">The following example shows how to add the [MSAL Provider](../providers/msal.md), but you can follow the same model with any of the providers.</span></span> <span data-ttu-id="b3464-116">Импортируйте поставщик и присвойте ему значение Initialize при инициализации приложения.</span><span class="sxs-lookup"><span data-stu-id="b3464-116">Import the provider and set it to initialize when the application initializes.</span></span> <span data-ttu-id="b3464-117">Замените `<YOUR-CLIENT-ID>` идентификатором клиента для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="b3464-117">Replace `<YOUR-CLIENT-ID>` with the client ID for your application.</span></span>

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
### <a name="create-an-appclient-id"></a><span data-ttu-id="b3464-118">Создание идентификатора приложения или клиента</span><span class="sxs-lookup"><span data-stu-id="b3464-118">Create an app/client ID</span></span>
<span data-ttu-id="b3464-119">Чтобы получить идентификатор клиента, необходимо [зарегистрировать приложение](../../auth-register-app-v2.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b3464-119">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> 
><span data-ttu-id="b3464-120">**Note**: MSAL поддерживает только неявный поток для OAuth.</span><span class="sxs-lookup"><span data-stu-id="b3464-120">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="b3464-121">Не забудьте включить неявный поток в приложении на портале Azure (по умолчанию он не включен).</span><span class="sxs-lookup"><span data-stu-id="b3464-121">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="b3464-122">В разделе **Проверка подлинности**найдите раздел **неявный предоставление** и установите флажки для **маркеров доступа** и **маркеров ID**.</span><span class="sxs-lookup"><span data-stu-id="b3464-122">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span>

## <a name="add-components"></a><span data-ttu-id="b3464-123">Добавление компонентов</span><span class="sxs-lookup"><span data-stu-id="b3464-123">Add components</span></span>

<span data-ttu-id="b3464-124">Теперь вы можете использовать любые компоненты набора инструментов Microsoft Graph, как и в случае шаблонов HTML.</span><span class="sxs-lookup"><span data-stu-id="b3464-124">Now, you can use any of the Microsoft Graph Toolkit components as you normally would in your HTML templates.</span></span> <span data-ttu-id="b3464-125">Например, чтобы добавить [компонент Person](../components/person.md), добавьте в шаблон следующий код:</span><span class="sxs-lookup"><span data-stu-id="b3464-125">For example, to add the [Person component](../components/person.md),  add the following to your template:</span></span>

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a><span data-ttu-id="b3464-126">Настройка компонентов с помощью угловой</span><span class="sxs-lookup"><span data-stu-id="b3464-126">Customizing components with Angular</span></span>

<span data-ttu-id="b3464-127">Все компоненты набора инструментов Microsoft Graph поддерживают [Настраиваемые шаблоны](../templates.md), которые позволяют изменять содержимое компонента.</span><span class="sxs-lookup"><span data-stu-id="b3464-127">All Microsoft Graph Toolkit components support [custom templates](../templates.md), which allow you to modify the content of a component.</span></span> <span data-ttu-id="b3464-128">По умолчанию для настройки компонентов используются двойные фигурные скобки, указывающие на данные свойства для каждого возвращенного элемента, как показано ниже:</span><span class="sxs-lookup"><span data-stu-id="b3464-128">The default syntax for customizing the components is to use double braces to refer to the property data for each of the returned items, as shown:</span></span>

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

<span data-ttu-id="b3464-129">Однако в угловых скобках для привязки данных используются двойные скобки, а при попытке использовать синтаксис двойной скобки будет выдаваться сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="b3464-129">In Angular, however, double braces are used for data binding and the Angular compiler will throw an error if you try to use the double brace syntax.</span></span>

<span data-ttu-id="b3464-130">Эти ошибки можно избежать, изменив символы по умолчанию, используемые в наборе инструментов, на другие, кроме двойных фигурных скобок, с помощью параметра `TemplateHelper` .</span><span class="sxs-lookup"><span data-stu-id="b3464-130">You can avoid these errors by changing the default characters used by the Toolkit to something other than double braces by using the `TemplateHelper`.</span></span> <span data-ttu-id="b3464-131">Это лучше всего сделать в компоненте приложения верхнего уровня, чтобы он применялся глобально.</span><span class="sxs-lookup"><span data-stu-id="b3464-131">It is best to do this in your top-level App component so that it applies globally.</span></span>

<span data-ttu-id="b3464-132">Импортируйте `TemplateHelper` метод и используйте его `.setBindingSyntax()` для установки пользовательского синтаксиса привязки.</span><span class="sxs-lookup"><span data-stu-id="b3464-132">Import the `TemplateHelper` and use the `.setBindingSyntax()` method to set your custom binding syntax.</span></span>

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
<span data-ttu-id="b3464-133">Теперь можно использовать пользовательский синтаксис привязки для определения пользовательских шаблонов.</span><span class="sxs-lookup"><span data-stu-id="b3464-133">Now, you can use your custom binding syntax to define custom templates.</span></span>

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a><span data-ttu-id="b3464-134">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b3464-134">Next steps</span></span>
- <span data-ttu-id="b3464-135">Ознакомьтесь с пошаговыми руководствами по [созданию углового приложения](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span><span class="sxs-lookup"><span data-stu-id="b3464-135">Check out this step-by-step tutorial on [building an Angular app](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>
- <span data-ttu-id="b3464-136">Опробуйте компоненты в [интерактивная среда](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="b3464-136">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="b3464-137">Задайте вопрос о [переполнении стека](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="b3464-137">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="b3464-138">Сообщать об ошибках или оставлять запрос на функцию в [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="b3464-138">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>