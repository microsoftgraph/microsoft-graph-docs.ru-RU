---
title: 'Краткое руководство по Microsoft Graph: вопросы и ответы'
description: В этой статье представлены ответы на вопросы, связанные с краткими руководствами по Microsoft Graph.
author: jasonjoh
ms.author: jasonjoh
localization_priority: Normal
ms.openlocfilehash: 00e1d3d20276c888f2f22d7e62f7434da282bca9
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806822"
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

Да, конечно! Каждый скачиваемый экземпляр краткого руководства основан на [учебнике по Microsoft Graph](tutorials.yml), поэтому у вас есть два других варианта для получения такого же исходного кода:

- Выполнить сборку кода самостоятельно, следуя пошаговым инструкциям из учебника.
- Скачать готовый проект из соответствующего репозитория GitHub и выполнить инструкции из файла сведений, чтобы настроить и запустить пример.

> [!NOTE]
> Мы работаем над созданием учебников для всех платформ, у которых в настоящее время есть краткие руководства. Для некоторых кратких руководств пока нет соответствующих учебников.

#### <a name="tutorials-and-github-repositories"></a>Учебники и репозитории GitHub

В таблице ниже перечислены соответствующие учебники и репозитории GitHub для каждого примера из краткого руководства.

| Краткое руководство | Учебник | Репозиторий GitHub |
|-------------|----------|-------------------|
| Android | [Учебник](/graph/tutorials/android) | [GitHub](https://github.com/microsoftgraph/msgraph-training-android) |
| Angular | [Учебник](/graph/tutorials/angular) | [GitHub](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| ASP.NET MVC | [Учебник](/learn/modules/msgraph-build-aspnetmvc-apps) | [GitHub](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| iOS Swift | Повторен (/граф/туториалс/Иос-Свифт | [GitHub](https://github.com/microsoftgraph/msgraph-training-ios-swift) |
| iOS Objective-C | Повторен (/граф/туториалс/Иос-обжективек | [GitHub](https://github.com/microsoftgraph/msgraph-training-ios-objectivec) |
| Node.js | [Учебник](/graph/tutorials/node) | [GitHub](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| PHP | [Учебник](/graph/tutorials/php) | [GitHub](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| Python | [Учебник](/graph/tutorials/python) | [GitHub](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| React | [Учебник](/graph/tutorials/react) | [GitHub](https://github.com/microsoftgraph/msgraph-training-reactspa) |
| Ruby | [Учебник](/graph/tutorials/ruby) | [GitHub](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| UWP | [Учебник](/graph/tutorials/uwp) | [GitHub](https://github.com/microsoftgraph/msgraph-training-uwp) |
| Xamarin | Повторен (/граф/туториалс/ксамарин | [GitHub](https://github.com/microsoftgraph/msgraph-training-xamarin) |

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>Почему в примерах из краткого руководства нет вариантов использования расширенной проверки подлинности?

Примеры из краткого руководства используются для ознакомления с функцией проверки подлинности и вызовов API Microsoft Graph. Дополнительные сведения о других потоках проверки подлинности см. в документации [Azure Active Directory](/azure/active-directory/develop/authentication-scenarios).

### <a name="what-if-i-run-into-an-unexpected-error-or-problem-with-a-quick-start"></a>Что делать при возникновении непредвиденной ошибки или проблемы с кратким руководством?

Если не удается обеспечить правильную работу при использовании краткого руководства, опубликуйте проблему в соответствующем репозитории GitHub.

## <a name="known-issues"></a>Известные проблемы

### <a name="aspnet-quick-start-displays-an-error-when-running-it-cannot-find-a-part-of-the-path-graph-tutorialgraph-tutorialbinroslyncscexe"></a>При запуске краткого руководства ASP.NET отображается ошибка "Не удается найти часть пути [...]\Graph Tutorial\graph-tutorial\bin\roslyn\csc.exe".

Это вызвано [проблемой с Visual Studio и компилятором Roslyn](https://github.com/dotnet/roslyn/issues/15556). Исправить эту ошибку можно одним из следующих вариантов:

- Выгрузка и повторная загрузка проекта в обозревателе решений
- Очистка и перестройка решения
- Обновление пакетов NuGet

### <a name="im-getting-aadsts50011-the-reply-url-specified-in-the-request-does-not-match-the-reply-urls-configured-for-the-application-when-running-a-quick-start"></a>При запуске краткого руководства возникает ошибка "AADSTS50011: URL-адрес ответа, указанный в запросе, не совпадает с URL-адресами ответов, настроенными для приложения".

Это указывает на проблему с регистрацией приложения для краткого руководства. Когда вы скачиваете краткое руководство со [страницы кратких руководств Microsoft Graph](https://developer.microsoft.com/graph/quick-start), для вас создается регистрация приложение и выполняется настройка URL-адреса ответа (другое название — URL-адрес перенаправления), совпадающего с URL-адресом по умолчанию, который используется примером проекта. Если изменить URL-адрес, нарушается соответствие регистрации приложения, и может возникнуть эта ошибка. Чтобы устранить эту ошибку, обратитесь к файлу README.md, включенному в проект краткого руководства, за инструкциями о том, как создать регистрацию приложения и настроить ее в примере кода.

## <a name="didnt-find-what-you-need"></a>Не нашли то, что искали?

Если в этой статье вы не нашли ответ на интересующий вас вопрос касательно одного или нескольких кратких руководств, сообщите нам об этом в разделе **Отзыв** ниже.
