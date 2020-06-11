---
title: Компонент входа в набор средств Microsoft Graph
description: Компонент входа — это кнопка и всплывающий элемент управления для упрощения проверки подлинности на платформе Microsoft Identity.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 441639c309025eb8fefbbe551dd60b6324a7fd3c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682035"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="368bc-103">Компонент входа в набор средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="368bc-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="368bc-104">Компонент входа — это кнопка и всплывающий элемент управления для упрощения проверки подлинности на платформе Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="368bc-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="368bc-105">Он предоставляет два состояния:</span><span class="sxs-lookup"><span data-stu-id="368bc-105">It provides two states:</span></span>
* <span data-ttu-id="368bc-106">Если пользователь не вошел в систему, элемент управления является простой кнопкой для запуска процесса входа.</span><span class="sxs-lookup"><span data-stu-id="368bc-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="368bc-107">Когда пользователь вошел в систему, элемент управления отображает имя пользователя, изображение профиля и адрес электронной почты, которые вошли в систему.</span><span class="sxs-lookup"><span data-stu-id="368bc-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="368bc-108">При нажатии открывается раскрывающееся меню с командой для выхода.</span><span class="sxs-lookup"><span data-stu-id="368bc-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="368bc-109">Пример</span><span class="sxs-lookup"><span data-stu-id="368bc-109">Example</span></span>

<span data-ttu-id="368bc-110">В следующем примере показан `mgt-login` компонент с пользователь, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="368bc-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="368bc-111">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="368bc-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="368bc-112">Использование элемента управления без поставщика проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="368bc-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="368bc-113">Компонент работает с поставщиком и Microsoft Graph из этого ящика.</span><span class="sxs-lookup"><span data-stu-id="368bc-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="368bc-114">Тем не менее, если вы хотите предоставить собственную логику и проверку подлинности, вы можете использовать `userDetails` свойство, чтобы задать сведения о пользователе, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="368bc-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="368bc-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="368bc-115">Attribute</span></span> | <span data-ttu-id="368bc-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="368bc-116">Property</span></span> | <span data-ttu-id="368bc-117">Описание</span><span class="sxs-lookup"><span data-stu-id="368bc-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="368bc-118">пользователь — сведения</span><span class="sxs-lookup"><span data-stu-id="368bc-118">user-details</span></span> | <span data-ttu-id="368bc-119">усердетаилс</span><span class="sxs-lookup"><span data-stu-id="368bc-119">userDetails</span></span> | <span data-ttu-id="368bc-120">Задайте объект пользователя, который будет отображаться в элементе управления.</span><span class="sxs-lookup"><span data-stu-id="368bc-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="368bc-121">В приведенном ниже примере задаются сведения о лице.</span><span class="sxs-lookup"><span data-stu-id="368bc-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="368bc-122">Для параметра значение будет указано состояние "выход `userDetails` `null` выполнен".</span><span class="sxs-lookup"><span data-stu-id="368bc-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="368bc-123">Используйте `loginInitiated` события и `logoutInitiated` для обработки входа и выхода из нее.</span><span class="sxs-lookup"><span data-stu-id="368bc-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="368bc-124">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="368bc-124">CSS custom properties</span></span>

<span data-ttu-id="368bc-125">`mgt-login`Компонент определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="368bc-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

```css
mgt-login {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --margin: 0;
  --padding: 12px 20px;
  --color: #201f1e;
  --color-hover: var(--theme-primary-color);
  --background-color: transparent;
  --background-color--hover: #edebe9;
  --popup-content-background-color: white;
  --popup-command-font-size: 12px;
  --popup-color: #201f1e;
}
```

<span data-ttu-id="368bc-126">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="368bc-126">To learn more, see [styling components](../style.md).</span></span>

## <a name="events"></a><span data-ttu-id="368bc-127">События</span><span class="sxs-lookup"><span data-stu-id="368bc-127">Events</span></span>

