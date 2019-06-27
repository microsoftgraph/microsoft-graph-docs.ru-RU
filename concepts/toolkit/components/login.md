---
title: Компонент входа в набор средств Microsoft Graph
description: Компонент входа — это кнопка и всплывающий элемент управления для упрощения проверки подлинности на платформе Microsoft Identity.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e7c657b3b6c9772b2d7b7b8e64a57c9982f4caef
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243084"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="ec074-103">Компонент входа в набор средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ec074-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="ec074-104">Компонент входа — это кнопка и всплывающий элемент управления для упрощения проверки подлинности на платформе Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="ec074-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="ec074-105">Он предоставляет два состояния:</span><span class="sxs-lookup"><span data-stu-id="ec074-105">It provides two states:</span></span>
* <span data-ttu-id="ec074-106">Если пользователь не вошел в систему, элемент управления является простой кнопкой для запуска процесса входа.</span><span class="sxs-lookup"><span data-stu-id="ec074-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="ec074-107">Когда пользователь вошел в систему, элемент управления отображает имя пользователя, изображение профиля и адрес электронной почты, которые вошли в систему.</span><span class="sxs-lookup"><span data-stu-id="ec074-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="ec074-108">При нажатии открывается раскрывающееся меню с командой для выхода.</span><span class="sxs-lookup"><span data-stu-id="ec074-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="ec074-109">Пример</span><span class="sxs-lookup"><span data-stu-id="ec074-109">Example</span></span>

[<span data-ttu-id="ec074-110">Пример жсфиддле</span><span class="sxs-lookup"><span data-stu-id="ec074-110">jsfiddle example</span></span>](https://jsfiddle.net/metulev/scb9muh4)

```html
<mgt-login></mgt-login>
```

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="ec074-111">Использование элемента управления без поставщика проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="ec074-111">Using the control without an authentication provider</span></span>

<span data-ttu-id="ec074-112">Компонент работает с поставщиком и Microsoft Graph из этого ящика.</span><span class="sxs-lookup"><span data-stu-id="ec074-112">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="ec074-113">Тем не менее, если вы хотите предоставить собственную логику и проверку подлинности, `userDetails` вы можете использовать свойство, чтобы задать сведения о пользователе, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="ec074-113">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="ec074-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec074-114">Property</span></span> | <span data-ttu-id="ec074-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="ec074-115">Attribute</span></span> | <span data-ttu-id="ec074-116">Описание</span><span class="sxs-lookup"><span data-stu-id="ec074-116">Description</span></span> |
| --- | --- | -- |
| `userDetails` | `user-details` | <span data-ttu-id="ec074-117">Задайте объект пользователя, который будет отображаться в элементе управления.</span><span class="sxs-lookup"><span data-stu-id="ec074-117">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="ec074-118">В приведенном ниже примере задаются сведения о лице.</span><span class="sxs-lookup"><span data-stu-id="ec074-118">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    email: 'nikola@contoso.com',
    profileImage: 'url'
}
```

<span data-ttu-id="ec074-119">Для `userDetails` `null` параметра значение будет указано состояние "выход выполнен".</span><span class="sxs-lookup"><span data-stu-id="ec074-119">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="ec074-120">Используйте события `loginInitiated` и `logoutInitiated` для обработки входа и выхода из нее.</span><span class="sxs-lookup"><span data-stu-id="ec074-120">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="ec074-121">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="ec074-121">CSS custom properties</span></span>

<span data-ttu-id="ec074-122">`mgt-login` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="ec074-122">The `mgt-login` component defines the following CSS custom properties.</span></span>

```css
mgt-login {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --margin: 0;
  --padding: 12px 20px;
  --color: #201f1e;
  --background-color: transparent;
  --background-color--hover: #edebe9;
  --popup-content-background-color: white;
  --popup-command-font-size: 12px; }
}
```

<span data-ttu-id="ec074-123">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="ec074-123">To learn more, see [styling components](../style.md).</span></span>

## <a name="events"></a><span data-ttu-id="ec074-124">События</span><span class="sxs-lookup"><span data-stu-id="ec074-124">Events</span></span>

<span data-ttu-id="ec074-125">Из элемента управления запускаются следующие события.</span><span class="sxs-lookup"><span data-stu-id="ec074-125">The following events are fired from the control.</span></span>

| <span data-ttu-id="ec074-126">Событие</span><span class="sxs-lookup"><span data-stu-id="ec074-126">Event</span></span> | <span data-ttu-id="ec074-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ec074-127">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="ec074-128">Пользователь нажимает кнопку входа, чтобы запустить процесс входа в систему с отменой входа.</span><span class="sxs-lookup"><span data-stu-id="ec074-128">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="ec074-129">процесс входа выполнен успешно, и пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="ec074-129">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="ec074-130">Пользователь отменил процесс входа или не смог выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="ec074-130">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="ec074-131">Пользователь начал выход из системы и отменяется.</span><span class="sxs-lookup"><span data-stu-id="ec074-131">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="ec074-132">Пользователь вышел.</span><span class="sxs-lookup"><span data-stu-id="ec074-132">The user signed out.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="ec074-133">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ec074-133">Microsoft Graph permissions</span></span>

<span data-ttu-id="ec074-134">Этот компонент использует [компонент Person](./person.md) для отображения пользователя и наследования всех разрешений.</span><span class="sxs-lookup"><span data-stu-id="ec074-134">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="ec074-135">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="ec074-135">Authentication</span></span>

<span data-ttu-id="ec074-136">Элемент управления входом использует глобальный поставщик проверки подлинности, описанный в [документации по проверке](./../providers.md)подлинности.</span><span class="sxs-lookup"><span data-stu-id="ec074-136">The login control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
