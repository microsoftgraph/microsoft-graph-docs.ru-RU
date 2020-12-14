---
title: Компонент входа в microsoft Graph набор средств
description: Компонент входа — это элемент управления кнопкой и flyout для упрощения проверки подлинности платформы удостоверений Майкрософт.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: a54dfaede64216e8a2254aedb06cf6aa41aaa295
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660067"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="cb39f-103">Компонент входа в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="cb39f-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="cb39f-104">Компонент входа — это элемент управления кнопкой и flyout для упрощения проверки подлинности платформы удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="cb39f-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="cb39f-105">Он предоставляет два состояния:</span><span class="sxs-lookup"><span data-stu-id="cb39f-105">It provides two states:</span></span>
* <span data-ttu-id="cb39f-106">Если пользователь не входил в учетную запись, он является простой кнопкой для запуска процесса.</span><span class="sxs-lookup"><span data-stu-id="cb39f-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="cb39f-107">Когда пользователь вписается, в этом контрольном оке отображается текущее имя пользователя, изображение профиля и электронная почта.</span><span class="sxs-lookup"><span data-stu-id="cb39f-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="cb39f-108">При нажатии на них открывается флажок с командой для выйдите из нее.</span><span class="sxs-lookup"><span data-stu-id="cb39f-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="cb39f-109">Пример</span><span class="sxs-lookup"><span data-stu-id="cb39f-109">Example</span></span>

<span data-ttu-id="cb39f-110">В следующем примере показан `mgt-login` компонент с во выписаным пользователем.</span><span class="sxs-lookup"><span data-stu-id="cb39f-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="cb39f-111">Откройте этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="cb39f-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="cb39f-112">Использование управления без поставщика проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="cb39f-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="cb39f-113">Компонент работает с поставщиком и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cb39f-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="cb39f-114">Однако если вы хотите предоставить собственную логику и проверку подлинности, вы можете использовать это свойство, чтобы установить сведения о `userDetails` вописаемом пользователе.</span><span class="sxs-lookup"><span data-stu-id="cb39f-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="cb39f-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="cb39f-115">Attribute</span></span> | <span data-ttu-id="cb39f-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb39f-116">Property</span></span> | <span data-ttu-id="cb39f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="cb39f-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="cb39f-118">user-details</span><span class="sxs-lookup"><span data-stu-id="cb39f-118">user-details</span></span> | <span data-ttu-id="cb39f-119">userDetails</span><span class="sxs-lookup"><span data-stu-id="cb39f-119">userDetails</span></span> | <span data-ttu-id="cb39f-120">Установите объект пользователя, который будет отображаться на этом объекте управления.</span><span class="sxs-lookup"><span data-stu-id="cb39f-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="cb39f-121">В следующем примере устанавливаются сведения о человеке.</span><span class="sxs-lookup"><span data-stu-id="cb39f-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="cb39f-122">Параметр `userDetails` будет `null` переходить в состояние выходных.</span><span class="sxs-lookup"><span data-stu-id="cb39f-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="cb39f-123">Используйте события `loginInitiated` и `logoutInitiated` события для обработки входов и выходов.</span><span class="sxs-lookup"><span data-stu-id="cb39f-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="cb39f-124">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="cb39f-124">CSS custom properties</span></span>

<span data-ttu-id="cb39f-125">Компонент `mgt-login` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="cb39f-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="cb39f-126">Дополнительные узнать см. [в компонентах стиля.](../customize-components/style.md)</span><span class="sxs-lookup"><span data-stu-id="cb39f-126">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="cb39f-127">События</span><span class="sxs-lookup"><span data-stu-id="cb39f-127">Events</span></span>

<span data-ttu-id="cb39f-128">Из этого управления и происходят следующие события.</span><span class="sxs-lookup"><span data-stu-id="cb39f-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="cb39f-129">Событие</span><span class="sxs-lookup"><span data-stu-id="cb39f-129">Event</span></span> | <span data-ttu-id="cb39f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="cb39f-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="cb39f-131">Пользователь нажал кнопку входа, чтобы запустить процесс входа — отмена.</span><span class="sxs-lookup"><span data-stu-id="cb39f-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="cb39f-132">процесс входа был успешным, и теперь пользователь в систему входить.</span><span class="sxs-lookup"><span data-stu-id="cb39f-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="cb39f-133">Пользователь отменил процесс входа или не смог войти.</span><span class="sxs-lookup"><span data-stu-id="cb39f-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="cb39f-134">Пользователь начал выходить из сети — отменяется.</span><span class="sxs-lookup"><span data-stu-id="cb39f-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="cb39f-135">Пользователь вышел из сети.</span><span class="sxs-lookup"><span data-stu-id="cb39f-135">The user signed out.</span></span> |

