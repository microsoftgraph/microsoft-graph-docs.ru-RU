---
title: Компонент входа в Microsoft Graph Toolkit
description: Компонент входа — это кнопка и всплывающий элемент управления, предназначенные для упрощения проверки подлинности платформы удостоверений Майкрософт.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: a54dfaede64216e8a2254aedb06cf6aa41aaa295
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660067"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="3dffa-103">Компонент входа в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="3dffa-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="3dffa-104">Компонент входа — это кнопка и всплывающий элемент управления, предназначенные для упрощения проверки подлинности платформы удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="3dffa-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="3dffa-105">Он обеспечивает два состояния:</span><span class="sxs-lookup"><span data-stu-id="3dffa-105">It provides two states:</span></span>
* <span data-ttu-id="3dffa-106">Если пользователь не вошел в систему, элемент управления является простой кнопкой для запуска входа в систему.</span><span class="sxs-lookup"><span data-stu-id="3dffa-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="3dffa-107">Если пользователь вошел в систему, элемент управления отображает имя, изображение профиля и электронную почту вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="3dffa-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="3dffa-108">При щелчке открывается всплывающее окно с командой для выхода.</span><span class="sxs-lookup"><span data-stu-id="3dffa-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="3dffa-109">Пример</span><span class="sxs-lookup"><span data-stu-id="3dffa-109">Example</span></span>

<span data-ttu-id="3dffa-110">В примере ниже показан компонент `mgt-login` с указанием вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="3dffa-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="3dffa-111">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="3dffa-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="3dffa-112">Использование элемента управления без поставщика проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="3dffa-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="3dffa-113">По умолчанию компонент поддерживает поставщика и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3dffa-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="3dffa-114">Но если вы хотите указать свою логику и проверку подлинности, вы можете воспользоваться свойством `userDetails`, чтобы настроить сведения о вошедшем пользователе.</span><span class="sxs-lookup"><span data-stu-id="3dffa-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="3dffa-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="3dffa-115">Attribute</span></span> | <span data-ttu-id="3dffa-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="3dffa-116">Property</span></span> | <span data-ttu-id="3dffa-117">Описание</span><span class="sxs-lookup"><span data-stu-id="3dffa-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="3dffa-118">user-details</span><span class="sxs-lookup"><span data-stu-id="3dffa-118">user-details</span></span> | <span data-ttu-id="3dffa-119">userDetails</span><span class="sxs-lookup"><span data-stu-id="3dffa-119">userDetails</span></span> | <span data-ttu-id="3dffa-120">Настройка объекта пользователя, который будет отображаться в элементе управления.</span><span class="sxs-lookup"><span data-stu-id="3dffa-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="3dffa-121">В примере ниже настраиваются сведения о пользователе.</span><span class="sxs-lookup"><span data-stu-id="3dffa-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="3dffa-122">Присвоение параметру `userDetails` значения `null` обеспечивает переход к состоянию выхода.</span><span class="sxs-lookup"><span data-stu-id="3dffa-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="3dffa-123">Чтобы обрабатывать вход и выход, используйте события `loginInitiated` и `logoutInitiated`.</span><span class="sxs-lookup"><span data-stu-id="3dffa-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="3dffa-124">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="3dffa-124">CSS custom properties</span></span>

<span data-ttu-id="3dffa-125">Компонент `mgt-login` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="3dffa-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="3dffa-126">Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="3dffa-126">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="3dffa-127">События</span><span class="sxs-lookup"><span data-stu-id="3dffa-127">Events</span></span>

<span data-ttu-id="3dffa-128">Из элемента управления инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="3dffa-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="3dffa-129">Событие</span><span class="sxs-lookup"><span data-stu-id="3dffa-129">Event</span></span> | <span data-ttu-id="3dffa-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3dffa-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="3dffa-131">Пользователь нажмет кнопку входа, чтобы начать вход в систему — можно отменить.</span><span class="sxs-lookup"><span data-stu-id="3dffa-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="3dffa-132">Вход выполнен успешно, и пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="3dffa-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="3dffa-133">Пользователь отменил вход в систему или не смог выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="3dffa-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="3dffa-134">Пользователь начал выход из системы — можно отменить.</span><span class="sxs-lookup"><span data-stu-id="3dffa-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="3dffa-135">Пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="3dffa-135">The user signed out.</span></span> |

## <a name="templates"></a><span data-ttu-id="3dffa-136">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="3dffa-136">Templates</span></span>

