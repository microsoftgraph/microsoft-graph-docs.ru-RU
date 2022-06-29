---
title: Управление несколькими клиентами с помощью Microsoft 365 Lighthouse API
description: Microsoft 365 Lighthouse Microsoft Graph помогает msPs удаленно управлять устройствами, данными и пользователями для клиентов, использующих Microsoft 365 бизнес премиум.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
ms.openlocfilehash: 8a59b310ef6ae5b5d50b423fc013b25bede133f4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440693"
---
# <a name="manage-multiple-customer-tenants-using-the-microsoft-365-lighthouse-api"></a>Управление несколькими клиентами с помощью Microsoft 365 Lighthouse API

Microsoft 365 Lighthouse — это портал администрирования, позволяющий управляемым поставщикам услуг удаленно управлять несколькими клиентами. Она помогает msPs защищать устройства, данные и пользователей в большом масштабе и управлять ими для клиентов малого и среднего бизнеса (SMB), использующих Microsoft 365 бизнес премиум.

Microsoft 365 Lighthouse помогает msPs упростить подключение Microsoft 365 бизнес премиум клиентов. Он предоставляет поставщику услуг MSP удобство мультитенантных представлений во всех клиентских средах клиента. Он может рекомендовать базовые конфигурации безопасности, адаптированные для клиентов SMB MSP. Используя Microsoft 365 Lighthouse, msPs может масштабировать управление клиентами клиентов, сосредоточиться на наиболее важных, быстро находить и исследовать риски, а также принимать меры для обеспечения работоспособности и безопасности клиентов.

> [!NOTE]  
> Эта документация предназначена для Microsoft 365 Lighthouse API, доступного в _Microsoft Graph_. Аналогичное предложение, Azure Lighthouse, помогает поставщикам услуг предоставлять управляемые службы для служб Azure с помощью комплексных и надежных средств управления, встроенных в _платформу Azure_ . Дополнительные сведения см. [в статье "Что такое Azure Lighthouse"](/azure/lighthouse/overview).

## <a name="why-integrate-with-microsoft-365-lighthouse"></a>Зачем выполнять интеграцию с Microsoft 365 Lighthouse?

Как MSP вы можете использовать API Microsoft 365 Lighthouse в Microsoft Graph, чтобы получить представление об обнаруженных рисках и принять меры для перевода клиентов в работоспособное и безопасное состояние.

### <a name="devices"></a>Устройства

API Lighthouse можно использовать для выполнения следующих задач устройства:

- [Проанализируйте тенденции соответствия устройств](/graph/api/resources/managedtenants-manageddevicecompliancetrend?view=graph-rest-beta&preserve-view=true), чтобы лучше понять, как соответствие устройств со временем развивается для ваших клиентов.
- Сведения о [политиках соответствия](/graph/api/resources/managedtenants-manageddevicecompliance) устройств, созданных для ваших клиентов, и о состоянии политик.

### <a name="threat-management"></a>Управление угрозами

API Lighthouse можно использовать для выполнения следующих задач по управлению угрозами:

- Получите представление о состоянии вредоносных программ [, которые](/graph/api/resources/managedtenants-windowsdevicemalwarestate) присутствуют на устройствах Windows, зарегистрированных для управления клиентами.
- Просмотрите [состояние защиты для](/graph/api/resources/managedtenants-windowsprotectionstate?view=graph-rest-beta&preserve-view=true) устройств Windows, зарегистрированных для управления клиентами, чтобы убедиться, что Защитник Windows находятся в работоспособном состоянии.

### <a name="users"></a>Пользователи

API Lighthouse можно использовать для выполнения следующих пользовательских задач:

- [Обнаруживать пользователей, которые могут быть](/graph/api/resources/riskyuser) рискованными, в разных клиентах.
- [Просмотрите сводку регистрации](/graph/api/resources/managedtenants-credentialuserregistrationssummary?view=graph-rest-beta&preserve-view=true) пользователей учетных данных, чтобы понять, какие пользователи в ваших клиентах зарегистрировались для многофакторной проверки подлинности и самостоятельного сброса пароля.

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

См[. Microsoft 365 Lighthouse API в Microsoft Graph (предварительная версия)](/graph/api/resources/managedtenants-managedtenant?view=graph-rest-beta&preserve-view=true).

> [!NOTE]
> API Microsoft 365 Lighthouse определяется в подименю OData. `microsoft.graph.managedTenants`


## <a name="next-steps"></a>Дальнейшие действия

- Дополнительные [сведения о Microsoft 365 Lighthouse](/microsoft-365/lighthouse/m365-lighthouse-overview?view=o365-worldwide&preserve-view=true) портале.
- Узнайте о [последних новых возможностях и обновлениях](/graph/whats-new-overview) API Lighthouse.
- Изучите [примеры](https://developer.microsoft.com/graph/graph/examples), чтобы получить более четкое представление об использовании Microsoft Graph.
