---
title: Контрольный список планирования миграции приложений
description: Контрольный список для переноса приложений из Azure Active Directory (Azure AD) Graph в Microsoft Graph
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 23b650b9e1d8dc046f6b503a2ded6f9c8ae8a5ad
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139053"
---
# <a name="app-migration-planning-checklist"></a>Контрольный список планирования миграции приложений

Чтобы спланировать миграцию, используйте следующий контрольный список.

## <a name="step-1-review-the-differences-between-the-apis"></a>Шаг 1. Обзор различий между API

Во многих отношениях microsoft Graph похожа на более ранние Azure Active Directory (Azure AD) Graph. Во многих случаях просто измените имя и версию службы конечной точки в коде, и все должно продолжать работать.

Тем не менее существуют различия. Изменились некоторые ресурсы, свойства, методы и основные возможности.

В частности, и посмотрите на различия в следующих областях:

- [Запрос синтаксиса вызовов](migrate-azure-ad-graph-request-differences.md) между двумя службами
- [Отличия функций,](migrate-azure-ad-graph-feature-differences.md)например расширения каталогов, пакетные пакеты, дифференциальные запросы и так далее
- [Имена ресурсов Entity и](migrate-azure-ad-graph-resource-differences.md) их типы
- [Свойства объектов](migrate-azure-ad-graph-property-differences.md) запроса и ответа
- [Методы,](migrate-azure-ad-graph-method-differences.md)включая параметры и типы

## <a name="step-2-examine-api-use"></a>Шаг 2. Изучение использования API

[Изучите API,](migrate-azure-ad-graph-audit-api-use.md) используемые вашим приложением, необходимые разрешения и сравните со списком известных различий.  

Убедитесь, что API, необходимые вашему приложению, обычно доступны в Microsoft Graph v1.0 и что эти API работают одинаково.

В некоторых случаях новые возможности и функции предназначены для замены более ранних подходов.

Используйте [Graph Explorer](https://aka.ms/ge) для экспериментов с новыми вызовами и разработки новых подходов. Для наилучших результатов впишитесь с помощью учетных данных тест-пользователя в тестовом клиенте, чтобы увидеть, что API делает над важными наборами данных.

## <a name="step-3-review-app-details"></a>Шаг 3. Просмотр сведений о приложении

- [Изменения регистрации](migrate-azure-ad-graph-app-registration.md) и согласия приложения (которых должно быть нет).
- Библиотеки приобретения маркеров [и проверки подлинности.](migrate-azure-ad-graph-authentication-library.md)
- Для приложений .NET используйте [клиентские библиотеки.](migrate-azure-ad-graph-client-libraries.md)

## <a name="step-4-deploy-test-and-extend-your-app"></a>Шаг 4. Развертывание, тестирование и расширение приложения

Перед обновлением приложения для всех убедитесь, что вы тщательно протестировать и этап вашего выкатки для вашей клиентской аудитории.

Теперь, когда вы перешли на Microsoft Graph, вам никогда не было проще разблокировать множество наборов данных и функций, которые теперь находятся у вас под рукой. Вы можете получить вкус того, что возможно, посмотрев на некоторые основные службы и функции в [Microsoft Graph](./overview-major-services.md).

[Библиотека проверки подлинности](/azure/active-directory/develop/reference-v2-libraries) Майкрософт (MSAL) теперь является рекомендуемой библиотекой проверки подлинности для использования в платформа удостоверений Майкрософт. Если вы используете библиотеку [Azure Active Directory](/azure/active-directory/develop/active-directory-authentication-libraries) проверки подлинности (ADAL), запланируйте переход на MSAL. Дополнительные рекомендации по переносу приложений в Библиотеку проверки подлинности [Майкрософт (MSAL).](/azure/active-directory/develop/msal-migration)

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте о [синтаксисе](migrate-azure-ad-graph-request-differences.md) вызовов запросов, чтобы начать шаг 1: рассмотрение различий API.
