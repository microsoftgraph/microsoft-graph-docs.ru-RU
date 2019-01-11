---
title: Использование Microsoft резервирования API в Microsoft Graph
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Priority
ms.openlocfilehash: def9260654baafe1953d629265c4b76a2afd2748
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845537"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a>Использование Microsoft резервирования API в Microsoft Graph

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.
 
Microsoft резервирования позволяет управлять резервирования клиента и данных с помощью минимальной установки владельцев для малого бизнеса. Владелец business можно создать один или несколько организаций, с каждой бизнеса, предоставляющая набор служб. Владелец можно настроить персонал и укажите службы, которые выполняет каждый сотрудник. В этой организации в приложении online или мобильного клиента можно книги встречи для определенной службы. Резервирования гарантирует, что, время встречи актуальность для бизнеса, сотрудниками и клиентами участвующие.

Программным способом, [bookingBusiness](bookingbusiness.md) в интерфейсе API резервирования состоит из следующих объектов:
 
- Один или несколько объектов [bookingStaffMember](bookingstaffmember.md)
- Один или несколько объектов [bookingService](bookingservice.md)
- Набор экземпляров [bookingAppointment](bookingappointment.md)
- Набор объектов [bookingCustomer](bookingcustomer.md)

## <a name="using-the-bookings-rest-api"></a>С помощью API-Интерфейс REST резервирования

Познакомьтесь с помощью следующих действий перед резервирования встречи для бизнеса в первый раз. Убедитесь, что соответствующие [маркеры доступа](/graph/auth-overview) обеспечения соответствующие операции.

1. Убедитесь в том, что подписка на [Office 365 бизнеса расширенный](https://products.office.com/en-us/business/office-365-business-premium) для бизнеса.
2. Создание нового **bookingBusiness** , отправив операция POST набора сущностей. Как минимум необходимо указать имя для нового предприятия, которое клиенты будут видеть:<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
Свойство **id** нового **bookingBusiness** , возвращаемого в ответе POST для продолжения [Настройка](../api/bookingbusiness-update.md) параметров business и добавьте персонал и службы для бизнеса.

3. Добавление отдельных сотрудников для бизнеса:<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Dana Swope",
    "emailAddress": "danas@contoso.com",
    "role": "externalGuest"
}
```
4. Определение каждой службы, предлагаемыми бизнеса:<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. Опубликуйте страницу планирования для бизнеса, чтобы позволить клиентам и операторы business начать назначения встреч:<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

Как правило чтобы получить список всех резервирование бизнеса в Office 365 клиентов:<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a>Основные сценарии выполнения 

В следующей таблице перечислены типичные операции для бизнеса в API резервирования.

| Варианты использования        | Ресурсы REST | См. также |
|:---------------|:--------|:----------|
| Создание, получение, обновление и удаление предприятие | [bookingBusiness](bookingbusiness.md) | [Методы bookingBusiness](bookingbusiness.md#methods) |
| Обновление политики планирования | [bookingSchedulingPolicy](bookingschedulingpolicy.md) | [Обновление bookingBusiness](../api/bookingbusiness-update.md) |
| Добавление, получение, обновление и удаление сотрудников | [bookingStaffMember](bookingstaffmember.md) | [Методы bookingStaffMember](bookingstaffmember.md#methods)  |
| Добавление, получение, обновление и удаление служб | [bookingService](bookingservice.md) | [Методы bookingService](bookingservice.md#methods)  |
| Публикации или отмены публикации планирования страницы | [bookingBusiness](bookingbusiness.md) | [Публикация](../api/bookingbusiness-publish.md) <br> [Отмена публикации](../api/bookingbusiness-unpublish.md) |
| Создание, получение, обновление, удаление или Отмена встречи | [bookingAppointment](bookingappointment.md) | [Методы bookingAppointment](bookingappointment.md#methods)  |
| Получение встреч в диапазон дат | [bookingBusiness](bookingbusiness.md) | [Список резервирования представления календаря](../api/bookingbusiness-list-calendarview.md) |
| Получение валюты | [bookingCurrency](bookingcurrency.md) | [Методы bookingCurrency](bookingcurrency.md#methods) |


## <a name="see-also"></a>См. также

- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
- В разделе [как партнеров используется Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).
- Узнайте, как выбрать [разрешения](/graph/permissions-reference) в Microsoft Graph.
