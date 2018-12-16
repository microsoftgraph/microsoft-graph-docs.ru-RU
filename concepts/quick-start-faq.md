---
title: 'Краткое руководство по Microsoft Graph: вопросы и ответы'
description: В этой статье представлены ответы на вопросы, связанные с краткими руководствами по Microsoft Graph.
author: jasonjoh
ms.author: jasonjoh
ms.date: 12/13/2018
ms.openlocfilehash: 55630e8fbdbccd8355d2b23e4c839d2ccec2b7d3
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283642"
---
# <a name="microsoft-graph-quick-start-faq"></a>Краткое руководство по Microsoft Graph: вопросы и ответы

В этой статье представлены ответы на вопросы, связанные с [краткими руководствами по Microsoft Graph](https://developer.microsoft.com/graph/quick-start).

## <a name="general-design"></a>Общая схема

В примерах, содержащихся в кратких руководствах, показано, как использовать всю мощь Microsoft Graph. В этих примерах выполняется доступ к двум службам с использованием одной проверки подлинности: к учетной записи Майкрософт и Outlook. В каждом кратком руководстве используются сведения из профилей пользователей с учетными записями Майкрософт и отображаются события из их календаря.

В каждом кратком руководстве необходимо выполнить четыре действия:

- выбрать необходимую платформу;
- получить идентификатор приложения (идентификатор клиента);
- выполнить сборку кода из примера;
- войти и просмотреть события в своем календаре.

В итоге вы получите приложение, готовое к запуску.

## <a name="general-quick-start-sample-questions"></a>Общие вопросы, касающиеся примеров из краткого руководства

<!-- markdownlint-disable MD026 -->

В этом разделе представлены ответы на вопросы о содержимом примеров из краткого руководства.

### <a name="can-i-get-the-quick-start-code-without-downloading-through-the-quick-start-page"></a>Можно ли получить код из краткого руководства, не выполняя скачивание на странице краткого руководства?

Да, конечно! Каждый скачиваемый экземпляр краткого руководства основан на [учебнике по Microsoft Graph](tutorials.md), поэтому у вас есть два других варианта для получения такого же исходного кода:

- Выполнить сборку кода самостоятельно, следуя пошаговым инструкциям из учебника.
- Скачать готовый проект из соответствующего репозитория GitHub и выполнить инструкции из файла сведений, чтобы настроить и запустить пример.

> **Примечание.** Мы работаем над созданием учебников для всех платформ, у которых в настоящее время есть краткие руководства. Для некоторых кратких руководств пока нет соответствующих учебников.

#### <a name="tutorials-and-github-repositories"></a>Учебники и репозитории GitHub

В таблице ниже перечислены соответствующие учебники и репозитории GitHub для каждого примера из краткого руководства.

| Краткое руководство | Учебник | Репозиторий GitHub |
|-------------|----------|-------------------|
| Android | Нет | [GitHub](https://github.com/microsoftgraph/android-java-connect-sample) |
| Angular | [Учебник](/graph/tutorials/angular) | [GitHub](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| ASP.NET MVC | [Учебник](/graph/tutorials/aspnet) | [GitHub](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| iOS Swift | Нет | [GitHub](https://github.com/microsoftgraph/ios-swift-connect-sample) |
| iOS Objective-C | Нет | [GitHub](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample) |
| Node.js | [Учебник](/graph/tutorials/node) | [GitHub](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| PHP | [Учебник](/graph/tutorials/php) | [GitHub](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| Python | [Учебник](/graph/tutorials/python) | [GitHub](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| Ruby | [Учебник](/graph/tutorials/ruby) | [GitHub](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| UWP | [Учебник](/graph/tutorials/uwp) | [GitHub](https://github.com/microsoftgraph/msgraph-training-uwp) |
| Xamarin | Нет | [GitHub](https://github.com/microsoftgraph/uwp-csharp-connect-sample) |

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>Почему в примерах из краткого руководства нет вариантов использования расширенной проверки подлинности?

Примеры из краткого руководства используются для ознакомления с функцией проверки подлинности и вызовов API Microsoft Graph. Дополнительные сведения о других потоках проверки подлинности см. в документации [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios).

### <a name="what-if-i-run-into-an-unexpected-error-or-problem-with-a-quick-start"></a>Что делать при возникновении непредвиденной ошибки или проблемы с кратким руководством?

Если не удается обеспечить правильную работу при использовании краткого руководства, опубликуйте проблему в соответствующем репозитории GitHub.

## <a name="didnt-find-what-you-need"></a>Не нашли то, что искали?

Если в этой статье вы не нашли ответ на интересующий вас вопрос касательно одного или нескольких кратких руководств, сообщите нам об этом в разделе **Отзыв** ниже.