## <a name="templates"></a><span data-ttu-id="cb39f-136">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="cb39f-136">Templates</span></span>

<span data-ttu-id="cb39f-137">Компонент `mgt-login` поддерживает несколько [шаблонов,](../customize-components/templates.md) которые позволяют заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="cb39f-137">The `mgt-login` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="cb39f-138">Чтобы указать шаблон, включив элемент в компонент и заключив в него одно из значений, перечисленных `<template>` `data-type` в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="cb39f-138">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="cb39f-139">Тип данных</span><span class="sxs-lookup"><span data-stu-id="cb39f-139">Data type</span></span> | <span data-ttu-id="cb39f-140">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="cb39f-140">Data context</span></span> | <span data-ttu-id="cb39f-141">Описание</span><span class="sxs-lookup"><span data-stu-id="cb39f-141">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="cb39f-142">signed-in-button-content</span><span class="sxs-lookup"><span data-stu-id="cb39f-142">signed-in-button-content</span></span> | <span data-ttu-id="cb39f-143">personDetails: объект person, `personImage` : строка изображения человека</span><span class="sxs-lookup"><span data-stu-id="cb39f-143">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="cb39f-144">Шаблон, используемый для отрисовки содержимого в кнопке при пользователе.</span><span class="sxs-lookup"><span data-stu-id="cb39f-144">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="cb39f-145">signed-out-button-content</span><span class="sxs-lookup"><span data-stu-id="cb39f-145">signed-out-button-content</span></span> | <span data-ttu-id="cb39f-146">null</span><span class="sxs-lookup"><span data-stu-id="cb39f-146">null</span></span> | <span data-ttu-id="cb39f-147">Шаблон, используемый для отображения содержимого кнопки, когда пользователь не вписались.</span><span class="sxs-lookup"><span data-stu-id="cb39f-147">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="cb39f-148">flyout-commands</span><span class="sxs-lookup"><span data-stu-id="cb39f-148">flyout-commands</span></span> | <span data-ttu-id="cb39f-149">handleSignOut: функция выход</span><span class="sxs-lookup"><span data-stu-id="cb39f-149">handleSignOut: sign out function</span></span> | <span data-ttu-id="cb39f-150">Шаблон, используемый для отображения команд во flyout</span><span class="sxs-lookup"><span data-stu-id="cb39f-150">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="cb39f-151">flyout-person-details</span><span class="sxs-lookup"><span data-stu-id="cb39f-151">flyout-person-details</span></span> | <span data-ttu-id="cb39f-152">personDetails: объект person, personImage: строка изображения человека</span><span class="sxs-lookup"><span data-stu-id="cb39f-152">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="cb39f-153">Шаблон, используемый для отображения сведений о человеке во flyout.</span><span class="sxs-lookup"><span data-stu-id="cb39f-153">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="cb39f-154">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cb39f-154">Microsoft Graph permissions</span></span>

<span data-ttu-id="cb39f-155">Этот компонент использует компонент [Person для](./person.md) отображения пользователя и наследует все разрешения.</span><span class="sxs-lookup"><span data-stu-id="cb39f-155">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="cb39f-156">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="cb39f-156">Authentication</span></span>

<span data-ttu-id="cb39f-157">Для управления входом используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="cb39f-157">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="extend-for-more-control"></a><span data-ttu-id="cb39f-158">Расширение для большего контроля</span><span class="sxs-lookup"><span data-stu-id="cb39f-158">Extend for more control</span></span>

