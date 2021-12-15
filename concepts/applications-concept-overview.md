---
title: Общие сведения об API приложений
description: Зарегистрируйте свое приложение в Azure AD, чтобы создать для него конфигурацию удостоверения для интеграции с Azure AD.
author: FaithOmbongi
ms.localizationpriority: high
ms.prod: applications
ms.custom: scenarios:getting-started
ms.openlocfilehash: c0e264cb0b0b9b638741aeb0db774efd121c83e9
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526172"
---
# <a name="applications-api-overview"></a>Общие сведения об API приложений

Чтобы делегировать функции управления удостоверениями и доступом в Azure AD, необходимо зарегистрировать приложение в клиенте Azure AD. При регистрации приложения в Azure AD для него создается конфигурация удостоверения для интеграции с Azure AD.

## <a name="why-use-applications-and-associated-resources"></a>Зачем использовать приложения и связанные с ними ресурсы?

Интерфейсы API Microsoft Graph позволяют управлять этими ресурсами и действиями, относящимися к приложениям в службе Azure Active Directory.
- **Управление приложениями**: служба Azure AD должна быть настроена для интеграции с приложением. Другими словами, ей нужно знать, какие приложения ее используют в качестве системы удостоверений. Процесс поддержания в актуальном состоянии знаний Azure AD об этих приложениях и о том, как с ними следует обращаться, называется управлением приложениями.
- **Локальная публикация**: локальные агенты (или соединители для прокси приложений), установленные администратором клиента, можно настроить для маршрутизации запросов к определенному опубликованному ресурсу.
- **Управление субъектом-службой**: локальное представление или экземпляр глобального приложения в одном клиенте или каталоге. Субъект-служба — это конкретный экземпляр, созданный на основе объекта приложения, который наследует определенные свойства объекта приложения.
- **Синхронизация**: синхронизация удостоверений Azure Active Directory (Azure AD) (которая также называется *подготовкой*) позволяет автоматизировать создание, обслуживание и удаление удостоверений в облаке.

## <a name="application-management"></a>Управление приложениями

Регистрация приложения включает уведомление Azure AD о вашем приложении, в том числе URL-адрес его расположения, URL-адрес для отправки ответов после проверки подлинности, URI для определения приложения и многое другое. Чтобы управлять приложениями программными средствами, можно использовать [интерфейсы API приложений](/graph/api/resources/application?view=graph-rest-1.0) в Microsoft Graph.

> [!VIDEO https://www.youtube-nocookie.com/embed/93j0MmRruFo]

Дополнительные сведения о приложениях см. в следующих статьях:
- [Модель приложения](/azure/active-directory/develop/application-model)
- [Объекты приложения и субъекта-службы в Azure Active Directory](/azure/active-directory/develop/app-objects-and-service-principals)
- [Типы приложений для платформы удостоверений Майкрософт](/azure/active-directory/develop/v2-app-types)

Дополнительные сведения об управлении приложениями см. в следующих статьях:
- [Что такое управление мобильными приложениями?](/azure/active-directory/manage-apps/what-is-application-management)
- [Сценарии проверки подлинности и сценарии приложений](/azure/active-directory/develop/authentication-flows-app-scenarios)

## <a name="on-premises-publishing-preview"></a>Доступ к локальной публикации (предварительная версия)

Создание локальных профилей публикаций и управление ими, включая создание локальных агентов и групп агентов. Чтобы управлять локальными профилями публикации программными средствами, можно использовать [интерфейсы API локальной публикации](/graph/api/resources/onpremisespublishingprofile-root) в Microsoft Graph.

Дополнительные сведения о локальной публикации см. в следующих статьях:
- [Удаленный доступ к локальным приложениям с помощью прокси приложения Azure Active Directory](/azure/active-directory/manage-apps/application-proxy)
- [Использование прокси приложения Azure AD для публикации локальных приложений для удаленных пользователей](/azure/active-directory/manage-apps/what-is-application-proxy)

Чтобы узнать о том, как использовать интерфейсы API локальной публикации, см. следующее руководство и связанные с ним API:
- [Автоматизация настройки прокси приложения с помощью API Microsoft Graph.](./application-proxy-configure-api.md)
    - [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [application](/graph/api/resources/application?view=graph-rest-1.0)
    - [onPremisesPublishing](/graph/api/resources/onpremisespublishingprofile-root)
    - [connector](/graph/api/resources/connector)
    - [connectorGroup](/graph/api/resources/connectorgroup)
    - [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="service-principal-management"></a>Управление именем субъекта-службы (SPN)

Чтобы получить доступ к ресурсам, защищенным клиентом Azure AD, субъект, которому требуется доступ, должен быть представлен субъектом безопасности. Чтобы управлять субъектами-службами программными средствами, можно воспользоваться [интерфейсами API субъекта-службы](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) в Microsoft Graph.

Подробнее о субъектах-службах см. в разделе[Объекты приложения и субъекта-службы в Azure Active Directory](/azure/active-directory/develop/app-objects-and-service-principals).

## <a name="synchronization"></a>Синхронизация

Можно воспользоваться [интерфейсами API синхронизации](/graph/api/resources/synchronization-overview) в Microsoft Graph для управления синхронизацией удостоверений программными средствами, в том числе для:
- создания, запуска и остановки заданий синхронизации
- изменения схемы синхронизации для заданий
- проверки текущего состояния синхронизации

Дополнительные сведения о синхронизации см. в следующих статьях:
- [Автоматизация подготовки пользователей для приложений и ее отмена с помощью Azure AD](/azure/active-directory/app-provisioning/user-provisioning)
- [Как работает подготовка](/azure/active-directory/app-provisioning/how-provisioning-works)

Чтобы узнать о том, как использовать интерфейсы API локальной публикации, см. следующие руководства и связанные с ними API:
- [Настройка подготовки с помощью интерфейсов API Microsoft Graph](/azure/active-directory/app-provisioning/application-provisioning-configure-api):
    - [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [synchronizationTemplate](/graph/api/resources/synchronization-synchronizationtemplate)
    - [synchronizationJob](/graph/api/resources/synchronization-synchronizationjob)
- [Автоматизация настройки единого входа на основе SAML для приложений с помощью API Microsoft Graph](/azure/active-directory/manage-apps/application-saml-sso-configure-api)
    - [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [application](/graph/api/resources/application?view=graph-rest-1.0)
    - [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy)
    - [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="next-steps"></a>Дальнейшие действия
- Протестируйте интерфейс API Microsoft Graph в [Песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- С помощью [этих примеров](/azure/active-directory/develop/sample-v2-code) узнайте о том, как добавить в веб-приложения и веб-API проверку подлинности и авторизацию.
