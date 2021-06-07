---
title: Компонент входа в Microsoft Graph Toolkit
description: Компонент входа — это кнопка и всплывающий элемент управления, предназначенные для упрощения проверки подлинности платформы удостоверений Майкрософт.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: ea7df01c77900eecc415b3670db0ea2736447d8c
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781081"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="9be20-103">Компонент входа в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="9be20-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="9be20-104">Компонент входа — это кнопка и всплывающий элемент управления, предназначенные для упрощения проверки подлинности платформы удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="9be20-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="9be20-105">Он обеспечивает два состояния:</span><span class="sxs-lookup"><span data-stu-id="9be20-105">It provides two states:</span></span>
* <span data-ttu-id="9be20-106">Если пользователь не вошел в систему, элемент управления является простой кнопкой для запуска входа в систему.</span><span class="sxs-lookup"><span data-stu-id="9be20-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="9be20-107">Если пользователь вошел в систему, элемент управления отображает имя, изображение профиля и электронную почту вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="9be20-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="9be20-108">При щелчке открывается всплывающее окно с командой для выхода.</span><span class="sxs-lookup"><span data-stu-id="9be20-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="9be20-109">Пример</span><span class="sxs-lookup"><span data-stu-id="9be20-109">Example</span></span>

<span data-ttu-id="9be20-110">В примере ниже показан компонент `mgt-login` с указанием вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="9be20-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="9be20-111">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="9be20-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="9be20-112">Использование элемента управления без поставщика проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="9be20-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="9be20-113">По умолчанию компонент поддерживает поставщика и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9be20-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="9be20-114">Но если вы хотите указать свою логику и проверку подлинности, вы можете воспользоваться свойством `userDetails`, чтобы настроить сведения о вошедшем пользователе.</span><span class="sxs-lookup"><span data-stu-id="9be20-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="9be20-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="9be20-115">Attribute</span></span> | <span data-ttu-id="9be20-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="9be20-116">Property</span></span> | <span data-ttu-id="9be20-117">Описание</span><span class="sxs-lookup"><span data-stu-id="9be20-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="9be20-118">user-details</span><span class="sxs-lookup"><span data-stu-id="9be20-118">user-details</span></span> | <span data-ttu-id="9be20-119">userDetails</span><span class="sxs-lookup"><span data-stu-id="9be20-119">userDetails</span></span> | <span data-ttu-id="9be20-120">Настройка объекта пользователя, который будет отображаться в элементе управления.</span><span class="sxs-lookup"><span data-stu-id="9be20-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="9be20-121">В примере ниже настраиваются сведения о пользователе.</span><span class="sxs-lookup"><span data-stu-id="9be20-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="9be20-122">Присвоение параметру `userDetails` значения `null` обеспечивает переход к состоянию выхода.</span><span class="sxs-lookup"><span data-stu-id="9be20-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="9be20-123">Чтобы обрабатывать вход и выход, используйте события `loginInitiated` и `logoutInitiated`.</span><span class="sxs-lookup"><span data-stu-id="9be20-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="9be20-124">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="9be20-124">CSS custom properties</span></span>

<span data-ttu-id="9be20-125">Компонент `mgt-login` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="9be20-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="9be20-126">Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="9be20-126">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="9be20-127">События</span><span class="sxs-lookup"><span data-stu-id="9be20-127">Events</span></span>

<span data-ttu-id="9be20-128">Из элемента управления инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="9be20-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="9be20-129">Событие</span><span class="sxs-lookup"><span data-stu-id="9be20-129">Event</span></span> | <span data-ttu-id="9be20-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9be20-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="9be20-131">Пользователь нажмет кнопку входа, чтобы начать вход в систему — можно отменить.</span><span class="sxs-lookup"><span data-stu-id="9be20-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="9be20-132">Вход выполнен успешно, и пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="9be20-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="9be20-133">Пользователь отменил вход в систему или не смог выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="9be20-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="9be20-134">Пользователь начал выход из системы — можно отменить.</span><span class="sxs-lookup"><span data-stu-id="9be20-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="9be20-135">Пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="9be20-135">The user signed out.</span></span> |

