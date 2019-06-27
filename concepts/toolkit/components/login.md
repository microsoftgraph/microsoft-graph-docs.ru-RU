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
# <a name="login-component-in-the-microsoft-graph-toolkit"></a>Компонент входа в набор средств Microsoft Graph

Компонент входа — это кнопка и всплывающий элемент управления для упрощения проверки подлинности на платформе Microsoft Identity. Он предоставляет два состояния:
* Если пользователь не вошел в систему, элемент управления является простой кнопкой для запуска процесса входа.
* Когда пользователь вошел в систему, элемент управления отображает имя пользователя, изображение профиля и адрес электронной почты, которые вошли в систему. При нажатии открывается раскрывающееся меню с командой для выхода.

## <a name="example"></a>Пример

[Пример жсфиддле](https://jsfiddle.net/metulev/scb9muh4)

```html
<mgt-login></mgt-login>
```

## <a name="using-the-control-without-an-authentication-provider"></a>Использование элемента управления без поставщика проверки подлинности

Компонент работает с поставщиком и Microsoft Graph из этого ящика. Тем не менее, если вы хотите предоставить собственную логику и проверку подлинности, `userDetails` вы можете использовать свойство, чтобы задать сведения о пользователе, выполнившего вход в систему. 

| Свойство | Атрибут | Описание |
| --- | --- | -- |
| `userDetails` | `user-details` | Задайте объект пользователя, который будет отображаться в элементе управления. |

В приведенном ниже примере задаются сведения о лице.

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    email: 'nikola@contoso.com',
    profileImage: 'url'
}
```

Для `userDetails` `null` параметра значение будет указано состояние "выход выполнен".

Используйте события `loginInitiated` и `logoutInitiated` для обработки входа и выхода из нее. 

## <a name="css-custom-properties"></a>Настраиваемые свойства CSS

`mgt-login` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.

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

Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).

## <a name="events"></a>События

Из элемента управления запускаются следующие события.

| Событие | Описание |
| --- | --- |
| `loginInitiated` | Пользователь нажимает кнопку входа, чтобы запустить процесс входа в систему с отменой входа.|
| `loginCompleted` | процесс входа выполнен успешно, и пользователь вошел в систему. |
| `loginFailed` | Пользователь отменил процесс входа или не смог выполнить вход.|
| `logoutInitiated` | Пользователь начал выход из системы и отменяется. |
| `logoutCompleted` | Пользователь вышел. |

## <a name="microsoft-graph-permissions"></a>Разрешения Microsoft Graph

Этот компонент использует [компонент Person](./person.md) для отображения пользователя и наследования всех разрешений. 

## <a name="authentication"></a>Проверка подлинности

Элемент управления входом использует глобальный поставщик проверки подлинности, описанный в [документации по проверке](./../providers.md)подлинности. 
