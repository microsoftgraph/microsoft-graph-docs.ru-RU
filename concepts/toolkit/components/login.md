---
title: Компонент входа в Microsoft Graph Toolkit
description: Компонент входа — это кнопка и всплывающий элемент управления, предназначенные для упрощения проверки подлинности платформы удостоверений Майкрософт.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 5dd610407fde25089a9c323b6b0cfb7965d33671
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334768"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="8dd6c-103">Компонент входа в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="8dd6c-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8dd6c-104">Компонент входа — это кнопка и всплывающий элемент управления, предназначенные для упрощения проверки подлинности платформы удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="8dd6c-105">Он обеспечивает два состояния:</span><span class="sxs-lookup"><span data-stu-id="8dd6c-105">It provides two states:</span></span>
* <span data-ttu-id="8dd6c-106">Если пользователь не вошел в систему, элемент управления является простой кнопкой для запуска входа в систему.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="8dd6c-107">Если пользователь вошел в систему, элемент управления отображает имя, изображение профиля и электронную почту вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="8dd6c-108">При щелчке открывается всплывающее окно с командой для выхода.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="8dd6c-109">Пример</span><span class="sxs-lookup"><span data-stu-id="8dd6c-109">Example</span></span>

<span data-ttu-id="8dd6c-110">В примере ниже показан компонент `mgt-login` с указанием вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="8dd6c-111">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="8dd6c-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="8dd6c-112">Использование элемента управления без поставщика проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="8dd6c-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="8dd6c-113">По умолчанию компонент поддерживает поставщика и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="8dd6c-114">Но если вы хотите указать свою логику и проверку подлинности, вы можете воспользоваться свойством `userDetails`, чтобы настроить сведения о вошедшем пользователе.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="8dd6c-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="8dd6c-115">Attribute</span></span> | <span data-ttu-id="8dd6c-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dd6c-116">Property</span></span> | <span data-ttu-id="8dd6c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="8dd6c-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="8dd6c-118">user-details</span><span class="sxs-lookup"><span data-stu-id="8dd6c-118">user-details</span></span> | <span data-ttu-id="8dd6c-119">userDetails</span><span class="sxs-lookup"><span data-stu-id="8dd6c-119">userDetails</span></span> | <span data-ttu-id="8dd6c-120">Настройка объекта пользователя, который будет отображаться в элементе управления.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="8dd6c-121">В примере ниже настраиваются сведения о пользователе.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="8dd6c-122">Присвоение параметру `userDetails` значения `null` обеспечивает переход к состоянию выхода.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="8dd6c-123">Чтобы обрабатывать вход и выход, используйте события `loginInitiated` и `logoutInitiated`.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="8dd6c-124">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="8dd6c-124">CSS custom properties</span></span>

<span data-ttu-id="8dd6c-125">Компонент `mgt-login` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

```css
mgt-login {
  --font-size: 14px;
  --font-weight: 600;
  --weith: '100%';
  --height: '100%';
  --margin: 0;
  --padding: 12px 20px;
  --button-color: #201f1e;
  --button-color--hover: var(--theme-primary-color);
  --button-background-color: transparent;
  --button-background-color--hover: #edebe9;
  --popup-background-color: white;
  --popup-command-font-size: 12px;
  --popup-color: #201f1e;
}
```

<span data-ttu-id="8dd6c-126">Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="8dd6c-126">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="8dd6c-127">События</span><span class="sxs-lookup"><span data-stu-id="8dd6c-127">Events</span></span>

<span data-ttu-id="8dd6c-128">Из элемента управления инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-128">The following events are fired from the control.</span></span>

