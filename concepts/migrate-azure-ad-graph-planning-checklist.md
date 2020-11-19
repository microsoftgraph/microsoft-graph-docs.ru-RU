---
title: Контрольный список планирования миграции приложений
description: Контрольный список для переноса приложений из Azure AD Graph в Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: d6a5fc83717c2facbbb016cbbc621d6d1bb36dc0
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352405"
---
# <a name="app-migration-planning-checklist"></a>Контрольный список планирования миграции приложений

> [!Important]
> API Graph Azure AD теперь устарел. Мы будем продолжать предоставлять техническую поддержку и обновления для системы безопасности, но не будут предоставлять обновления компонентов.
> Начиная с 30 июня 2022 г. мы завершаем поддержку Azure AD Graph и больше не будут предоставлять техническую поддержку или обновления для системы безопасности. Приложения, использующие Azure AD Graph после этого, больше не будут получать ответы от конечной точки Azure AD Graph.

Используйте следующий контрольный список для планирования миграции.

## <a name="step-1-review-the-differences-between-the-apis"></a>Шаг 1: Ознакомьтесь с различиями между API

Во многих отношениях Microsoft Graph аналогичен более ранней версии Azure AD Graph. Во многих случаях просто измените имя и версию службы конечных точек в коде, и все должно продолжать работу.

Тем не менее, существуют различия. Изменены некоторые ресурсы, свойства, методы и основные возможности.

В частности, ищите различия в следующих областях:

- [Синтаксис запроса на вызов](migrate-azure-ad-graph-request-differences.md) между двумя службами
- [Различия в функциях](migrate-azure-ad-graph-feature-differences.md), такие как расширения каталогов, пакетная обработка, разностные запросы и т. д.
- [Имена ресурсов сущностей](migrate-azure-ad-graph-resource-differences.md) и их типы
- [Свойства](migrate-azure-ad-graph-property-differences.md) объектов Request и Response
- [Методы](migrate-azure-ad-graph-method-differences.md), включая параметры и типы

## <a name="step-2-examine-api-use"></a>Шаг 2: Проверка использования API

[Изучите API](migrate-azure-ad-graph-audit-api-use.md) , используемые вашим приложением, необходимые разрешения и сравните со списком известных отличий.  

Убедитесь, что нужные API-интерфейсы, как правило, доступны в Microsoft Graph версии 1.0, и что эти API работают одинаковым образом.

В некоторых случаях новые возможности и функции предназначены для замены более ранних подходов.

Используйте [проводник Graph](https://aka.ms/ge) для экспериментов с новыми вызовами и разработки новых подходов. Для достижения лучших результатов Войдите в систему, используя учетные данные тестового пользователя в тестовом клиенте, чтобы увидеть, что API выполняет над важными наборами данных.

## <a name="step-3-review-app-details"></a>Шаг 3: Просмотр сведений о приложении

- Изменения регистрации и согласия [приложения](migrate-azure-ad-graph-app-registration.md) (не должно быть None).
- Получение маркеров и [библиотек проверки подлинности](migrate-azure-ad-graph-authentication-library.md).
- Для приложений .NET используйте [клиентские библиотеки](migrate-azure-ad-graph-client-libraries.md).

## <a name="step-4-deploy-test-and-extend-your-app"></a>Шаг 4: развертывание, тестирование и расширение приложения

Прежде чем обновлять приложение для всех пользователей, убедитесь, что вы тщательно протестируете и разработайте перед развертыванием вашей аудитории клиентов.

Теперь, когда вы переключились на Microsoft Graph, вы не сможете упростить разблокировку многих дополнительных наборов данных и функций, которые теперь доступны вам. Вы можете получить сведения о возможных возможностях, изучив некоторые [основные службы и функции Microsoft Graph](/graph/overview-major-services).

Если вы используете [библиотеку проверки подлинности Active Directory](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), рассмотрите возможность переключения на [библиотеку проверки подлинности Microsoft](/azure/active-directory/develop/reference-v2-libraries) (MSAL).

## <a name="next-steps"></a>Дальнейшие действия

- Сведения о [синтаксисе запроса request](migrate-azure-ad-graph-request-differences.md) для начала действия 1: обзор различий API.