<span data-ttu-id="368bc-128">Из элемента управления запускаются следующие события.</span><span class="sxs-lookup"><span data-stu-id="368bc-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="368bc-129">Событие</span><span class="sxs-lookup"><span data-stu-id="368bc-129">Event</span></span> | <span data-ttu-id="368bc-130">Описание</span><span class="sxs-lookup"><span data-stu-id="368bc-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="368bc-131">Пользователь нажимает кнопку входа, чтобы запустить процесс входа в систему с отменой входа.</span><span class="sxs-lookup"><span data-stu-id="368bc-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="368bc-132">процесс входа выполнен успешно, и пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="368bc-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="368bc-133">Пользователь отменил процесс входа или не смог выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="368bc-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="368bc-134">Пользователь начал выход из системы и отменяется.</span><span class="sxs-lookup"><span data-stu-id="368bc-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="368bc-135">Пользователь вышел.</span><span class="sxs-lookup"><span data-stu-id="368bc-135">The user signed out.</span></span> |

## <a name="templates"></a><span data-ttu-id="368bc-136">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="368bc-136">Templates</span></span>

<span data-ttu-id="368bc-137">`mgt-login`Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="368bc-137">The `mgt-login` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="368bc-138">Чтобы указать шаблон, включите элемент в `<template>` компонент и задайте `data-type` для него одно из значений, приведенных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="368bc-138">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="368bc-139">Тип данных</span><span class="sxs-lookup"><span data-stu-id="368bc-139">Data type</span></span> | <span data-ttu-id="368bc-140">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="368bc-140">Data context</span></span> | <span data-ttu-id="368bc-141">Description</span><span class="sxs-lookup"><span data-stu-id="368bc-141">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="368bc-142">Вход — кнопка с содержимым</span><span class="sxs-lookup"><span data-stu-id="368bc-142">signed-in-button-content</span></span> | <span data-ttu-id="368bc-143">Персондетаилс: объект Person `personImage` : строка изображения пользователя</span><span class="sxs-lookup"><span data-stu-id="368bc-143">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="368bc-144">Шаблон, используемый для отображения содержимого кнопки при входе пользователя.</span><span class="sxs-lookup"><span data-stu-id="368bc-144">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="368bc-145">"с выходом" — кнопка — контент</span><span class="sxs-lookup"><span data-stu-id="368bc-145">signed-out-button-content</span></span> | <span data-ttu-id="368bc-146">пусто</span><span class="sxs-lookup"><span data-stu-id="368bc-146">null</span></span> | <span data-ttu-id="368bc-147">Шаблон, используемый для отображения содержимого кнопки, когда пользователь не выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="368bc-147">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="368bc-148">всплывающие команды</span><span class="sxs-lookup"><span data-stu-id="368bc-148">flyout-commands</span></span> | <span data-ttu-id="368bc-149">Хандлесигнаут: функция выхода</span><span class="sxs-lookup"><span data-stu-id="368bc-149">handleSignOut: sign out function</span></span> | <span data-ttu-id="368bc-150">Шаблон, используемый для отображения команд в меню</span><span class="sxs-lookup"><span data-stu-id="368bc-150">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="368bc-151">раскрывающееся меню — Person — сведения</span><span class="sxs-lookup"><span data-stu-id="368bc-151">flyout-person-details</span></span> | <span data-ttu-id="368bc-152">Персондетаилс: объект Person, Персонимаже: строка изображения пользователя</span><span class="sxs-lookup"><span data-stu-id="368bc-152">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="368bc-153">Шаблон, используемый для отображения сведений о лице в всплывающем меню.</span><span class="sxs-lookup"><span data-stu-id="368bc-153">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="368bc-154">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="368bc-154">Microsoft Graph permissions</span></span>

<span data-ttu-id="368bc-155">Этот компонент использует [компонент Person](./person.md) для отображения пользователя и наследования всех разрешений.</span><span class="sxs-lookup"><span data-stu-id="368bc-155">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="368bc-156">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="368bc-156">Authentication</span></span>

<span data-ttu-id="368bc-157">Элемент управления входом использует глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="368bc-157">The login control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 

## <a name="extend-for-more-control"></a><span data-ttu-id="368bc-158">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="368bc-158">Extend for more control</span></span>

