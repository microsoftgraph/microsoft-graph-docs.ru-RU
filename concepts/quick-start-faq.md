---
title: 'Краткое руководство по Microsoft Graph: вопросы и ответы'
description: В этой статье представлены ответы на вопросы, связанные с краткими руководствами по Microsoft Graph.
author: jasonjoh
ms.author: jasonjoh
localization_priority: Normal
ms.openlocfilehash: 4aded41cab30133856041c073699948ed7ae49ff
ms.sourcegitcommit: 093d89c7583bb6880c8395e9498a1f33cdd938b4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44568756"
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

## <a name="prerequisites"></a>Необходимые компоненты

Для всех примеров быстрого запуска требуется доступ к личной учетной записи Майкрософт с почтовым ящиком на Outlook.com или с помощью рабочей или учебной учетной записи Майкрософт с почтовым ящиком Exchange Online. Если у вас нет учетной записи Майкрософт, у вас есть несколько вариантов для получения бесплатной учетной записи:

- Вы можете [зарегистрироваться для создания новой личной учетной записи Майкрософт](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1).
- Вы можете [зарегистрироваться в программе для разработчиков office 365](https://developer.microsoft.com/office/dev-program) , чтобы получить бесплатную подписку на Office 365.

## <a name="general-quick-start-sample-questions"></a>Общие вопросы, касающиеся примеров из краткого руководства

<!-- markdownlint-disable MD026 -->

В этом разделе представлены ответы на вопросы о содержимом примеров из краткого руководства.

### <a name="can-i-get-the-quick-start-code-without-downloading-through-the-quick-start-page"></a>Можно ли получить код из краткого руководства, не выполняя скачивание на странице краткого руководства?

Да, конечно! Каждый скачиваемый экземпляр краткого руководства основан на [учебнике по Microsoft Graph](tutorials.yml), поэтому у вас есть два других варианта для получения такого же исходного кода:

- Выполнить сборку кода самостоятельно, следуя пошаговым инструкциям из учебника.
- Скачать готовый проект из соответствующего репозитория GitHub и выполнить инструкции из файла сведений, чтобы настроить и запустить пример.

#### <a name="tutorials-and-github-repositories"></a>Учебники и репозитории GitHub

В таблице ниже перечислены соответствующие учебники и репозитории GitHub для каждого примера из краткого руководства.

| Краткое руководство | Учебник | Репозиторий GitHub |
|-------------|----------|-------------------|
| Android | [Учебник](/graph/tutorials/android) | [GitHub](https://github.com/microsoftgraph/msgraph-training-android) |
| Angular | [Учебник](/graph/tutorials/angular) | [GitHub](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| ASP.NET MVC | [Учебник](/learn/modules/msgraph-build-aspnetmvc-apps) | [GitHub](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| iOS Swift | [Учебник](/graph/tutorials/ios-swift) | [GitHub](https://github.com/microsoftgraph/msgraph-training-ios-swift) |
| iOS Objective-C | [Учебник](/graph/tutorials/ios-objectivec) | [GitHub](https://github.com/microsoftgraph/msgraph-training-ios-objectivec) |
| Node.js | [Учебник](/graph/tutorials/node) | [GitHub](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| PHP | [Учебник](/graph/tutorials/php) | [GitHub](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| Python | [Учебник](/graph/tutorials/python) | [GitHub](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| React | [Учебник](/graph/tutorials/react) | [GitHub](https://github.com/microsoftgraph/msgraph-training-reactspa) |
| Ruby | [Учебник](/graph/tutorials/ruby) | [GitHub](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| UWP | [Учебник](/graph/tutorials/uwp) | [GitHub](https://github.com/microsoftgraph/msgraph-training-uwp) |
| Xamarin | [Учебник](/graph/tutorials/xamarin) | [GitHub](https://github.com/microsoftgraph/msgraph-training-xamarin) |

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

### <a name="after-signing-in-im-told-i-need-admin-approval"></a>Войдя в программу, я хотел, чтобы он был одобрен администратором.

После входа в один из примеров краткого руководства вы можете увидеть сообщение, в котором говорится о **необходимости утверждения администратором** "XXX" требуется разрешение на доступ к ресурсам Организации, которые могут быть предоставлены только администратором. Попросите администратора предоставить разрешение для этого приложения, прежде чем его можно будет использовать. " Эта ошибка не является ошибкой для примера! Ни один из быстрых запусков не запрашивает все области разрешений графа, которые по *умолчанию* требуют согласия администратора. Администраторы клиентов могут отключить возможность предоставления согласия на области разрешений графа для любых приложений, которые не были утверждены. В этом случае вы увидите эту ошибку.

Для получения утверждения необходимо обратиться к администратору, использовать личную учетную запись Майкрософт (Outlook.com) или протестировать клиент Microsoft 365 с Exchange Online.

## <a name="didnt-find-what-you-need"></a>Не нашли то, что искали?

Если в этой статье вы не нашли ответ на интересующий вас вопрос касательно одного или нескольких кратких руководств, сообщите нам об этом в разделе **Отзыв** ниже.