<span data-ttu-id="8dd6c-129">Событие</span><span class="sxs-lookup"><span data-stu-id="8dd6c-129">Event</span></span> | <span data-ttu-id="8dd6c-130">Когда он излучается</span><span class="sxs-lookup"><span data-stu-id="8dd6c-130">When is it emitted</span></span> | <span data-ttu-id="8dd6c-131">Настраиваемые данные</span><span class="sxs-lookup"><span data-stu-id="8dd6c-131">Custom data</span></span> | <span data-ttu-id="8dd6c-132">Отмена</span><span class="sxs-lookup"><span data-stu-id="8dd6c-132">Cancelable</span></span> | <span data-ttu-id="8dd6c-133">Пузыри</span><span class="sxs-lookup"><span data-stu-id="8dd6c-133">Bubbles</span></span> | <span data-ttu-id="8dd6c-134">Работает с настраиваемой шаблонной</span><span class="sxs-lookup"><span data-stu-id="8dd6c-134">Works with custom template</span></span>
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`loginInitiated` | <span data-ttu-id="8dd6c-135">Чтобы запустить процесс входа, пользователь нажал кнопку вход в систему.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-135">The user clicked the sign in button to start the login process</span></span> | <span data-ttu-id="8dd6c-136">Нет</span><span class="sxs-lookup"><span data-stu-id="8dd6c-136">None</span></span> | <span data-ttu-id="8dd6c-137">Да</span><span class="sxs-lookup"><span data-stu-id="8dd6c-137">Yes</span></span> | <span data-ttu-id="8dd6c-138">Нет</span><span class="sxs-lookup"><span data-stu-id="8dd6c-138">No</span></span> | <span data-ttu-id="8dd6c-139">Да</span><span class="sxs-lookup"><span data-stu-id="8dd6c-139">Yes</span></span>
`loginCompleted` | <span data-ttu-id="8dd6c-140">Процесс входа был успешным, и теперь пользователь входит в</span><span class="sxs-lookup"><span data-stu-id="8dd6c-140">The login process was successful and the user is now signed in</span></span> | <span data-ttu-id="8dd6c-141">Нет.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-141">None</span></span> | <span data-ttu-id="8dd6c-142">Нет</span><span class="sxs-lookup"><span data-stu-id="8dd6c-142">No</span></span> | <span data-ttu-id="8dd6c-143">Нет</span><span class="sxs-lookup"><span data-stu-id="8dd6c-143">No</span></span> | <span data-ttu-id="8dd6c-144">Да</span><span class="sxs-lookup"><span data-stu-id="8dd6c-144">Yes</span></span>
`loginFailed` | <span data-ttu-id="8dd6c-145">Пользователь отменил процесс входа или не смог войти</span><span class="sxs-lookup"><span data-stu-id="8dd6c-145">The user canceled the login process or was unable to sign in</span></span> | <span data-ttu-id="8dd6c-146">Нет.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-146">None</span></span> | <span data-ttu-id="8dd6c-147">Нет</span><span class="sxs-lookup"><span data-stu-id="8dd6c-147">No</span></span> | <span data-ttu-id="8dd6c-148">Нет</span><span class="sxs-lookup"><span data-stu-id="8dd6c-148">No</span></span> | <span data-ttu-id="8dd6c-149">Да</span><span class="sxs-lookup"><span data-stu-id="8dd6c-149">Yes</span></span>
`logoutInitiated` | <span data-ttu-id="8dd6c-150">Пользователь начал выходить на сайт</span><span class="sxs-lookup"><span data-stu-id="8dd6c-150">The user started to logout</span></span> | <span data-ttu-id="8dd6c-151">Нет</span><span class="sxs-lookup"><span data-stu-id="8dd6c-151">None</span></span> | <span data-ttu-id="8dd6c-152">Да</span><span class="sxs-lookup"><span data-stu-id="8dd6c-152">Yes</span></span> | <span data-ttu-id="8dd6c-153">Нет</span><span class="sxs-lookup"><span data-stu-id="8dd6c-153">No</span></span> | <span data-ttu-id="8dd6c-154">Да</span><span class="sxs-lookup"><span data-stu-id="8dd6c-154">Yes</span></span>
`logoutCompleted` | <span data-ttu-id="8dd6c-155">Пользователь вышел из</span><span class="sxs-lookup"><span data-stu-id="8dd6c-155">The user signed out</span></span> | <span data-ttu-id="8dd6c-156">Нет.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-156">None</span></span> | <span data-ttu-id="8dd6c-157">Нет</span><span class="sxs-lookup"><span data-stu-id="8dd6c-157">No</span></span> | <span data-ttu-id="8dd6c-158">Нет</span><span class="sxs-lookup"><span data-stu-id="8dd6c-158">No</span></span> | <span data-ttu-id="8dd6c-159">Да</span><span class="sxs-lookup"><span data-stu-id="8dd6c-159">Yes</span></span>

