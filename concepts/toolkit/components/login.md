---
title: Компонент входа в Microsoft Graph Toolkit
description: Компонент входа — это кнопка и всплывающий элемент управления, предназначенные для упрощения проверки подлинности платформы удостоверений Майкрософт.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 1042201492720dce92016a13bd7bbd8477ce2d2c
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082155"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="a90b0-103">Компонент входа в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="a90b0-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="a90b0-104">Компонент входа — это кнопка и всплывающий элемент управления, предназначенные для упрощения проверки подлинности платформы удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="a90b0-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="a90b0-105">Он обеспечивает два состояния:</span><span class="sxs-lookup"><span data-stu-id="a90b0-105">It provides two states:</span></span>
* <span data-ttu-id="a90b0-106">Если пользователь не вошел в систему, элемент управления является простой кнопкой для запуска входа в систему.</span><span class="sxs-lookup"><span data-stu-id="a90b0-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="a90b0-107">Если пользователь вошел в систему, элемент управления отображает имя, изображение профиля и электронную почту вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="a90b0-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="a90b0-108">При щелчке открывается всплывающее окно с командой для выхода.</span><span class="sxs-lookup"><span data-stu-id="a90b0-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="a90b0-109">Пример</span><span class="sxs-lookup"><span data-stu-id="a90b0-109">Example</span></span>

<span data-ttu-id="a90b0-110">В примере ниже показан компонент `mgt-login` с указанием вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="a90b0-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="a90b0-111">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="a90b0-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="a90b0-112">Использование элемента управления без поставщика проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="a90b0-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="a90b0-113">По умолчанию компонент поддерживает поставщика и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a90b0-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="a90b0-114">Но если вы хотите указать свою логику и проверку подлинности, вы можете воспользоваться свойством `userDetails`, чтобы настроить сведения о вошедшем пользователе.</span><span class="sxs-lookup"><span data-stu-id="a90b0-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="a90b0-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="a90b0-115">Attribute</span></span> | <span data-ttu-id="a90b0-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="a90b0-116">Property</span></span> | <span data-ttu-id="a90b0-117">Описание</span><span class="sxs-lookup"><span data-stu-id="a90b0-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="a90b0-118">user-details</span><span class="sxs-lookup"><span data-stu-id="a90b0-118">user-details</span></span> | <span data-ttu-id="a90b0-119">userDetails</span><span class="sxs-lookup"><span data-stu-id="a90b0-119">userDetails</span></span> | <span data-ttu-id="a90b0-120">Настройка объекта пользователя, который будет отображаться в элементе управления.</span><span class="sxs-lookup"><span data-stu-id="a90b0-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="a90b0-121">В примере ниже настраиваются сведения о пользователе.</span><span class="sxs-lookup"><span data-stu-id="a90b0-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="a90b0-122">Присвоение параметру `userDetails` значения `null` обеспечивает переход к состоянию выхода.</span><span class="sxs-lookup"><span data-stu-id="a90b0-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="a90b0-123">Чтобы обрабатывать вход и выход, используйте события `loginInitiated` и `logoutInitiated`.</span><span class="sxs-lookup"><span data-stu-id="a90b0-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="a90b0-124">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="a90b0-124">CSS custom properties</span></span>

<span data-ttu-id="a90b0-125">Компонент `mgt-login` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="a90b0-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="a90b0-126">Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="a90b0-126">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="a90b0-127">События</span><span class="sxs-lookup"><span data-stu-id="a90b0-127">Events</span></span>

<span data-ttu-id="a90b0-128">Из элемента управления инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="a90b0-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="a90b0-129">Событие</span><span class="sxs-lookup"><span data-stu-id="a90b0-129">Event</span></span> | <span data-ttu-id="a90b0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a90b0-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="a90b0-131">Пользователь нажмет кнопку входа, чтобы начать вход в систему — можно отменить.</span><span class="sxs-lookup"><span data-stu-id="a90b0-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="a90b0-132">Вход выполнен успешно, и пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="a90b0-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="a90b0-133">Пользователь отменил вход в систему или не смог выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="a90b0-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="a90b0-134">Пользователь начал выход из системы — можно отменить.</span><span class="sxs-lookup"><span data-stu-id="a90b0-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="a90b0-135">Пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="a90b0-135">The user signed out.</span></span> |

