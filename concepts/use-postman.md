---
title: Использование Postman с API Microsoft Graph
description: Используйте коллекцию Microsoft Graph Postman, чтобы начать работу с API Microsoft Graph в считанные минуты.
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: 0a26b444249a6ee85f875b3a88222f4404aaa238
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243068"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a>Использование Postman с API Microsoft Graph

Вы можете использовать коллекцию Microsoft Graph Postman, чтобы начать работу с API Microsoft Graph в считанные минуты.

![Изображение Postman](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

В этой статье рассказывается о том, как быстро приступить к работе с Postman и Microsoft Graph. Кроме того, вы можете просматривать API Microsoft Graph непосредственно в веб-браузере с помощью [песочницы Graph](https://developer.microsoft.com/ru-RU/graph/graph-explorer).

## <a name="accessing-the-collection"></a>Доступ к коллекции
Доступ к коллекции в Postman можно получить двумя способами: путем ее потребления или путем добавления к ней. Вначале вам потребуется запустить [Postman](https://www.getpostman.com/) на вашем компьютере.

### <a name="consume-the-collection"></a>Потребление коллекции
Потребление коллекции – самый простой способ начать работу с API Microsoft Graph. [Ссылка совместного доступа Postman](https://www.getpostman.com/collections/d89a737b5f0c0825898a) запустит Postman.

Преимущество использования коллекции с общим доступом заключается в том, что новые запросы будут автоматически отображаться без каких-либо дополнительных действий с вашей стороны.

После получения доступа к коллекции необходимо настроить переменные среды:

1. Выберите **Файл | Импорт ...**.
2. Выберите **Импорт из ссылки**.
3. Скопируйте и вставьте следующий URL-адрес, затем выберите **Импорт**.
 
    ```
    https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_environment.json
    ```

В правой верхней части окна должна отобразиться **среда Microsoft Graph** в виде значка с изображением глаза. Теперь необходимо [настроить среду](#using-the-collection).

### <a name="contribute-to-the-collection"></a>Добавление в коллекцию
Если вы хотите добавить собственные запросы, вам потребуется создать развилку репозитория GitHub [коллекций Postman Microsoft Graph](https://github.com/microsoftgraph/microsoftgraph-postman-collections). 

Дополнительные сведения о том, как это сделать, см. в следующем видео.

> [!VIDEO https://www.youtube-nocookie.com/embed/4tg-OBdv_8o]

Чтобы импортировать коллекции Postman:

1. Скачайте и зарегистрируйтесь для использования [Postman](https://www.getpostman.com/).
2. Выберите **Файл | Импорт ...**.
3. Выберите **Импорт из ссылки**.
4. Вставьте два указанных ниже URL-адреса и выберите **Импорт** после каждого из них.

    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_collection.json
      
    ```
    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_environment.json

    ```

Теперь в области **Коллекции** должна отобразиться коллекция **Microsoft Graph v1.0**.

## <a name="using-the-collection"></a>Использование коллекции
После создания коллекции **Microsoft Graph v1.0** и **среды Microsoftr Graph** в Postman, выполните указанные ниже действия.

### <a name="set-up-application-api-calls"></a>Настройка вызовов API приложений

1. В правом верхнем углу выберите **Без среды** из раскрывающегося списка.
2. Выберите **Среда Microsoft Graph**.
3. Щелкните значок с изображением **глаза** справа и затем выберите **Изменить**. 
4. Введите свое приложение Microsoft Identity в **текущих** (не **начальных**) переменных: **ClientID**, **ClientSecret** и ** TenantID**. 
 Дополнительные сведения о том, как создать приложение и настроить согласие администратора для потока только для приложений, см запись блога[Использование Postman для осуществления вызовов Microsoft Graph](https://developer.microsoft.com/en-us/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/).

5. Нажмите кнопку **Обновить**. Закройте диалоговое окно** Управление средами.** В коллекции **MicrosoftGraph v1.0 | Приложение** с левой стороны, выберите **Получить маркер доступа только для приложений**. Затем в правой части нажмите кнопку **Отправить**.
6. Разверните папку **Приложение | Пользователи** и выберите **Получить пользователей**. Затем нажмите кнопку **Отправить**.

Теперь вы можете работать с коллекциями Microsoft Graph v 1.0.

>**Примечание.** Если вы хотите использовать другие API в коллекции, вам будет необходимо подтвердить разрешения, необходимые для вашего приложения.

### <a name="set-up-on-behalf-of-api-calls"></a>Настройка вызовов API по сценарию “от имени”
Самый простой способ настроить вызовы API по сценарию “от имени” – это указать **UserName (Имя пользователя)** и **UserPassword (Пароль пользователя)** в параметрах среды и использовать **От имени пользователя | Получить маркер доступа пользователя**. 

>**Важно!** мы не рекомендуем использовать учетные записи пользователей рабочей среды, так как эта информация хранится непосредственно в Postman. Также не рекомендуем использовать этот способ для получения маркеров доступа в рабочей среде. Используйте его только в целях тестирования.

Если вы не хотите хранить имена пользователей и пароли в переменных среды, которые синхронизируются с вашей облачной учетной записью Postman, можно использовать возможность **Получить новый маркер доступа**, чтобы получить маркер, не выходя из Postman.

1. Выберите **От имени пользователя | Получить маркер доступа с помощью Postman**.
2. Откройте вкладку **Авторизация**.
3. Нажмите кнопку **Получить новый маркер доступа**
4. Заполните приведенные ниже поля с реальными значениями клиента и приложения. Обратите внимание на то, что здесь вы не можете использовать переменные среды: необходимо использовать фактические значения. Их можно найти, выбрав **EndPoints (конечные точки)** в колонке приложения на portal.azure.com.

    - URL-адрес обратного вызова: https://app.getpostman.com/oauth2/callback
    - URL-адрес проверки подлинности: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize
    - URL-адрес маркера доступа: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token
    - Идентификатор клиента: **CLIENTID**
    - Секрет клиента: **CLIENTSECRET**
    - Область: https://graph.microsoft.com/.default
    - Состояние: **RANDOMSTRING**
 
5. Нажмите **Запросить маркер**. Вы увидите запрос пользовательского интерфейса на вход в систему и одобрение разрешений.
6. Скопируйте маркер доступа, откройте ваши переменные среды и вставьте его в поле **UserAccessToken (Маркер доступа пользователя)**.

Теперь все ваши запросы будут рабочими.