<span data-ttu-id="8dd6c-160">Дополнительные сведения об обработке событий см. в [этой работе.](../customize-components/events.md)</span><span class="sxs-lookup"><span data-stu-id="8dd6c-160">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="8dd6c-161">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="8dd6c-161">Templates</span></span>

<span data-ttu-id="8dd6c-162">Компонент `mgt-login` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-162">The `mgt-login` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="8dd6c-163">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из значений, указанных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-163">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="8dd6c-164">Тип данных</span><span class="sxs-lookup"><span data-stu-id="8dd6c-164">Data type</span></span> | <span data-ttu-id="8dd6c-165">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="8dd6c-165">Data context</span></span> | <span data-ttu-id="8dd6c-166">Описание</span><span class="sxs-lookup"><span data-stu-id="8dd6c-166">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="8dd6c-167">signed-in-button-content</span><span class="sxs-lookup"><span data-stu-id="8dd6c-167">signed-in-button-content</span></span> | <span data-ttu-id="8dd6c-168">personDetails: объект пользователя, `personImage`: строка изображения пользователя</span><span class="sxs-lookup"><span data-stu-id="8dd6c-168">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="8dd6c-169">Шаблон, используемый для отображения содержимого в кнопке, если пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-169">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="8dd6c-170">signed-out-button-content</span><span class="sxs-lookup"><span data-stu-id="8dd6c-170">signed-out-button-content</span></span> | <span data-ttu-id="8dd6c-171">null</span><span class="sxs-lookup"><span data-stu-id="8dd6c-171">null</span></span> | <span data-ttu-id="8dd6c-172">Шаблон, используемый для отображения содержимого в кнопке, если пользователь не выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-172">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="8dd6c-173">flyout-commands</span><span class="sxs-lookup"><span data-stu-id="8dd6c-173">flyout-commands</span></span> | <span data-ttu-id="8dd6c-174">handleSignOut: функция выхода</span><span class="sxs-lookup"><span data-stu-id="8dd6c-174">handleSignOut: sign out function</span></span> | <span data-ttu-id="8dd6c-175">Шаблон, используемый для отображения команд во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-175">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="8dd6c-176">flyout-person-details</span><span class="sxs-lookup"><span data-stu-id="8dd6c-176">flyout-person-details</span></span> | <span data-ttu-id="8dd6c-177">personDetails: объект пользователя, personImage: строка изображения пользователя</span><span class="sxs-lookup"><span data-stu-id="8dd6c-177">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="8dd6c-178">Шаблон, используемый для отображения сведений о пользователе во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-178">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="8dd6c-179">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8dd6c-179">Microsoft Graph permissions</span></span>

<span data-ttu-id="8dd6c-180">Этот компонент использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-180">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="8dd6c-181">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="8dd6c-181">Configuration</span></span> | <span data-ttu-id="8dd6c-182">Разрешение</span><span class="sxs-lookup"><span data-stu-id="8dd6c-182">Permission</span></span> | <span data-ttu-id="8dd6c-183">API</span><span class="sxs-lookup"><span data-stu-id="8dd6c-183">API</span></span>
| - | - | - |
| <span data-ttu-id="8dd6c-184">default</span><span class="sxs-lookup"><span data-stu-id="8dd6c-184">default</span></span> | <span data-ttu-id="8dd6c-185">User.Read</span><span class="sxs-lookup"><span data-stu-id="8dd6c-185">User.Read</span></span> | [<span data-ttu-id="8dd6c-186">/users/me/</span><span class="sxs-lookup"><span data-stu-id="8dd6c-186">/users/me/</span></span>](/graph/api/user-get) |

<span data-ttu-id="8dd6c-187">При использовании шаблонов по умолчанию этот компонент использует компонент Person для отображения пользователя и наследует `signed-in-button-content` `flyout-person-details` все разрешения. [](./person.md)</span><span class="sxs-lookup"><span data-stu-id="8dd6c-187">When using the default `signed-in-button-content` and `flyout-person-details` templates, this component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span>

## <a name="authentication"></a><span data-ttu-id="8dd6c-188">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="8dd6c-188">Authentication</span></span>