<span data-ttu-id="a90b0-136">Дополнительные сведения об обработке событий см. в [этой работе.](../customize-components/events.md)</span><span class="sxs-lookup"><span data-stu-id="a90b0-136">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="a90b0-137">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="a90b0-137">Templates</span></span>

<span data-ttu-id="a90b0-138">Компонент `mgt-login` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="a90b0-138">The `mgt-login` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="a90b0-139">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из значений, указанных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a90b0-139">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="a90b0-140">Тип данных</span><span class="sxs-lookup"><span data-stu-id="a90b0-140">Data type</span></span> | <span data-ttu-id="a90b0-141">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="a90b0-141">Data context</span></span> | <span data-ttu-id="a90b0-142">Описание</span><span class="sxs-lookup"><span data-stu-id="a90b0-142">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="a90b0-143">signed-in-button-content</span><span class="sxs-lookup"><span data-stu-id="a90b0-143">signed-in-button-content</span></span> | <span data-ttu-id="a90b0-144">personDetails: объект пользователя, `personImage`: строка изображения пользователя</span><span class="sxs-lookup"><span data-stu-id="a90b0-144">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="a90b0-145">Шаблон, используемый для отображения содержимого в кнопке, если пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="a90b0-145">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="a90b0-146">signed-out-button-content</span><span class="sxs-lookup"><span data-stu-id="a90b0-146">signed-out-button-content</span></span> | <span data-ttu-id="a90b0-147">null</span><span class="sxs-lookup"><span data-stu-id="a90b0-147">null</span></span> | <span data-ttu-id="a90b0-148">Шаблон, используемый для отображения содержимого в кнопке, если пользователь не выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="a90b0-148">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="a90b0-149">flyout-commands</span><span class="sxs-lookup"><span data-stu-id="a90b0-149">flyout-commands</span></span> | <span data-ttu-id="a90b0-150">handleSignOut: функция выхода</span><span class="sxs-lookup"><span data-stu-id="a90b0-150">handleSignOut: sign out function</span></span> | <span data-ttu-id="a90b0-151">Шаблон, используемый для отображения команд во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="a90b0-151">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="a90b0-152">flyout-person-details</span><span class="sxs-lookup"><span data-stu-id="a90b0-152">flyout-person-details</span></span> | <span data-ttu-id="a90b0-153">personDetails: объект пользователя, personImage: строка изображения пользователя</span><span class="sxs-lookup"><span data-stu-id="a90b0-153">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="a90b0-154">Шаблон, используемый для отображения сведений о пользователе во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="a90b0-154">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="a90b0-155">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a90b0-155">Microsoft Graph permissions</span></span>

<span data-ttu-id="a90b0-156">Этот компонент использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a90b0-156">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="a90b0-157">Настройка</span><span class="sxs-lookup"><span data-stu-id="a90b0-157">Configuration</span></span> | <span data-ttu-id="a90b0-158">Разрешение</span><span class="sxs-lookup"><span data-stu-id="a90b0-158">Permission</span></span> | <span data-ttu-id="a90b0-159">API</span><span class="sxs-lookup"><span data-stu-id="a90b0-159">API</span></span>
| - | - | - |
| <span data-ttu-id="a90b0-160">default</span><span class="sxs-lookup"><span data-stu-id="a90b0-160">default</span></span> | <span data-ttu-id="a90b0-161">User.Read</span><span class="sxs-lookup"><span data-stu-id="a90b0-161">User.Read</span></span> | [<span data-ttu-id="a90b0-162">/users/me/</span><span class="sxs-lookup"><span data-stu-id="a90b0-162">/users/me/</span></span>](/graph/api/user-get) |

<span data-ttu-id="a90b0-163">При использовании шаблонов по умолчанию этот компонент использует компонент Person для отображения пользователя и наследует `signed-in-button-content` `flyout-person-details` все разрешения. [](./person.md)</span><span class="sxs-lookup"><span data-stu-id="a90b0-163">When using the default `signed-in-button-content` and `flyout-person-details` templates, this component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span>

## <a name="authentication"></a><span data-ttu-id="a90b0-164">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="a90b0-164">Authentication</span></span>

