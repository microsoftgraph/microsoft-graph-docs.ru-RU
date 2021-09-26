---
title: Используйте Graph Explorer, чтобы попробовать API Graph Microsoft
description: Используйте Graph Explorer, чтобы попробовать API microsoft Graph на примере клиента по умолчанию, чтобы изучить возможности, или войти в собственный клиент и использовать его в качестве средства создания образцов для выполнения сценариев приложений.
ms.localizationpriority: medium
author: bettirosengugi
ms.openlocfilehash: 14b16562c05b22000d299d3d2cd7dc608fa29293
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766980"
---
# <a name="use-graph-explorer-to-try-microsoft-graph-apis"></a>Используйте Graph Explorer, чтобы попробовать API Graph Microsoft

[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) — это средство разработчика, которое позволяет удобно создавать запросы microsoft Graph API REST и просматривать соответствующие ответы. Используйте Graph Explorer, чтобы попробовать API на примере клиента по умолчанию, чтобы изучить возможности или войти в собственный клиент и использовать его в качестве средства создания образцов для выполнения сценариев приложений. Этот инструмент включает такие полезные функции, как фрагменты кода в C#, Java, JavaScript и Objective C; Интеграция Graph набор средств и адаптивных карт; и более.

Используйте Graph Explorer для:

- Сделайте запросы Graph API Microsoft (GET, POST, PUT, PATCH и DELETE) и см. ответы, включая код ответа и любые заголовки и органы.
- Согласие на разрешения. Graph Explorer поддерживает только [делегированную разрешения.](/graph/auth/auth-concepts#delegated-and-application-permissions)
- Добавьте в запрос тело запроса и заглавный заголовок запроса.
- Просмотр и копирование маркера доступа.
- Просмотр примерных запросов для различных служб в Microsoft Graph.
- Просмотр, скачивание или удаление запросов за последние 30 дней.
- Просмотр и копирование фрагментов кода каждого запроса, запускаемого в C#, Java, JavaScript и Objective C.
- Доступ к компонентам Graph набор средств Microsoft и адаптивным картам для некоторых примерных запросов.
- Делитесь запросами, включая тело запроса и заглавные заголовки запросов.

Graph Explorer обрабатывает процесс проверки подлинности для вас. Настройка работы путем сбоя боковой панели или изменения темы.

## <a name="get-started"></a>Начало работы

Graph Explorer — это веб-приложение, которое находится в [центре Graph Майкрософт.](https://developer.microsoft.com/en-us/graph/graph-explorer) Это проект с открытым исходным кодом, и мы приветствуем ваши вклады и отзывы в [GitHub репо](https://github.com/microsoftgraph/microsoft-graph-explorer-v4).

Graph Обозреватель содержит следующие элементы:

1. Список выпаданий HTTP-глаголов
2. Список выпаданий версии API
3. Адресная планка запроса запроса
4. Пример запроса
5. Ссылка на документацию для примера запроса

:::image type="content" source="./images/getting-started.png" alt-text="Снимок экрана пользовательского интерфейса Graph Explorer." border="true":::

### <a name="make-a-get-request-in-graph-explorer"></a>Сделайте запрос GET в Graph Explorer

Чтобы выполнить запрос GET в Graph Explorer, вам не нужно вписаться. Просто нажмите пример запроса и пример данных будет показываться в предварительном просмотре ответа. 

:::image type="content" source="./images/making-a-get-request.png" alt-text="Снимок экрана примера запроса в Graph Explorer." border="true":::

Чтобы сделать запрос:

1. Выберите пример запроса и запустите его.
2. Получите код ответа HTTP.
3. См. ответ от API microsoft Graph с примерами данных.

Когда вы войдите в Graph Explorer и щелкните тот же запрос, ответ будет возвращен с реальными данными от клиента, в который вы подписались.

### <a name="running-non-get-requests-in-graph-explorer"></a>Запуск запросов без GET в Graph Explorer

Чтобы попробовать запросы POST, PUT, PATCH и DELETE, воставьте Graph Explorer с помощью Microsoft 365 учетной записи. Это может быть учетная запись организации для тестирования или демонстрации. Чтобы получить бесплатную Microsoft 365 E5 подписку на разработчика, а также средства и другие ресурсы, которые помогут вам создать решения для платформы Microsoft 365, присоединитесь к программе [Microsoft 365 разработчика](https://developer.microsoft.com/microsoft-365/dev-program). 

>[!IMPORTANT]
>Если вы решите войти с помощью своей учетной записи организации, запуск запроса, не влияемого на get, может повлиять на данные клиента.

Например, чтобы выполнить запрос POST, выберите POST в списке drop-down для глагола HTTP, а также добавьте тело запроса и заглавные заголовки запроса по мере необходимости.

:::image type="content" source="./images/making-a-post-request.png" alt-text="Снимок экрана запроса POST в Graph Explorer." border="true":::

1. Выберите пример запроса POST.
2. Обновление **тела запроса;** например, дайте приложению имя.
3. Нажмите **кнопку Выполнить запрос**.
4. См. ответ от Microsoft Graph API.

Чтобы просмотреть ответ в формате, помимо JSON по умолчанию, выберите вкладку Заглавные таблицы запроса в области запросов, определите пару ключ/значение и нажмите **кнопку Добавить**. 

:::image type="content" source="./images/adding-key-value-pairs.png" alt-text="Снимок экрана, на который показана вкладка заглавных Graph Explorer." border="true":::

## <a name="next-steps"></a>Дальнейшие действия

- Посетите [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/).
- Дополнительные возможности [Graph Explorer.](./graph-explorer-features.md)
- Внести или предоставить обратную связь [в GitHub репо](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).
