---
title: Обзор API Microsoft Bookings (предварительная версия)
description: Microsoft Bookings предоставляет онлайн и мобильные приложения, которые делают планирование встреч простым и эффективным для организации, ее пользователей и клиентов.
author: arvindmicrosoft
localization_priority: Priority
ms.prod: bookings
ms.custom: scenarios:getting-started
ms.openlocfilehash: 5dfd34bb7defd6f525a5869221ce2c0215826da6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50432867"
---
# <a name="microsoft-bookings-api-overview-preview"></a>Обзор API Microsoft Bookings (предварительная версия)

Microsoft Bookings — это приложения для браузера и мобильных устройств, упрощающие планирование встреч для небольших компаний и их клиентов. Любая организация, предоставляющая услуги по предварительной записи, например крупные компании, автосервисы, парикмахерские и юридические фирмы, может получить выгоду от управления своими заказами, чтобы высвободить время для более важной задачи развития своего бизнеса. Служба Microsoft Bookings доступна корпоративным организациям и предприятиям, имеющим подписку на Microsoft 365 бизнес премиум.

## <a name="why-integrate-with-microsoft-bookings-using-microsoft-graph"></a>Зачем проводить интеграцию с Microsoft Bookings, используя Microsoft Graph?

### <a name="streamline-appointment-booking"></a>Простое планирование встреч
Предприниматель не должен упускать клиентов из-за того, что не может ответить на звонок или компания закрыта. Клиенты могут [видеть доступные услуги](/graph/api/bookingbusiness-list-services?view=graph-rest-beta) и [записываться](/graph/api/bookingbusiness-post-appointments?view=graph-rest-beta) в любой момент прямо на странице планирования, на Facebook или веб-сайте компании. 

Предприниматели могут подтверждать записи в мобильном или интернет-приложении, лично или по телефону. Они могут [перенести](/graph/api/bookingappointment-update?view=graph-rest-beta) или [отменить](/graph/api/bookingappointment-cancel?view=graph-rest-beta) бронь, а также [переназначить](/graph/api/bookingappointment-update?view=graph-rest-beta) ее, указав другого доступного сотрудника. 

### <a name="reduce-no-shows-and-increase-productivity-of-the-staff"></a>Сокращение количества неявок и увеличение эффективности сотрудников
Предприниматели могут указать [политики планирования](/graph/api/resources/bookingschedulingpolicy?view=graph-rest-beta), включающие минимальные уведомления о резервировании и отмене, а клиенты могут планировать и переносить встречи самостоятельно. Автоматические подтверждения встреч и напоминания позволяют сократить количество неявок и эффективнее использовать рабочее время. 

### <a name="manage-customer-information-and-relationships-from-anywhere"></a>Управление сведениями о клиентах и соответствующих отношениях с любого устройства
При добавлении встречи автоматически проверяется, указан ли человек в [списке клиентов](/graph/api/bookingbusiness-list-customers?view=graph-rest-beta), и при необходимости [добавляются](/graph/api/bookingbusiness-post-customers?view=graph-rest-beta) его имя и электронный адрес в этот список. Благодаря этому предприниматели могут с легкостью оставаться на связи с клиентами и периодически отправлять им информационные бюллетени и другие рекламные материалы.

### <a name="integrate-with-productivity-and-team-collaboration-services-in-microsoft-graph"></a>Интеграция со службами, повышающими эффективность работы и сотрудничества, в Microsoft Graph
Используя единую конечную точку REST Microsoft Graph, вы можете получить доступ к API Bookings и [интегрировать лучшее из Microsoft 365](overview-major-services.md) для поддержки многофункциональных сценариев. Например, с помощью [Excel](excel-concept-overview.md#generate-reports-and-analyze-results) вы можете отслеживать и анализировать финансовые данные компании, создавать профессиональные отчеты, а с помощью [SharePoint](sharepoint-concept-overview.md) или [Microsoft Teams](teams-concept-overview.md) — повысить эффективность сотрудничества команд.

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

См. статью [API Microsoft Bookings в бета-версии Microsoft Graph](/graph/api/resources/booking-api-overview?view=graph-rest-beta).


## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Microsoft Bookings](https://support.office.com/article/Publish-your-business-calendar-online-with-Microsoft-Bookings-47403d64-a067-4754-9ae9-00157244c27d) и другие [бизнес-приложения Microsoft 365](https://support.office.com/article/manage-your-business-apps-in-the-business-center-47eca808-cf96-42ba-83e8-55daf18e49dc?ui=en-US&rs=en-US&ad=US).
- [Использование API Bookings](/graph/api/resources/booking-api-overview?view=graph-rest-beta) в Microsoft Graph.

