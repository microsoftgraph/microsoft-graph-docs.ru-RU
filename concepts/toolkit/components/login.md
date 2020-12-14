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
# <a name="login-component-in-the-microsoft-graph-toolkit"></a>Компонент входа в microsoft Graph набор средств

Компонент входа — это элемент управления кнопкой и flyout для упрощения проверки подлинности платформы удостоверений Майкрософт. Он предоставляет два состояния:
* Если пользователь не входил в учетную запись, он является простой кнопкой для запуска процесса.
* Когда пользователь вписается, в этом контрольном оке отображается текущее имя пользователя, изображение профиля и электронная почта. При нажатии на них открывается флажок с командой для выйдите из нее.

## <a name="example"></a>Пример

В следующем примере показан `mgt-login` компонент с во выписаным пользователем. 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[Откройте этот пример в mgt.dev](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a>Использование управления без поставщика проверки подлинности

Компонент работает с поставщиком и Microsoft Graph. Однако если вы хотите предоставить собственную логику и проверку подлинности, вы можете использовать это свойство, чтобы установить сведения о `userDetails` вописаемом пользователе. 

| Атрибут | Свойство | Описание |
| --- | --- | -- |
| user-details | userDetails | Установите объект пользователя, который будет отображаться на этом объекте управления. |

В следующем примере устанавливаются сведения о человеке.

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

Параметр `userDetails` будет `null` переходить в состояние выходных.

Используйте события `loginInitiated` и `logoutInitiated` события для обработки входов и выходов. 

## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

Компонент `mgt-login` определяет следующие настраиваемые свойства CSS.

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

Дополнительные узнать см. [в компонентах стиля.](../customize-components/style.md)

## <a name="events"></a>События

Из этого управления и происходят следующие события.

| Событие | Описание |
| --- | --- |
| `loginInitiated` | Пользователь нажал кнопку входа, чтобы запустить процесс входа — отмена.|
| `loginCompleted` | процесс входа был успешным, и теперь пользователь в систему входить. |
| `loginFailed` | Пользователь отменил процесс входа или не смог войти.|
| `logoutInitiated` | Пользователь начал выходить из сети — отменяется. |
| `logoutCompleted` | Пользователь вышел из сети. |

## <a name="templates"></a>Шаблоны

Компонент `mgt-login` поддерживает несколько [шаблонов,](../customize-components/templates.md) которые позволяют заменить определенные части компонента. Чтобы указать шаблон, включив элемент в компонент и заключив в него одно из значений, перечисленных `<template>` `data-type` в следующей таблице. 

| Тип данных | Контекст данных | Описание |
| --- | --- | --- |
| signed-in-button-content | personDetails: объект person, `personImage` : строка изображения человека | Шаблон, используемый для отрисовки содержимого в кнопке при пользователе. |
| signed-out-button-content | null | Шаблон, используемый для отображения содержимого кнопки, когда пользователь не вписались. |
| flyout-commands | handleSignOut: функция выход | Шаблон, используемый для отображения команд во flyout |
| flyout-person-details | personDetails: объект person, personImage: строка изображения человека | Шаблон, используемый для отображения сведений о человеке во flyout. |

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот компонент использует компонент [Person для](./person.md) отображения пользователя и наследует все разрешения. 

## <a name="authentication"></a>Проверка подлинности

Для управления входом используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности.](../providers/providers.md) 

## <a name="extend-for-more-control"></a>Расширение для большего контроля

Для более сложных сценариев или по-настоящему настраиваемого пользовательского пользовательского управления этот компонент предоставляет несколько методов для переопределения `protected render*` в расширениях компонентов.

| Метод | Описание |
| - | - |
| renderButton | Отрисовка хрома кнопки. |
| renderButtonContent | Отрисовка содержимого кнопки. |
| renderSignedInButtonContent | Отрисовка содержимого кнопки при вписи пользователя. |
| renderSignedOutButtonContent | Отрисовка содержимого кнопки, когда пользователь не вписались. |
| renderFlyout | Отрисовка хрома во весь экран. |
| renderFlyoutContent | Отрисовка содержимого flyout. |
| renderFlyoutPersonDetails | Отрисовка сведений о выявимом человеке. |
| renderFlyoutCommands | Отрисовка команд flyout. |

### <a name="bring-your-own-flyout"></a>Принеси свой собственный flyout

Можно использовать собственный компонент flyout, а не встроенный, переопределив метод и предоставив `renderFlyout()` новый элемент.

В этом случае убедитесь, что компонент входа продолжает работать ожидаемым образом, переопределив методы отображения элементов для обновления видимости альтернативного `protected` flyout.

| Метод | Описание |
| - | - |
| hideFlyout | Отклоняться от flyout. |
| showFlyout | Отображает flyout. |
| toggleFlyout | Перетагрегает состояние flyout. |
