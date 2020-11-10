---
title: Начало работы с набором средств Microsoft Graph
description: Приступите к работе с набором инструментов Microsoft Graph в приложении.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e3739bb6180e19569ae40e873d3a018bbb541833
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977137"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Начало работы с набором средств Microsoft Graph

Компоненты набора инструментов Microsoft Graph легко можно добавить в веб-приложение, веб-часть SharePoint или вкладки Microsoft Teams. Компоненты основываются на веб-стандартах и могут использоваться как в простых проектах JavaScript, так и на популярных веб-платформах, таких как REACH, угловой, Vue.js и многое другое.

Вы можете посмотреть это короткое видео, чтобы узнать, как быстро и легко начать работу с набором средств.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

## <a name="set-up-your-microsoft-365-tenant"></a>Настройка клиента Microsoft 365
Для разработки с помощью набора инструментов вам необходим доступ к клиенту Microsoft 365. Если у вас его нет, вы можете получить бесплатную подписку на Microsoft 365 для разработчиков, [присоединяясь к программе для разработчиков microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program). Сведения о том, как настроить подписку, можно найти [в разделе Настройка подписки на Microsoft 365 для разработчиков](/office/developer-program/microsoft-365-developer-program-get-started).

## <a name="set-up-your-development-environment"></a>Настройка среды разработки
Для разработки с помощью набора инструментов вам потребуется текстовый редактор или IDE. Вы можете использовать нужный редактор или IDE или установить и использовать [Visual Studio Code](https://code.visualstudio.com/download) бесплатно. Кроме того, вам потребуется современный веб-браузер, например Microsoft EDGE, Google Chrome или Firefox. Кроме того, вам потребуется LTS версия Node.js, которую можно установить из [NodeJS.org](https://nodejs.org).

## <a name="using-the-microsoft-graph-toolkit"></a>Использование набора средств Microsoft Graph
Вы можете использовать набор средств Microsoft Graph в приложении, обратившись непосредственно к загрузчику (через унпкг) или установив пакет NPM.

### <a name="use-via-mgt-loader"></a>Использование с помощью упр. загрузчиком
Чтобы использовать набор средств с помощью элемента управления "центр управления", добавьте ссылку в скрипт в код:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>Использование через NPM (модули ES6)
Использование набора средств с помощью модулей ES6 даст вам полный контроль над процессом создания пучка и позволяет объединить только код, который требуется для приложения. Чтобы использовать модули ES6, добавьте в проект пакет NPM:

```bash
npm install @microsoft/mgt
```
Теперь вы можете ссылаться на все компоненты на странице, которые вы используете:

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

Или просто сделайте ссылку на необходимый компонент и не загружаете все остальные:
```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

#### <a name="polyfills"></a>Polyfills

Если вы используете модули ES6 из пакета NPM и используете [браузер, например IE11](https://caniuse.com/#search=components) , который не поддерживает встроенные веб-компоненты, необходимо включить в проект только те, которые не включены автоматически. С помощью заполнения в браузерах можно заполнять отсутствующие возможности браузера в браузерах, которые по-прежнему находятся в процессе обновления для поддержки стандартов Вебккомпонент. Инструкции и дополнительные сведения [см.](https://www.webcomponents.org/polyfills) 

При использовании набора инструментов с помощью скрипта управления, в котором используется набор средств.

## <a name="next-steps"></a>Дальнейшие действия
Теперь вы готовы приступить к разработке с помощью набора инструментов Microsoft Graph! Ниже приведены руководства, которые помогут вам приступить к работе.

- [Создание приложения Azure Active Directory](./add-aad-app-registration.md)
- [Создание веб-приложения](./build-a-web-app.md) (Ванилла JavaScript)
- [Создание веб-части SharePoint](./build-a-sharepoint-web-part.md)
- [Создание вкладки Microsoft Teams](./build-a-microsoft-teams-tab.md)
- [Использование набора инструментов с откликом](./use-toolkit-with-react.md)
- [Использование набора инструментов с угловой](./use-toolkit-with-angular.md)