<span data-ttu-id="3dffa-137">Компонент `mgt-login` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="3dffa-137">The `mgt-login` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="3dffa-138">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из значений, указанных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="3dffa-138">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="3dffa-139">Тип данных</span><span class="sxs-lookup"><span data-stu-id="3dffa-139">Data type</span></span> | <span data-ttu-id="3dffa-140">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="3dffa-140">Data context</span></span> | <span data-ttu-id="3dffa-141">Описание</span><span class="sxs-lookup"><span data-stu-id="3dffa-141">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="3dffa-142">signed-in-button-content</span><span class="sxs-lookup"><span data-stu-id="3dffa-142">signed-in-button-content</span></span> | <span data-ttu-id="3dffa-143">personDetails: объект пользователя, `personImage`: строка изображения пользователя</span><span class="sxs-lookup"><span data-stu-id="3dffa-143">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="3dffa-144">Шаблон, используемый для отображения содержимого в кнопке, если пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="3dffa-144">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="3dffa-145">signed-out-button-content</span><span class="sxs-lookup"><span data-stu-id="3dffa-145">signed-out-button-content</span></span> | <span data-ttu-id="3dffa-146">null</span><span class="sxs-lookup"><span data-stu-id="3dffa-146">null</span></span> | <span data-ttu-id="3dffa-147">Шаблон, используемый для отображения содержимого в кнопке, если пользователь не выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="3dffa-147">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="3dffa-148">flyout-commands</span><span class="sxs-lookup"><span data-stu-id="3dffa-148">flyout-commands</span></span> | <span data-ttu-id="3dffa-149">handleSignOut: функция выхода</span><span class="sxs-lookup"><span data-stu-id="3dffa-149">handleSignOut: sign out function</span></span> | <span data-ttu-id="3dffa-150">Шаблон, используемый для отображения команд во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="3dffa-150">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="3dffa-151">flyout-person-details</span><span class="sxs-lookup"><span data-stu-id="3dffa-151">flyout-person-details</span></span> | <span data-ttu-id="3dffa-152">personDetails: объект пользователя, personImage: строка изображения пользователя</span><span class="sxs-lookup"><span data-stu-id="3dffa-152">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="3dffa-153">Шаблон, используемый для отображения сведений о пользователе во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="3dffa-153">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="3dffa-154">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3dffa-154">Microsoft Graph permissions</span></span>

<span data-ttu-id="3dffa-155">Этот компонент использует компонент [Person](./person.md) для отображения пользователя и наследует все разрешения.</span><span class="sxs-lookup"><span data-stu-id="3dffa-155">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="3dffa-156">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="3dffa-156">Authentication</span></span>

<span data-ttu-id="3dffa-157">В элементе управления входом используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="3dffa-157">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="extend-for-more-control"></a><span data-ttu-id="3dffa-158">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="3dffa-158">Extend for more control</span></span>

<span data-ttu-id="3dffa-159">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="3dffa-159">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="3dffa-160">Метод</span><span class="sxs-lookup"><span data-stu-id="3dffa-160">Method</span></span> | <span data-ttu-id="3dffa-161">Описание</span><span class="sxs-lookup"><span data-stu-id="3dffa-161">Description</span></span> |
| - | - |
| <span data-ttu-id="3dffa-162">renderButton</span><span class="sxs-lookup"><span data-stu-id="3dffa-162">renderButton</span></span> | <span data-ttu-id="3dffa-163">Отображает хром кнопки.</span><span class="sxs-lookup"><span data-stu-id="3dffa-163">Renders the button chrome.</span></span> |
| <span data-ttu-id="3dffa-164">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="3dffa-164">renderButtonContent</span></span> | <span data-ttu-id="3dffa-165">Отображает содержимое кнопки.</span><span class="sxs-lookup"><span data-stu-id="3dffa-165">Renders the button content.</span></span> |
| <span data-ttu-id="3dffa-166">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="3dffa-166">renderSignedInButtonContent</span></span> | <span data-ttu-id="3dffa-167">Отображение содержимого кнопки, если пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="3dffa-167">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="3dffa-168">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="3dffa-168">renderSignedOutButtonContent</span></span> | <span data-ttu-id="3dffa-169">Отображение содержимого кнопки, если пользователь не выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="3dffa-169">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="3dffa-170">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="3dffa-170">renderFlyout</span></span> | <span data-ttu-id="3dffa-171">Отображает хром всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="3dffa-171">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="3dffa-172">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="3dffa-172">renderFlyoutContent</span></span> | <span data-ttu-id="3dffa-173">Отображает содержимое всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="3dffa-173">Renders the flyout content.</span></span> |
| <span data-ttu-id="3dffa-174">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="3dffa-174">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="3dffa-175">Отображение сведений о пользователе во всплывающем окне.</span><span class="sxs-lookup"><span data-stu-id="3dffa-175">Render the flyout person details.</span></span> |
| <span data-ttu-id="3dffa-176">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="3dffa-176">renderFlyoutCommands</span></span> | <span data-ttu-id="3dffa-177">Отображение команд всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="3dffa-177">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="3dffa-178">Создание собственного всплывающего окна</span><span class="sxs-lookup"><span data-stu-id="3dffa-178">Bring your own flyout</span></span>

<span data-ttu-id="3dffa-179">Можно использовать собственный компонент всплывающего окна вместо встроенного, переопределив метод `renderFlyout()` и предоставив новое всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="3dffa-179">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="3dffa-180">В этом случае нужно убедиться, что компонент входа продолжает правильно работать, переопределяя методы отображения всплывающего окна `protected`, чтобы изменить видимость альтернативного всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="3dffa-180">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="3dffa-181">Метод</span><span class="sxs-lookup"><span data-stu-id="3dffa-181">Method</span></span> | <span data-ttu-id="3dffa-182">Описание</span><span class="sxs-lookup"><span data-stu-id="3dffa-182">Description</span></span> |
| - | - |
| <span data-ttu-id="3dffa-183">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="3dffa-183">hideFlyout</span></span> | <span data-ttu-id="3dffa-184">Закрывает всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="3dffa-184">Dismisses the flyout.</span></span> |
| <span data-ttu-id="3dffa-185">showFlyout</span><span class="sxs-lookup"><span data-stu-id="3dffa-185">showFlyout</span></span> | <span data-ttu-id="3dffa-186">Отображает всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="3dffa-186">Displays the flyout.</span></span> |
| <span data-ttu-id="3dffa-187">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="3dffa-187">toggleFlyout</span></span> | <span data-ttu-id="3dffa-188">Переключает состояние всплывающего окна.</span><span class="sxs-lookup"><span data-stu-id="3dffa-188">Toggles the state of the flyout.</span></span> |
