---
title: Контрольный список планирования миграции приложений
description: Контрольный список для переноса приложений из Azure AD Graph в Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: f8e231166fdb39676ce2778b369c6962cae70cb0
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882747"
---
# <a name="app-migration-planning-checklist"></a>Контрольный список планирования миграции приложений

> [!Important]
> API Graph Azure AD теперь является неподготовленным. Мы продолжим предоставлять техническую поддержку и обновления для системы безопасности, но больше не будем предоставлять обновления функций.
> Начиная с 30 июня 2022 г., поддержка Azure AD Graph будет прекратиться и мы больше не будем предоставлять техническую поддержку или обновления для системы безопасности. После этого приложения, использующие Azure AD Graph, больше не будут получать ответы от конечной точки Azure AD Graph.

Используйте следующий контрольный список для планирования миграции.

## <a name="step-1-review-the-differences-between-the-apis"></a>Шаг 1. Просмотр различий между API

Во многом Microsoft Graph похож на предыдущий Azure AD Graph. Во многих случаях просто измените имя и версию службы конечной точки в коде, и все должно работать.

Тем не менее, существуют различия. Изменены некоторые ресурсы, свойства, методы и основные возможности.

В частности, следует искать различия в следующих областях:

- [Запрос синтаксиса вызовов](migrate-azure-ad-graph-request-differences.md) между двумя службами
- [Отличия функций,](migrate-azure-ad-graph-feature-differences.md)такие как расширения каталогов, пакетная обработка, разнонаправленные запросы и так далее
- [Имена ресурсов сущности и](migrate-azure-ad-graph-resource-differences.md) их типы
- [Свойства объектов](migrate-azure-ad-graph-property-differences.md) запросов и ответов
- [Методы,](migrate-azure-ad-graph-method-differences.md)включая параметры и типы

## <a name="step-2-examine-api-use"></a>Шаг 2. Изучение использования API

[Проверьте API,](migrate-azure-ad-graph-audit-api-use.md) используемые вашим приложением, необходимые им разрешения, и сравните их со списком известных различий.  

Убедитесь, что API, необходимые вашему приложению, как правило, доступны в Microsoft Graph 1.0 и что эти API работают одинаково.

В некоторых случаях новые возможности и функции предназначены для замены более ранних подходов.

Используйте [обозреватель Graph для](https://aka.ms/ge) экспериментов с новыми вызовами и разработки новых подходов. Для наилучших результатов во sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.

## <a name="step-3-review-app-details"></a>Шаг 3. Просмотр сведений о приложении

- [Изменения регистрации](migrate-azure-ad-graph-app-registration.md) и согласия приложения (которых не должно быть).
- Библиотеки получения маркеров [и проверки подлинности.](migrate-azure-ad-graph-authentication-library.md)
- Для приложений .NET используйте [клиентские библиотеки.](migrate-azure-ad-graph-client-libraries.md)

## <a name="step-4-deploy-test-and-extend-your-app"></a>Шаг 4. Развертывание, тестирование и расширение приложения

Перед обновлением приложения для всех убедитесь, что вы тщательно протестировали свое приложение и развяли его для аудитории клиента.

Теперь, когда вы перешли на Microsoft Graph, вам никогда не было проще разблокировать намного больше наборов данных и функций, которые теперь находятся под рукой. Вы можете получить опробуя возможности, изумив некоторые основные службы и [функции в Microsoft Graph.](./overview-major-services.md)

Если вы в настоящее время используете библиотеку проверки подлинности [AD](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), рассмотрите возможность перехода на библиотеку проверки подлинности [Майкрософт](/azure/active-directory/develop/reference-v2-libraries) (MSAL).

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте о [синтаксис вызова](migrate-azure-ad-graph-request-differences.md) запроса для начала шага 1: просмотр различий API.