## <a name="templates"></a><span data-ttu-id="9be20-136">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="9be20-136">Templates</span></span>

<span data-ttu-id="9be20-137">Компонент `mgt-login` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="9be20-137">The `mgt-login` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="9be20-138">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из значений, указанных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="9be20-138">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="9be20-139">Тип данных</span><span class="sxs-lookup"><span data-stu-id="9be20-139">Data type</span></span> | <span data-ttu-id="9be20-140">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="9be20-140">Data context</span></span> | <span data-ttu-id="9be20-141">Описание</span><span class="sxs-lookup"><span data-stu-id="9be20-141">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="9be20-142">signed-in-button-content</span><span class="sxs-lookup"><span data-stu-id="9be20-142">signed-in-button-content</span></span> | <span data-ttu-id="9be20-143">personDetails: объект пользователя, `personImage`: строка изображения пользователя</span><span class="sxs-lookup"><span data-stu-id="9be20-143">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="9be20-144">Шаблон, используемый для отображения содержимого в кнопке, если пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="9be20-144">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="9be20-145">signed-out-button-content</span><span class="sxs-lookup"><span data-stu-id="9be20-145">signed-out-button-content</span></span> | <span data-ttu-id="9be20-146">null</span><span class="sxs-lookup"><span data-stu-id="9be20-146">null</span></span> | <span data-ttu-id="9be20-147">Шаблон, используемый для отображения содержимого в кнопке, если пользователь не выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="9be20-147">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="9be20-148">flyout-commands</span><span class="sxs-lookup"><span data-stu-id="9be20-148">flyout-commands</span></span> | <span data-ttu-id="9be20-149">handleSignOut: функция выхода</span><span class="sxs-lookup"><span data-stu-id="9be20-149">handleSignOut: sign out function</span></span> | <span data-ttu-id="9be20-150">Шаблон, используемый для отображения команд во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="9be20-150">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="9be20-151">flyout-person-details</span><span class="sxs-lookup"><span data-stu-id="9be20-151">flyout-person-details</span></span> | <span data-ttu-id="9be20-152">personDetails: объект пользователя, personImage: строка изображения пользователя</span><span class="sxs-lookup"><span data-stu-id="9be20-152">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="9be20-153">Шаблон, используемый для отображения сведений о пользователе во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="9be20-153">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="9be20-154">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9be20-154">Microsoft Graph permissions</span></span>

<span data-ttu-id="9be20-155">Этот компонент использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9be20-155">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="9be20-156">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="9be20-156">Configuration</span></span> | <span data-ttu-id="9be20-157">Разрешение</span><span class="sxs-lookup"><span data-stu-id="9be20-157">Permission</span></span> | <span data-ttu-id="9be20-158">API</span><span class="sxs-lookup"><span data-stu-id="9be20-158">API</span></span>
| - | - | - |
| <span data-ttu-id="9be20-159">default</span><span class="sxs-lookup"><span data-stu-id="9be20-159">default</span></span> | <span data-ttu-id="9be20-160">User.Read</span><span class="sxs-lookup"><span data-stu-id="9be20-160">User.Read</span></span> | [<span data-ttu-id="9be20-161">/users/me/</span><span class="sxs-lookup"><span data-stu-id="9be20-161">/users/me/</span></span>](/graph/api/user-get) |

<span data-ttu-id="9be20-162">При использовании шаблонов по умолчанию этот компонент использует компонент Person для отображения пользователя и наследует `signed-in-button-content` `flyout-person-details` все разрешения. [](./person.md)</span><span class="sxs-lookup"><span data-stu-id="9be20-162">When using the default `signed-in-button-content` and `flyout-person-details` templates, this component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span>

## <a name="authentication"></a><span data-ttu-id="9be20-163">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="9be20-163">Authentication</span></span>

<span data-ttu-id="9be20-164">В элементе управления входом используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="9be20-164">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="cache"></a><span data-ttu-id="9be20-165">Кэш</span><span class="sxs-lookup"><span data-stu-id="9be20-165">Cache</span></span>

