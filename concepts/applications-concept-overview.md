---
title: Общие сведения об API приложений
description: Зарегистрируйте свое приложение с помощью Azure AD, чтобы создать конфигурацию удостоверения, позволяющую интегрироваться с Azure AD.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: scenarios:getting-started
ms.openlocfilehash: ff38e14182d2e38fbc2203241da911dec07f9846
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081205"
---
# <a name="applications-api-overview"></a>Общие сведения об API приложений

Чтобы делегировать функции управления удостоверениями и доступом в Azure AD, приложение должно быть зарегистрировано в клиенте Azure AD. При регистрации приложения в Azure AD вы создаете конфигурацию удостоверения для вашего приложения, которое позволяет им интегрироваться с Azure AD.

## <a name="why-use-applications-and-associated-resources"></a>Зачем использовать приложения и связанные ресурсы?

API Microsoft Graph позволяют управлять этими ресурсами и действиями, относящимися к приложениям в Azure Active Directory:
- **Управление приложениями** — служба Azure AD должна быть настроена для интеграции с приложением. Другими словами, им необходимо знать, какие приложения используют его в качестве системы идентификации. Процесс поддержания этих приложений службой Azure AD и то, как он должен их обрабатывать, называется "Управление приложениями".
- Локальные агенты **публикации** (или соединители для прокси-сервера приложений), установленные администратором клиента, можно настроить на маршрутизацию запросов к определенному опубликованному ресурсу.
- **Управление субъектами служб** — локальное представление или экземпляр приложения глобального объекта приложения в отдельном клиенте или каталоге. Участник службы — это конкретный экземпляр, созданный из объекта Application и наследующий определенные свойства этого объекта Application.
- **Синхронизация** удостоверений Azure Active Directory (Azure AD) (также называемая *подготовкой*) позволяет автоматизировать создание, Обслуживание и удаление удостоверений в облаке.

## <a name="application-management"></a>Управление приложениями

Регистрация приложения включает уведомление Azure AD о вашем приложении, в том числе URL-адрес его расположения, URL-адрес для отправки ответов после проверки подлинности, URI для определения приложения и многое другое. С помощью [API приложений](/graph/api/resources/application?view=graph-rest-1.0) в Microsoft Graph можно управлять приложениями программным способом.

> [!VIDEO https://www.youtube-nocookie.com/embed/93j0MmRruFo]

Дополнительные сведения о приложениях можно найти в следующих статьях:
- [Модель приложения](https://docs.microsoft.com/azure/active-directory/develop/application-model)
- [Объекты приложения и субъекта-службы в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
- [Типы приложений для платформы удостоверений Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/v2-app-types)

Дополнительные сведения об управлении приложениями можно найти в следующих статьях:
- [Что такое управление приложениями?](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-application-management)
- [Потоки проверки подлинности и сценарии приложений](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios)

## <a name="on-premises-publishing-preview"></a>Локальная публикация (Предварительная версия)

Создание локальных профилей публикации и управление ими, включая создание локальных агентов и групп агентов. Вы можете использовать [локальные интерфейсы API публикации](/graph/api/resources/onpremisespublishingprofile-root) в Microsoft Graph для управления локальными профилями публикации программным способом.

Дополнительные сведения об локальной публикации приведены в следующих статьях:
- [Удаленный доступ к локальным приложениям через прокси-сервер приложений Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy)
- [Использование прокси-сервера приложения Azure AD для публикации локальных приложений для удаленных пользователей](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-application-proxy)

Для получения сведений об использовании API локальной публикации ознакомьтесь со следующими учебными материалами и связанными с ними API:
- [Автоматизация настройки прокси-сервера приложений с помощью API Microsoft Graph](https://docs.microsoft.com/graph/application-proxy-configure-api)
    - [аппликатионтемплате](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [application](/graph/api/resources/application?view=graph-rest-1.0)
    - [онпремисеспублишинг](/graph/api/resources/onpremisespublishingprofile-root)
    - [PDIF](/graph/api/resources/connector)
    - [connectorGroup](/graph/api/resources/connectorgroup)
    - [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="service-principal-management"></a>Управление субъектами служб

Чтобы получить доступ к ресурсам, защищенным клиентом Azure AD, объект, которому требуется доступ, должен быть представлен участником безопасности. С помощью [API субъектов-служб](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) в Microsoft Graph можно управлять субъектами-службами программным способом.

Дополнительные сведения об участниках служб содержатся в разделе [Application and Service Principal Objects in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).

## <a name="synchronization"></a>Синхронизация

С помощью [API синхронизации](/graph/api/resources/synchronization-overview) в Microsoft Graph можно управлять синхронизацией удостоверений программным способом, в том числе:
- Создание, запуск и остановка заданий синхронизации
- Внесение изменений в схему синхронизации для заданий
- Проверка текущего состояния синхронизации

Дополнительные сведения о синхронизации можно найти в следующих статьях:
- [Автоматизация подготовки пользователей и их отмена в приложениях с помощью Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)
- [Как работает подготовка](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works)

Чтобы узнать больше об использовании API синхронизации, ознакомьтесь со следующими учебными материалами и связанными с ними API:
- [Настройка подготовки с помощью API Microsoft Graph](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api)
    - [аппликатионтемплате](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [синчронизатионтемплате](/graph/api/resources/synchronization-synchronizationtemplate)
    - [синчронизатионжоб](/graph/api/resources/synchronization-synchronizationjob)
- [Автоматизация настройки приложения единого входа на основе SAML с помощью API Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api)
    - [аппликатионтемплате](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [application](/graph/api/resources/application?view=graph-rest-1.0)
    - [клаимсмаппингполици](/graph/api/resources/claimsmappingpolicy)
    - [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="next-steps"></a>Дальнейшие действия
- Попробуйте использовать API Microsoft Graph в [проводнике Graph](https://developer.microsoft.com/graph/graph-explorer).
- Узнайте, как добавить проверку подлинности и авторизацию в веб-приложения и веб-API с помощью [этих примеров](https://docs.microsoft.com/azure/active-directory/develop/sample-v2-code).
