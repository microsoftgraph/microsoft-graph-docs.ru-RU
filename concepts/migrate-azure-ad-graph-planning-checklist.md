---
title: Контрольный список миграции приложения Graph в Azure Active Directory (Azure AD)
description: Используйте этот контрольный список для переноса приложений из Azure Active Directory (Azure AD) Graph в Microsoft Graph.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: ca3625d7462d1801dc5056f6f65246495aee1e56
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577702"
---
# <a name="azure-ad-graph-app-migration-planning-checklist"></a>Azure AD планирования миграции приложений Graph

Используйте следующий контрольный список для планирования миграции из Azure Active Directory (Azure AD) Graph в Microsoft Graph.

## <a name="step-1-review-the-differences-between-the-apis"></a>Шаг 1. Просмотр различий между API-интерфейсами

Во многом Microsoft Graph похож на предыдущий Azure AD Graph. Во многих случаях просто измените имя и версию службы конечной точки в коде, и все должно продолжать работать.

Тем не менее существуют различия. Некоторые ресурсы, свойства, методы и основные возможности были изменены.

В частности, найдите различия в следующих областях:

- [Синтаксис вызова запроса](migrate-azure-ad-graph-request-differences.md) между двумя службами
- [Различия в функциях](migrate-azure-ad-graph-feature-differences.md), такие как расширения каталогов, пакетная обработка, разностные запросы и т. д.
- [Имена ресурсов сущностей](migrate-azure-ad-graph-resource-differences.md) и их типы
- [Свойства объектов](migrate-azure-ad-graph-property-differences.md) запроса и ответа
- [Методы](migrate-azure-ad-graph-method-differences.md), включая параметры и типы

## <a name="step-2-examine-api-use"></a>Шаг 2. Изучение использования API

[Изучите API](migrate-azure-ad-graph-audit-api-use.md) - интерфейсы, используемые приложением, требуемые разрешения, и сравните их со списком известных различий.  

Убедитесь, что API, необходимые вашему приложению, общедоступны в Microsoft Graph версии 1.0 и работают одинаково.

В некоторых случаях новые возможности и функции предназначены для замены более ранних подходов.

Используйте [песочницу Graph](https://aka.ms/ge) для экспериментов с новыми вызовами и разработки новых подходов. Для получения наилучших результатов войдите, используя учетные данные тестового пользователя в тестовом клиенте, чтобы увидеть, что API делает над важными наборами данных.

## <a name="step-3-review-app-details"></a>Шаг 3. Просмотр сведений о приложении

- [Изменения регистрации](migrate-azure-ad-graph-app-registration.md) и согласия приложения (которых не должно быть).
- Библиотеки получения маркеров [и проверки подлинности](migrate-azure-ad-graph-authentication-library.md).
- Для .NET приложений используйте [клиентские библиотеки](migrate-azure-ad-graph-client-libraries.md).

## <a name="step-4-deploy-test-and-extend-your-app"></a>Шаг 4. Развертывание, тестирование и расширение приложения

Перед обновлением приложения для всех убедитесь, что вы тщательно протестируйте и выполните развертывание для аудитории клиента.

Теперь, когда вы переключились на Microsoft Graph, вам никогда не было проще разблокировать множество дополнительных наборов данных и функций, которые теперь находятся под рукой. Чтобы получить представление о возможностях, ознакомьтесь с некоторыми основными службами [и функциями Microsoft Graph](./overview-major-services.md).

[Библиотека проверки подлинности](/azure/active-directory/develop/reference-v2-libraries) Майкрософт (MSAL) теперь является рекомендуемой библиотекой проверки подлинности для использования с платформа удостоверений Майкрософт. Если вы используете библиотеку проверки подлинности [Azure Active Directory](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), запланируйте переход на MSAL. Дополнительные рекомендации по [переносу приложений в библиотеку проверки подлинности Майкрософт (MSAL)](/azure/active-directory/develop/msal-migration).

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте о [синтаксисе вызова](migrate-azure-ad-graph-request-differences.md) запроса, чтобы начать шаг 1. Просмотр различий в API.