<span data-ttu-id="9be20-166">Этот компонент использует [компонент Person](./person.md) для отображения пользователя и наследует всю конфигурацию кэша из него.</span><span class="sxs-lookup"><span data-stu-id="9be20-166">This component uses the [Person component](./person.md) to display the user and inherits all cache configuration from it.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="9be20-167">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="9be20-167">Extend for more control</span></span>

<span data-ttu-id="9be20-168">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="9be20-168">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="9be20-169">Метод</span><span class="sxs-lookup"><span data-stu-id="9be20-169">Method</span></span> | <span data-ttu-id="9be20-170">Описание</span><span class="sxs-lookup"><span data-stu-id="9be20-170">Description</span></span> |
| - | - |
| <span data-ttu-id="9be20-171">renderButton</span><span class="sxs-lookup"><span data-stu-id="9be20-171">renderButton</span></span> | <span data-ttu-id="9be20-172">Отображает хром кнопки.</span><span class="sxs-lookup"><span data-stu-id="9be20-172">Renders the button chrome.</span></span> |
| <span data-ttu-id="9be20-173">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="9be20-173">renderButtonContent</span></span> | <span data-ttu-id="9be20-174">Отображает содержимое кнопки.</span><span class="sxs-lookup"><span data-stu-id="9be20-174">Renders the button content.</span></span> |
| <span data-ttu-id="9be20-175">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="9be20-175">renderSignedInButtonContent</span></span> | <span data-ttu-id="9be20-176">Отображение содержимого кнопки, если пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="9be20-176">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="9be20-177">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="9be20-177">renderSignedOutButtonContent</span></span> | <span data-ttu-id="9be20-178">Отображение содержимого кнопки, если пользователь не выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="9be20-178">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="9be20-179">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="9be20-179">renderFlyout</span></span> | <span data-ttu-id="9be20-180">Отображает хром всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="9be20-180">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="9be20-181">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="9be20-181">renderFlyoutContent</span></span> | <span data-ttu-id="9be20-182">Отображает содержимое всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="9be20-182">Renders the flyout content.</span></span> |
| <span data-ttu-id="9be20-183">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="9be20-183">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="9be20-184">Отображение сведений о пользователе во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="9be20-184">Render the flyout person details.</span></span> |
| <span data-ttu-id="9be20-185">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="9be20-185">renderFlyoutCommands</span></span> | <span data-ttu-id="9be20-186">Отображение команд всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="9be20-186">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="9be20-187">Создание собственного всплывающего окна</span><span class="sxs-lookup"><span data-stu-id="9be20-187">Bring your own flyout</span></span>

<span data-ttu-id="9be20-188">Можно использовать собственный компонент всплывающего окна вместо встроенного, переопределив метод `renderFlyout()` и предоставив новое всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="9be20-188">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="9be20-189">В этом случае нужно убедиться, что компонент входа продолжает правильно работать, переопределяя методы отображения всплывающего окна `protected`, чтобы изменить видимость альтернативного всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="9be20-189">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="9be20-190">Метод</span><span class="sxs-lookup"><span data-stu-id="9be20-190">Method</span></span> | <span data-ttu-id="9be20-191">Описание</span><span class="sxs-lookup"><span data-stu-id="9be20-191">Description</span></span> |
| - | - |
| <span data-ttu-id="9be20-192">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="9be20-192">hideFlyout</span></span> | <span data-ttu-id="9be20-193">Закрывает всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="9be20-193">Dismisses the flyout.</span></span> |
| <span data-ttu-id="9be20-194">showFlyout</span><span class="sxs-lookup"><span data-stu-id="9be20-194">showFlyout</span></span> | <span data-ttu-id="9be20-195">Отображает всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="9be20-195">Displays the flyout.</span></span> |
| <span data-ttu-id="9be20-196">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="9be20-196">toggleFlyout</span></span> | <span data-ttu-id="9be20-197">Переключает состояние всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="9be20-197">Toggles the state of the flyout.</span></span> |
