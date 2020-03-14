---
title: Компонент входа в набор средств Microsoft Graph
description: Компонент входа — это кнопка и всплывающий элемент управления для упрощения проверки подлинности на платформе Microsoft Identity.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 3b326cc97bf7a3463e43ffcf757cc34d5cc00975
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639984"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="23216-103">Компонент входа в набор средств Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="23216-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="23216-104">Компонент входа — это кнопка и всплывающий элемент управления для упрощения проверки подлинности на платформе Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="23216-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="23216-105">Он предоставляет два состояния:</span><span class="sxs-lookup"><span data-stu-id="23216-105">It provides two states:</span></span>
* <span data-ttu-id="23216-106">Если пользователь не вошел в систему, элемент управления является простой кнопкой для запуска процесса входа.</span><span class="sxs-lookup"><span data-stu-id="23216-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="23216-107">Когда пользователь вошел в систему, элемент управления отображает имя пользователя, изображение профиля и адрес электронной почты, которые вошли в систему.</span><span class="sxs-lookup"><span data-stu-id="23216-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="23216-108">При нажатии открывается раскрывающееся меню с командой для выхода.</span><span class="sxs-lookup"><span data-stu-id="23216-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="23216-109">Пример</span><span class="sxs-lookup"><span data-stu-id="23216-109">Example</span></span>

<span data-ttu-id="23216-110">В следующем примере показан `mgt-login` компонент с пользователь, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="23216-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="23216-111">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="23216-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="23216-112">Использование элемента управления без поставщика проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="23216-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="23216-113">Компонент работает с поставщиком и Microsoft Graph из этого ящика.</span><span class="sxs-lookup"><span data-stu-id="23216-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="23216-114">Тем не менее, если вы хотите предоставить собственную логику и проверку подлинности, `userDetails` вы можете использовать свойство, чтобы задать сведения о пользователе, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="23216-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="23216-115">Атрибут</span><span class="sxs-lookup"><span data-stu-id="23216-115">Attribute</span></span> | <span data-ttu-id="23216-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="23216-116">Property</span></span> | <span data-ttu-id="23216-117">Описание</span><span class="sxs-lookup"><span data-stu-id="23216-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="23216-118">пользователь — сведения</span><span class="sxs-lookup"><span data-stu-id="23216-118">user-details</span></span> | <span data-ttu-id="23216-119">усердетаилс</span><span class="sxs-lookup"><span data-stu-id="23216-119">userDetails</span></span> | <span data-ttu-id="23216-120">Задайте объект пользователя, который будет отображаться в элементе управления.</span><span class="sxs-lookup"><span data-stu-id="23216-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="23216-121">В приведенном ниже примере задаются сведения о лице.</span><span class="sxs-lookup"><span data-stu-id="23216-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    email: 'nikola@contoso.com',
    profileImage: 'url'
}
```

<span data-ttu-id="23216-122">Для `userDetails` `null` параметра значение будет указано состояние "выход выполнен".</span><span class="sxs-lookup"><span data-stu-id="23216-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="23216-123">Используйте события `loginInitiated` и `logoutInitiated` для обработки входа и выхода из нее.</span><span class="sxs-lookup"><span data-stu-id="23216-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="23216-124">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="23216-124">CSS custom properties</span></span>

<span data-ttu-id="23216-125">`mgt-login` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="23216-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="23216-126">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="23216-126">To learn more, see [styling components](../style.md).</span></span>

## <a name="events"></a><span data-ttu-id="23216-127">События</span><span class="sxs-lookup"><span data-stu-id="23216-127">Events</span></span>

<span data-ttu-id="23216-128">Из элемента управления запускаются следующие события.</span><span class="sxs-lookup"><span data-stu-id="23216-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="23216-129">Событие</span><span class="sxs-lookup"><span data-stu-id="23216-129">Event</span></span> | <span data-ttu-id="23216-130">Описание</span><span class="sxs-lookup"><span data-stu-id="23216-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="23216-131">Пользователь нажимает кнопку входа, чтобы запустить процесс входа в систему с отменой входа.</span><span class="sxs-lookup"><span data-stu-id="23216-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="23216-132">процесс входа выполнен успешно, и пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="23216-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="23216-133">Пользователь отменил процесс входа или не смог выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="23216-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="23216-134">Пользователь начал выход из системы и отменяется.</span><span class="sxs-lookup"><span data-stu-id="23216-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="23216-135">Пользователь вышел.</span><span class="sxs-lookup"><span data-stu-id="23216-135">The user signed out.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="23216-136">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="23216-136">Microsoft Graph permissions</span></span>

<span data-ttu-id="23216-137">Этот компонент использует [компонент Person](./person.md) для отображения пользователя и наследования всех разрешений.</span><span class="sxs-lookup"><span data-stu-id="23216-137">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="23216-138">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="23216-138">Authentication</span></span>

<span data-ttu-id="23216-139">Элемент управления входом использует глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="23216-139">The login control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
