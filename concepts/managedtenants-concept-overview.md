---
title: Microsoft 365 Lighthouse Обзор API
description: Microsoft 365 Lighthouse является порталом администрирования, который помогает управляемым поставщикам услуг (MSP) обеспечивать безопасность устройств, данных и пользователей в масштабе для клиентов малого и среднего бизнеса(SMB), использующих Microsoft 365 бизнес премиум.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
ms.openlocfilehash: 177a2f03fe5ee0e2e7d90ade038dcef1f7d6c3db
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401893"
---
# <a name="overview-for-multi-tenant-management-using-the-microsoft-365-lighthouse-api"></a>Обзор управления несколькими клиентами с Microsoft 365 Lighthouse API

Microsoft 365 Lighthouse является порталом администрирования, который позволяет управляемым поставщикам услуг (MSP) удаленно управлять несколькими клиентами. Это помогает msPs обеспечить безопасность устройств, данных и пользователей в масштабе для клиентов малого и среднего бизнеса (SMB), использующих Microsoft 365 бизнес премиум.

Microsoft 365 Lighthouse помогает msPs упростить процесс Microsoft 365 бизнес премиум клиентов. Он предлагает службе MSP удобство представлений с несколькими клиентами во всех средах клиента. Он может рекомендовать базовые параметры конфигурации безопасности, адаптированные к клиентам SMB MSP. С Microsoft 365 Lighthouse, msPs может масштабировать управление клиентом клиентов, сосредоточиться на наиболее важных, быстро найти и исследовать риски, а также принять меры, чтобы помочь их клиенты клиентов в здоровом и безопасном состоянии.

> [!NOTE]  
> Эта документация о Microsoft 365 Lighthouse API, доступном в _Microsoft Graph._ Аналогичное предложение, Azure Lighthouse, помогает поставщикам услуг предоставлять управляемые службы для служб Azure с помощью комплексного и надежного инструмента управления, встроенного в _платформу Azure._ Дополнительные дополнительные информации см. [в видеоролике What is Azure Lighthouse.](/azure/lighthouse/overview)

## <a name="why-integrate-with-microsoft-365-lighthouse"></a>Зачем интегрироваться с Microsoft 365 Lighthouse?

В качестве MSP вы можете использовать API Microsoft 365 Lighthouse Microsoft Graph, чтобы получить сведения о выявленных рисках и принять меры, чтобы помочь вашим клиентам в здоровом и безопасном состоянии.

### <a name="devices"></a>Устройства

API Маяка можно использовать для выполнения следующих задач устройства:

- Анализ [тенденций соответствия](/graph/api/resources/managedtenants-manageddevicecompliancetrend?view=graph-rest-beta&preserve-view=true) требованиям устройств, чтобы лучше понять, как со временем развивается соответствие требованиям к устройствам для клиентов.
- Поймите, [какие политики](/graph/api/resources/managedtenants-manageddevicecompliance) соответствия требованиям к устройствам были созданы для ваших клиентов, и состояние политик.

### <a name="threat-management"></a>Управление угрозами

API Маяка можно использовать для выполнения следующих задач по управлению угрозами:

- Сведения о состоянии [вредоносных](/graph/api/resources/managedtenants-windowsdevicemalwarestate) программ, которые присутствуют на Windows устройствах, зарегистрированных для управления клиентами.
- Просмотр состояния [защиты](/graph/api/resources/managedtenants-windowsprotectionstate?view=graph-rest-beta&preserve-view=true) для Windows устройств, зарегистрированных для управления в клиентах, чтобы убедиться, что Защитник Windows находятся в нормальном состоянии.

### <a name="users"></a>Пользователи

API Маяка можно использовать для выполнения следующих пользовательских задач:

- Откройте [для себя рискованных пользователей](/graph/api/resources/managedtenants-riskyuser?view=graph-rest-beta&preserve-view=true) в ваших клиентах.
- Просмотреть [сводку](/graph/api/resources/managedtenants-credentialuserregistrationssummary?view=graph-rest-beta&preserve-view=true) регистрации пользователей учетных данных, чтобы понять, какие пользователи в ваших клиентах зарегистрировались для многофакторной проверки подлинности и сброса пароля самообслуживления.

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

См. [Microsoft 365 Lighthouse API в Microsoft Graph (предварительный просмотр).](/graph/api/resources/managedtenants-managedtenant?view=graph-rest-beta&preserve-view=true)

> [!NOTE]
> API Microsoft 365 Lighthouse определяется в поднаемной области OData. `microsoft.graph.managedTenants`


## <a name="next-steps"></a>Дальнейшие действия

- Узнайте больше о [портале Microsoft 365 Lighthouse.](/microsoft-365/lighthouse/m365-lighthouse-overview?view=o365-worldwide&preserve-view=true)
- Узнайте о [последних новых функций](/graph/whats-new-overview) и обновлениях API Маяка.
- Изучите [примеры](https://developer.microsoft.com/graph/graph/examples), чтобы получить более четкое представление об использовании Microsoft Graph.