<span data-ttu-id="8dd6c-189">В элементе управления входом используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="8dd6c-189">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="cache"></a><span data-ttu-id="8dd6c-190">Кэш</span><span class="sxs-lookup"><span data-stu-id="8dd6c-190">Cache</span></span>

<span data-ttu-id="8dd6c-191">Этот компонент использует [компонент Person](./person.md) для отображения пользователя и наследует всю конфигурацию кэша из него.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-191">This component uses the [Person component](./person.md) to display the user and inherits all cache configuration from it.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="8dd6c-192">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="8dd6c-192">Extend for more control</span></span>

<span data-ttu-id="8dd6c-193">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-193">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="8dd6c-194">Метод</span><span class="sxs-lookup"><span data-stu-id="8dd6c-194">Method</span></span> | <span data-ttu-id="8dd6c-195">Описание</span><span class="sxs-lookup"><span data-stu-id="8dd6c-195">Description</span></span> |
| - | - |
| <span data-ttu-id="8dd6c-196">renderButton</span><span class="sxs-lookup"><span data-stu-id="8dd6c-196">renderButton</span></span> | <span data-ttu-id="8dd6c-197">Отображает хром кнопки.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-197">Renders the button chrome.</span></span> |
| <span data-ttu-id="8dd6c-198">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="8dd6c-198">renderButtonContent</span></span> | <span data-ttu-id="8dd6c-199">Отображает содержимое кнопки.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-199">Renders the button content.</span></span> |
| <span data-ttu-id="8dd6c-200">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="8dd6c-200">renderSignedInButtonContent</span></span> | <span data-ttu-id="8dd6c-201">Отображение содержимого кнопки, если пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-201">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="8dd6c-202">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="8dd6c-202">renderSignedOutButtonContent</span></span> | <span data-ttu-id="8dd6c-203">Отображение содержимого кнопки, если пользователь не выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-203">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="8dd6c-204">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="8dd6c-204">renderFlyout</span></span> | <span data-ttu-id="8dd6c-205">Отображает хром всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-205">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="8dd6c-206">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="8dd6c-206">renderFlyoutContent</span></span> | <span data-ttu-id="8dd6c-207">Отображает содержимое всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-207">Renders the flyout content.</span></span> |
| <span data-ttu-id="8dd6c-208">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="8dd6c-208">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="8dd6c-209">Отображение сведений о пользователе во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-209">Render the flyout person details.</span></span> |
| <span data-ttu-id="8dd6c-210">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="8dd6c-210">renderFlyoutCommands</span></span> | <span data-ttu-id="8dd6c-211">Отображение команд всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-211">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="8dd6c-212">Создание собственного всплывающего окна</span><span class="sxs-lookup"><span data-stu-id="8dd6c-212">Bring your own flyout</span></span>

<span data-ttu-id="8dd6c-213">Можно использовать собственный компонент всплывающего окна вместо встроенного, переопределив метод `renderFlyout()` и предоставив новое всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-213">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="8dd6c-214">В этом случае нужно убедиться, что компонент входа продолжает правильно работать, переопределяя методы отображения всплывающего окна `protected`, чтобы изменить видимость альтернативного всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-214">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="8dd6c-215">Метод</span><span class="sxs-lookup"><span data-stu-id="8dd6c-215">Method</span></span> | <span data-ttu-id="8dd6c-216">Описание</span><span class="sxs-lookup"><span data-stu-id="8dd6c-216">Description</span></span> |
| - | - |
| <span data-ttu-id="8dd6c-217">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="8dd6c-217">hideFlyout</span></span> | <span data-ttu-id="8dd6c-218">Закрывает всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-218">Dismisses the flyout.</span></span> |
| <span data-ttu-id="8dd6c-219">showFlyout</span><span class="sxs-lookup"><span data-stu-id="8dd6c-219">showFlyout</span></span> | <span data-ttu-id="8dd6c-220">Отображает всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-220">Displays the flyout.</span></span> |
| <span data-ttu-id="8dd6c-221">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="8dd6c-221">toggleFlyout</span></span> | <span data-ttu-id="8dd6c-222">Переключает состояние всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="8dd6c-222">Toggles the state of the flyout.</span></span> |