<span data-ttu-id="cb39f-159">Для более сложных сценариев или по-настоящему настраиваемого пользовательского пользовательского управления этот компонент предоставляет несколько методов для переопределения `protected render*` в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="cb39f-159">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="cb39f-160">Метод</span><span class="sxs-lookup"><span data-stu-id="cb39f-160">Method</span></span> | <span data-ttu-id="cb39f-161">Описание</span><span class="sxs-lookup"><span data-stu-id="cb39f-161">Description</span></span> |
| - | - |
| <span data-ttu-id="cb39f-162">renderButton</span><span class="sxs-lookup"><span data-stu-id="cb39f-162">renderButton</span></span> | <span data-ttu-id="cb39f-163">Отрисовка хрома кнопки.</span><span class="sxs-lookup"><span data-stu-id="cb39f-163">Renders the button chrome.</span></span> |
| <span data-ttu-id="cb39f-164">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="cb39f-164">renderButtonContent</span></span> | <span data-ttu-id="cb39f-165">Отрисовка содержимого кнопки.</span><span class="sxs-lookup"><span data-stu-id="cb39f-165">Renders the button content.</span></span> |
| <span data-ttu-id="cb39f-166">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="cb39f-166">renderSignedInButtonContent</span></span> | <span data-ttu-id="cb39f-167">Отрисовка содержимого кнопки при вписи пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb39f-167">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="cb39f-168">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="cb39f-168">renderSignedOutButtonContent</span></span> | <span data-ttu-id="cb39f-169">Отрисовка содержимого кнопки, когда пользователь не вписались.</span><span class="sxs-lookup"><span data-stu-id="cb39f-169">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="cb39f-170">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="cb39f-170">renderFlyout</span></span> | <span data-ttu-id="cb39f-171">Отрисовка хрома во весь экран.</span><span class="sxs-lookup"><span data-stu-id="cb39f-171">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="cb39f-172">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="cb39f-172">renderFlyoutContent</span></span> | <span data-ttu-id="cb39f-173">Отрисовка содержимого flyout.</span><span class="sxs-lookup"><span data-stu-id="cb39f-173">Renders the flyout content.</span></span> |
| <span data-ttu-id="cb39f-174">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="cb39f-174">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="cb39f-175">Отрисовка сведений о выявимом человеке.</span><span class="sxs-lookup"><span data-stu-id="cb39f-175">Render the flyout person details.</span></span> |
| <span data-ttu-id="cb39f-176">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="cb39f-176">renderFlyoutCommands</span></span> | <span data-ttu-id="cb39f-177">Отрисовка команд flyout.</span><span class="sxs-lookup"><span data-stu-id="cb39f-177">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="cb39f-178">Принеси свой собственный flyout</span><span class="sxs-lookup"><span data-stu-id="cb39f-178">Bring your own flyout</span></span>

<span data-ttu-id="cb39f-179">Можно использовать собственный компонент flyout, а не встроенный, переопределив метод и предоставив `renderFlyout()` новый элемент.</span><span class="sxs-lookup"><span data-stu-id="cb39f-179">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="cb39f-180">В этом случае убедитесь, что компонент входа продолжает работать ожидаемым образом, переопределив методы отображения элементов для обновления видимости альтернативного `protected` flyout.</span><span class="sxs-lookup"><span data-stu-id="cb39f-180">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="cb39f-181">Метод</span><span class="sxs-lookup"><span data-stu-id="cb39f-181">Method</span></span> | <span data-ttu-id="cb39f-182">Описание</span><span class="sxs-lookup"><span data-stu-id="cb39f-182">Description</span></span> |
| - | - |
| <span data-ttu-id="cb39f-183">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="cb39f-183">hideFlyout</span></span> | <span data-ttu-id="cb39f-184">Отклоняться от flyout.</span><span class="sxs-lookup"><span data-stu-id="cb39f-184">Dismisses the flyout.</span></span> |
| <span data-ttu-id="cb39f-185">showFlyout</span><span class="sxs-lookup"><span data-stu-id="cb39f-185">showFlyout</span></span> | <span data-ttu-id="cb39f-186">Отображает flyout.</span><span class="sxs-lookup"><span data-stu-id="cb39f-186">Displays the flyout.</span></span> |
| <span data-ttu-id="cb39f-187">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="cb39f-187">toggleFlyout</span></span> | <span data-ttu-id="cb39f-188">Перетагрегает состояние flyout.</span><span class="sxs-lookup"><span data-stu-id="cb39f-188">Toggles the state of the flyout.</span></span> |
