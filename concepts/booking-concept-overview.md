---
title: Обзор API Microsoft Bookings
description: Microsoft Bookings — это приложения для браузера и мобильных устройств, предназначенные для удобного и эффективного планирования встреч для организаций, их пользователей и клиентов.
author: arvindmicrosoft
ms.localizationpriority: high
ms.prod: bookings
ms.custom: scenarios:getting-started
ms.openlocfilehash: 3b143969faf7dcc67d4fc07a0ac117d9b020d09e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442164"
---
# <a name="microsoft-bookings-api-overview"></a>Обзор API Microsoft Bookings

Microsoft Bookings — это приложения для браузера и мобильных устройств, предназначенные для удобного и эффективного планирования встреч для коммерческих компаний и их клиентов. Любая организация, предоставляющая услуги по предварительной записи, например крупные компании, автосервисы, парикмахерские и юридические фирмы, может получить выгоду от управления своими заказами, чтобы высвободить время для более важной задачи развития своего бизнеса. Служба Microsoft Bookings доступна корпоративным организациям и предприятиям, имеющим подписку на Microsoft 365 бизнес премиум.

## <a name="why-integrate-with-microsoft-bookings-using-microsoft-graph"></a>Зачем проводить интеграцию с Microsoft Bookings, используя Microsoft Graph?

### <a name="streamline-appointment-booking"></a>Простое планирование встреч
Предприниматель не должен упускать клиентов из-за того, что не может ответить на звонок или компания закрыта. Клиенты могут [видеть доступные услуги](/graph/api/bookingbusiness-list-services) и [записываться](/graph/api/bookingbusiness-post-appointments) в любой момент прямо на странице планирования, на Facebook или веб-сайте компании. 

Предприниматели могут подтверждать записи в мобильном или интернет-приложении, лично или по телефону. Они могут [перенести](/graph/api/bookingappointment-update) или [отменить](/graph/api/bookingappointment-cancel) бронь, а также [переназначить](/graph/api/bookingappointment-update) ее, указав другого доступного сотрудника. 

### <a name="reduce-no-shows-and-increase-productivity-of-the-staff"></a>Сокращение количества неявок и увеличение эффективности сотрудников
Предприниматели могут указать [политики планирования](/graph/api/resources/bookingschedulingpolicy), включающие минимальные уведомления о резервировании и отмене, а клиенты могут планировать и переносить встречи самостоятельно. Автоматические подтверждения встреч и напоминания позволяют сократить количество неявок и эффективнее использовать рабочее время. 

### <a name="manage-customer-information-and-relationships-from-anywhere"></a>Управление сведениями о клиентах и соответствующих отношениях с любого устройства
При добавлении встречи автоматически проверяется, указан ли человек в [списке клиентов](/graph/api/bookingbusiness-list-customers), и при необходимости [добавляются](/graph/api/bookingbusiness-post-customers) его имя и электронный адрес в этот список. Благодаря этому предприниматели могут с легкостью оставаться на связи с клиентами и периодически отправлять им информационные бюллетени и другие рекламные материалы.

### <a name="integrate-with-productivity-and-team-collaboration-services-in-microsoft-graph"></a>Интеграция со службами, повышающими эффективность работы и сотрудничества, в Microsoft Graph
Используя единую конечную точку REST Microsoft Graph, вы можете получить доступ к API Bookings и [интегрировать лучшее из Microsoft 365](overview-major-services.md) для поддержки многофункциональных сценариев. Например, с помощью [Excel](excel-concept-overview.md#generate-reports-and-analyze-results) вы можете отслеживать и анализировать финансовые данные компании, создавать профессиональные отчеты, а с помощью [SharePoint](sharepoint-concept-overview.md) или [Microsoft Teams](teams-concept-overview.md) — повысить эффективность сотрудничества команд.

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы? См. статью [API Microsoft Bookings в версии Microsoft Graph](/graph/api/resources/booking-api-overview).

## <a name="see-also"></a>См. также

- [Microsoft Bookings для Microsoft 365](https://support.office.com/article/Publish-your-business-calendar-online-with-Microsoft-Bookings-47403d64-a067-4754-9ae9-00157244c27d)
- Другие [бизнес-приложения Microsoft 365](https://www.microsoft.com/microsoft-365)