<span data-ttu-id="368bc-159">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет несколько `protected render*` способов переопределения в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="368bc-159">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="368bc-160">Метод</span><span class="sxs-lookup"><span data-stu-id="368bc-160">Method</span></span> | <span data-ttu-id="368bc-161">Описание</span><span class="sxs-lookup"><span data-stu-id="368bc-161">Description</span></span> |
| - | - |
| <span data-ttu-id="368bc-162">рендербуттон</span><span class="sxs-lookup"><span data-stu-id="368bc-162">renderButton</span></span> | <span data-ttu-id="368bc-163">Отрисовывает хром кнопки.</span><span class="sxs-lookup"><span data-stu-id="368bc-163">Renders the button chrome.</span></span> |
| <span data-ttu-id="368bc-164">рендербуттонконтент</span><span class="sxs-lookup"><span data-stu-id="368bc-164">renderButtonContent</span></span> | <span data-ttu-id="368bc-165">Отрисовывает содержимое кнопки.</span><span class="sxs-lookup"><span data-stu-id="368bc-165">Renders the button content.</span></span> |
| <span data-ttu-id="368bc-166">рендерсигнединбуттонконтент</span><span class="sxs-lookup"><span data-stu-id="368bc-166">renderSignedInButtonContent</span></span> | <span data-ttu-id="368bc-167">Отображение содержимого кнопки, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="368bc-167">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="368bc-168">рендерсигнедаутбуттонконтент</span><span class="sxs-lookup"><span data-stu-id="368bc-168">renderSignedOutButtonContent</span></span> | <span data-ttu-id="368bc-169">Отображение содержимого кнопки, когда пользователь не выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="368bc-169">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="368bc-170">рендерфлйоут</span><span class="sxs-lookup"><span data-stu-id="368bc-170">renderFlyout</span></span> | <span data-ttu-id="368bc-171">Отрисовывает всплывающий хром.</span><span class="sxs-lookup"><span data-stu-id="368bc-171">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="368bc-172">рендерфлйоутконтент</span><span class="sxs-lookup"><span data-stu-id="368bc-172">renderFlyoutContent</span></span> | <span data-ttu-id="368bc-173">Отрисовывает содержимое всплывающего меню.</span><span class="sxs-lookup"><span data-stu-id="368bc-173">Renders the flyout content.</span></span> |
| <span data-ttu-id="368bc-174">рендерфлйоутперсондетаилс</span><span class="sxs-lookup"><span data-stu-id="368bc-174">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="368bc-175">Отображение сведений о пользователе всплывающего меню.</span><span class="sxs-lookup"><span data-stu-id="368bc-175">Render the flyout person details.</span></span> |
| <span data-ttu-id="368bc-176">рендерфлйоуткоммандс</span><span class="sxs-lookup"><span data-stu-id="368bc-176">renderFlyoutCommands</span></span> | <span data-ttu-id="368bc-177">Отображение команд всплывающего меню.</span><span class="sxs-lookup"><span data-stu-id="368bc-177">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="368bc-178">Перенесите собственное всплывающее окно</span><span class="sxs-lookup"><span data-stu-id="368bc-178">Bring your own flyout</span></span>

<span data-ttu-id="368bc-179">Можно использовать собственный компонент всплывающего окна вместо встроенного, переопределив `renderFlyout()` метод и указав новое всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="368bc-179">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="368bc-180">В этом случае убедитесь, что компонент входа продолжает работать должным образом, переопределяя `protected` методы всплывающего отображения, чтобы обновить видимость альтернативного всплывающего меню.</span><span class="sxs-lookup"><span data-stu-id="368bc-180">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="368bc-181">Метод</span><span class="sxs-lookup"><span data-stu-id="368bc-181">Method</span></span> | <span data-ttu-id="368bc-182">Описание</span><span class="sxs-lookup"><span data-stu-id="368bc-182">Description</span></span> |
| - | - |
| <span data-ttu-id="368bc-183">хидефлйоут</span><span class="sxs-lookup"><span data-stu-id="368bc-183">hideFlyout</span></span> | <span data-ttu-id="368bc-184">Закрывает всплывающее окно.</span><span class="sxs-lookup"><span data-stu-id="368bc-184">Dismisses the flyout.</span></span> |
| <span data-ttu-id="368bc-185">шовфлйоут</span><span class="sxs-lookup"><span data-stu-id="368bc-185">showFlyout</span></span> | <span data-ttu-id="368bc-186">Отображает всплывающее меню.</span><span class="sxs-lookup"><span data-stu-id="368bc-186">Displays the flyout.</span></span> |
| <span data-ttu-id="368bc-187">тогглефлйоут</span><span class="sxs-lookup"><span data-stu-id="368bc-187">toggleFlyout</span></span> | <span data-ttu-id="368bc-188">Переключает состояние всплывающего меню.</span><span class="sxs-lookup"><span data-stu-id="368bc-188">Toggles the state of the flyout.</span></span> |
