---
title: 'Набор средств Microsoft Graph: веб-компоненты на платформе Microsoft Graph'
description: Набор инструментов Microsoft Graph представляет собой набор ресуабле, независимых от платформы веб-компонентов и вспомогательных средств для доступа к Microsoft Graph и работы с ним.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: ba19e1697700800de22d193f8bbb1a959776a18f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036865"
---
# <a name="microsoft-graph-toolkit-web-components-powered-by-microsoft-graph"></a>Набор средств Microsoft Graph: веб-компоненты на платформе Microsoft Graph

Набор инструментов Microsoft Graph представляет собой набор компонентов и вспомогательных программ для доступа к Microsoft Graph, не зависящего от платформы. Компоненты полностью функционируют прямо из этого поля со встроенными поставщиками, которые проходят проверку подлинности и извлекают данные из Microsoft Graph.

Набор средств Microsoft Graph позволяет легко использовать Microsoft Graph в приложении. В приведенном ниже примере показано, как пользователи, вошедшего в систему, и их события календаря отображаются только с двумя строками кода, используя компоненты [входа](./components/login.md) и [повестки](./components/agenda.md) .

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[Откройте этот пример в меню упр. dev.](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a>Что входит в набор средств Microsoft Graph?

### <a name="components"></a>Компоненты

Набор средств Microsoft Graph включает в себя набор веб-компонентов для наиболее часто создаваемых интерфейсов API Microsoft Graph.

|Компонент|Описание|
|---------|-----------|
|[Вход](./components/login.md)|Кнопка и всплывающий элемент управления для проверки подлинности пользователя с платформой Microsoft Identity и отображения сведений о профиле пользователя при входе.|
|[Пользователь](./components/person.md)|Отображает пользователя или контакт по фотографии, названию и/или адресу электронной почты.|
|[Люди](./components/people.md)|Отображает группу людей или контактов по их фотографиям или инициалам.|
|[Повестка](./components/agenda.md)|Отображает события в календаре пользователя или группы.|
|[Задачи](./components/tasks.md)|Показывает и разрешает добавлять, удалять, завершать или изменять задачи из планировщика (Майкрософт) или задачи Майкрософт.|
|[Средство выбора людей](./components/people-picker.md)|Предоставляет возможность поиска людей и отображения списка результатов.|
|[Карточка лица](./components/person-card.md)|Раскрывающееся меню, используемое компонентом Person для отображения дополнительных сведений о профиле пользователя.|
|[получение](./components/get.md);|Сделайте запрос GET к любому API Microsoft Graph непосредственно в HTML-коде.|
|[Выбор канала](./components/teams-channel-picker.md)|Обеспечивает возможность поиска каналов Microsoft Teams для выбора канала из подготовленного списка результатов.|

### <a name="providers"></a>Поставщики

Компоненты лучше всего подходят для использования с [поставщиками](/providers/providers.md). Поставщики обеспечивают проверку подлинности и предоставляют реализацию для получения маркеров доступа для вызова API Microsoft Graph.

|Поставщики|Описание|
|---------|-----------|
|[Msal](./providers/msal.md)|Использует MSAL.js для входа пользователей и получения маркеров для использования с Microsoft Graph.|
|[SharePoint](./providers/sharepoint.md)|Проверяет подлинность и предоставляет Microsoft Graph доступ к компонентам в веб-частях SharePoint.|
|[Teams](./providers/teams.md)|Проверка подлинности и предоставление доступа Microsoft Graph к компонентам внутри вкладок Microsoft Teams.|
|[Сервера](./providers/proxy.md)|Позволяет использовать внутреннюю проверку подлинности путем маршрутизации всех вызовов Microsoft Graph через серверный сервер.|
|[Пользовательский](./providers/custom.md)|Создайте настраиваемый поставщик, чтобы включить проверку подлинности и доступ к Microsoft Graph с помощью существующего кода проверки подлинности приложения.|

## <a name="why-use-the-microsoft-graph-toolkit"></a>Зачем использовать набор средств Microsoft Graph?

Набор средств Microsoft Graph позволяет быстро и легко интегрировать общедоступные возможности Microsoft Graph в свое приложение.

:::row:::
   :::column span="":::
    **Сокращение времени разработки**

    Работа по подключению к API Microsoft Graph и визуализация данных в пользовательском интерфейсе, которая выглядит так же, как Microsoft365, выполняется без необходимости настройки.
  :::column-end:::
  :::column span="":::
    **Работает везде**

    Все компоненты основываются на веб-стандартах и тесно работают с любым современным браузером и веб-средой (реагируем, радиально, Vue и т. д.). 
  :::column-end:::
  :::column span="":::
    **Прекрасная, но гибкая**

    Компоненты предназначены для внешнего вида и работы с Microsoft365, но также могут настраиваться с помощью [настраиваемых свойств CSS](./style.md) и [шаблонов](./templates.md).
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a>Кто должен использовать его?

Набор средств Microsoft Graph прекрасно подходит разработчикам всех уровней опыта разработки веб-приложения, вкладки Microsoft Teams или веб-части SharePoint, которые подключаются к данным из Microsoft Graph и обращаются к ним.

## <a name="where-can-i-use-it"></a>Где можно использовать его?

Набор средств Microsoft Graph поддерживается в следующих браузерах.

|![Microsoft Edge](images/edgeIcon.png)|![Internet Explorer 11](images/internetExplorerIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|**Microsoft Edge**|**IE 11**|**Firefox**|**Chrome**|**Safari**|**Opera**|**Samsung**|

## <a name="next-steps"></a>Следующие шаги

- Опробуйте компоненты в [интерактивная среда](https://mgt.dev).
- Приступите к [работе](./get-started/overview.md) с набором инструментов Microsoft Graph.
- Ознакомьтесь со статьей Microsoft Graph Toolkit на сайте [GitHub](https://aka.ms/mgt).