<span data-ttu-id="a90b0-165">В элементе управления входом используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="a90b0-165">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="cache"></a><span data-ttu-id="a90b0-166">Кэш</span><span class="sxs-lookup"><span data-stu-id="a90b0-166">Cache</span></span>

<span data-ttu-id="a90b0-167">Этот компонент использует [компонент Person](./person.md) для отображения пользователя и наследует всю конфигурацию кэша из него.</span><span class="sxs-lookup"><span data-stu-id="a90b0-167">This component uses the [Person component](./person.md) to display the user and inherits all cache configuration from it.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="a90b0-168">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="a90b0-168">Extend for more control</span></span>

<span data-ttu-id="a90b0-169">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="a90b0-169">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="a90b0-170">Метод</span><span class="sxs-lookup"><span data-stu-id="a90b0-170">Method</span></span> | <span data-ttu-id="a90b0-171">Описание</span><span class="sxs-lookup"><span data-stu-id="a90b0-171">Description</span></span> |
| - | - |
| <span data-ttu-id="a90b0-172">renderButton</span><span class="sxs-lookup"><span data-stu-id="a90b0-172">renderButton</span></span> | <span data-ttu-id="a90b0-173">Отображает хром кнопки.</span><span class="sxs-lookup"><span data-stu-id="a90b0-173">Renders the button chrome.</span></span> |
| <span data-ttu-id="a90b0-174">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="a90b0-174">renderButtonContent</span></span> | <span data-ttu-id="a90b0-175">Отображает содержимое кнопки.</span><span class="sxs-lookup"><span data-stu-id="a90b0-175">Renders the button content.</span></span> |
| <span data-ttu-id="a90b0-176">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="a90b0-176">renderSignedInButtonContent</span></span> | <span data-ttu-id="a90b0-177">Отображение содержимого кнопки, если пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="a90b0-177">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="a90b0-178">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="a90b0-178">renderSignedOutButtonContent</span></span> | <span data-ttu-id="a90b0-179">Отображение содержимого кнопки, если пользователь не выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="a90b0-179">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="a90b0-180">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="a90b0-180">renderFlyout</span></span> | <span data-ttu-id="a90b0-181">Отображает хром всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="a90b0-181">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="a90b0-182">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="a90b0-182">renderFlyoutContent</span></span> | <span data-ttu-id="a90b0-183">Отображает содержимое всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="a90b0-183">Renders the flyout content.</span></span> |
| <span data-ttu-id="a90b0-184">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="a90b0-184">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="a90b0-185">Отображение сведений о пользователе во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="a90b0-185">Render the flyout person details.</span></span> |
| <span data-ttu-id="a90b0-186">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="a90b0-186">renderFlyoutCommands</span></span> | <span data-ttu-id="a90b0-187">Отображение команд всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="a90b0-187">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="a90b0-188">Создание собственного всплывающего окна</span><span class="sxs-lookup"><span data-stu-id="a90b0-188">Bring your own flyout</span></span>

<span data-ttu-id="a90b0-189">Можно использовать собственный компонент всплывающего окна вместо встроенного, переопределив метод `renderFlyout()` и предоставив новое всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="a90b0-189">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="a90b0-190">В этом случае нужно убедиться, что компонент входа продолжает правильно работать, переопределяя методы отображения всплывающего окна `protected`, чтобы изменить видимость альтернативного всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="a90b0-190">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="a90b0-191">Метод</span><span class="sxs-lookup"><span data-stu-id="a90b0-191">Method</span></span> | <span data-ttu-id="a90b0-192">Описание</span><span class="sxs-lookup"><span data-stu-id="a90b0-192">Description</span></span> |
| - | - |
| <span data-ttu-id="a90b0-193">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="a90b0-193">hideFlyout</span></span> | <span data-ttu-id="a90b0-194">Закрывает всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="a90b0-194">Dismisses the flyout.</span></span> |
| <span data-ttu-id="a90b0-195">showFlyout</span><span class="sxs-lookup"><span data-stu-id="a90b0-195">showFlyout</span></span> | <span data-ttu-id="a90b0-196">Отображает всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="a90b0-196">Displays the flyout.</span></span> |
| <span data-ttu-id="a90b0-197">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="a90b0-197">toggleFlyout</span></span> | <span data-ttu-id="a90b0-198">Переключает состояние всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="a90b0-198">Toggles the state of the flyout.</span></span> |
