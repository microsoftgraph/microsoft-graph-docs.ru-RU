---
title: Использование API Microsoft Bookings в Microsoft Graph
description: Microsoft Bookings позволяет крупным организациям и владельцам малого бизнеса управлять резервированиями и сведениями клиентов с минимальной настройкой.
ms.localizationpriority: high
author: arvindmicrosoft
ms.prod: bookings
doc_type: conceptualPageType
ms.openlocfilehash: d3b1209d4ae7414233de44c8c51d62fd7bea751e
ms.sourcegitcommit: 9759b647acfbed99d5675a6f512aaa33932a723f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/23/2021
ms.locfileid: "61604212"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a>Использование API Microsoft Bookings в Microsoft Graph

Microsoft Bookings позволяет крупным организациям и владельцам малого бизнеса управлять резервированиями и сведениями клиентов с минимальной настройкой. Владелец бизнеса можно создать одну или несколько компаний, каждая из которых предлагает набор услуг. Владелец может настроить сотрудников и указать услуги, оказываемые каждым из них. Клиент может зарезервировать встречу для определенной услуги в этой компании в сетевом или мобильном приложении. Приложение Bookings обеспечивает обновление времени встречи для компании, сотрудников и соответствующих клиентов.

На программном уровне объект [bookingBusiness](bookingbusiness.md) в API Bookings включает указанные ниже объекты:

- один или несколько объектов [bookingStaffMember](bookingstaffmember.md);
- один или несколько объектов [bookingService](bookingservice.md);
- набор экземпляров [bookingAppointment](bookingappointment.md);
- набор объектов [bookingCustomer](bookingcustomer.md).

## <a name="using-the-bookings-rest-api"></a>Использование REST API Bookings

Выполните указанные ниже действия перед первым резервированием встреч клиента с компанией. Убедитесь, что предоставлены подходящие [маркеры доступа](/graph/auth/auth-concepts#access-tokens) для соответствующих операций.

1. Убедитесь, что у компании есть подписка на [Microsoft 365 бизнес премиум](https://products.office.com/en-us/business/office-365-business-premium).
2. Создайте новый объект **bookingBusiness**, отправив операцию POST в набор объектов. Как минимум, следует указать имя новой компании, отображаемое для клиентов:
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
Используйте свойство **id** нового объекта **bookingBusiness**, возвращенного в отклике POST, чтобы продолжить [настройку](../api/bookingbusiness-update.md) бизнес-параметров и добавить сотрудников и услуги для компании.

3. Добавьте отдельных сотрудников для компании:
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/{id}/staffMembers
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Dana Swope",
    "emailAddress": "danas@contoso.com",
    "role": "externalGuest"
}
```
4. Определите каждую услугу, предлагаемую компанией:
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. Опубликуйте страницу расписания для компании, чтобы у клиентов и бизнес-операторов была возможность начать резервирование встреч:
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

Как правило, можно указать список всех компаний для резервирования в клиенте Microsoft 365:
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a>Основные варианты использования

В таблице ниже перечислены распространенные операции для бизнеса в API Bookings.

| Варианты использования        | Ресурсы REST | См. также |
|:---------------|:--------|:----------|
| Создание, получение, обновление или удаление компании | [bookingBusiness](bookingbusiness.md) | [Методы ресурса bookingBusiness](bookingbusiness.md#methods) |
| Обновление политики планирования | [bookingSchedulingPolicy](bookingschedulingpolicy.md) | [Обновление bookingBusiness](../api/bookingbusiness-update.md) |
| Добавление, получение, обновление или удаление сотрудников | [bookingStaffMember](bookingstaffmember.md) | [Методы ресурса bookingStaffMember](bookingstaffmember.md#methods)  |
| Добавление, получение, обновление или удаление услуг | [bookingService](bookingservice.md) | [Методы ресурса bookingService](bookingservice.md#methods)  |
| Добавление, получение, обновление или удаление настраиваемых вопросов | [bookingCustomQuestion](bookingcustomquestion.md) | [Методы bookingCustomQuestion](bookingcustomquestion.md#methods)  |
| Добавление, получение, обновление или удаление пользователей | [bookingCustomer](bookingcustomer.md) | [Методы bookingCustomer](bookingcustomer.md#methods)  |
| Публикация или отмена публикации страницы расписания | [bookingBusiness](bookingbusiness.md) | [publish](../api/bookingbusiness-publish.md) <br> [unpublish](../api/bookingbusiness-unpublish.md) |
| Создание, получение, обновление, удаление или отмена встречи | [bookingAppointment](bookingappointment.md) | [Методы ресурса bookingAppointment](bookingappointment.md#methods)  |
| Получение встреч в диапазоне дат | [bookingBusiness](bookingbusiness.md) | [Представление календаря "Список резервирований"](../api/bookingbusiness-list-calendarview.md) |
| Получение валюты | [bookingCurrency](bookingcurrency.md) | [Методы ресурса bookingCurrency](bookingcurrency.md#methods) |

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="see-also"></a>См. также

- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/partners).
- Узнайте, как выбрать [разрешения](/graph/permissions-reference) в Microsoft Graph.


