---
title: Локальное опубликование профилей
description: Различные службы Azure (например, Azure Active Directory Подключение проверки подлинности passthrough, подготовка рабочих дней для пользователей Azure AD) позволяют получить условный доступ к различным локальному ресурсу из-за пределов корпоративной сети.
ms.localizationpriority: medium
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: b8bb4a485f06ea45d553134668fff241984b2ad8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095525"
---
# <a name="on-premises-publishing-profiles"></a>Локальное опубликование профилей

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Различные службы Azure (например, Azure Active Directory Подключение проверки подлинности [passthrough,](/azure/active-directory/hybrid/how-to-connect-pta)подготовка рабочих [](/azure/active-directory/app-proxy/what-is-application-proxy) дней для пользователей [Azure AD](/azure/active-directory/saas-apps/workday-inbound-tutorial)и прокси-серверы приложений позволяют получать доступ к различным локальному ресурсу из-за пределов корпоративной сети. [Локальное агенты](onpremisesagent.md) (или [соединители](connector.md) для application Proxy), установленные администратором клиента, могут быть настроены для маршрутов запросов на определенный [опубликованный ресурс.](publishedresource.md)
[Группы агентов](onpremisesagentgroup.md) [(или](connectorgroup.md) соединители группы для application Proxy) позволяют администратору клиента назначать определенных агентов для обслуживания определенных опубликованных локально ресурсов. Администраторы клиента могут сгруппить несколько агентов вместе, а затем назначить каждый опубликованный ресурс группе. Весь набор сущностями одного и того же локального типа публикации представлен [onPremisesPublishingProfile.](onpremisespublishingprofile.md)

Администратор клиента может настроить для каждого **onPremisesPublishingProfile** время, в течение которого агенты могут получать обновления или откладывать обновления агентам. [](updatewindow.md) Конфигурация [обновителей,](hybridagentupdaterconfiguration.md) заданная для **onPremisesPublishingProfile,** применима ко всем агентам в **этом onPremisesPublishingProfile.**

Руководство по настройке прокси-сервера приложений см. в руководстве [Automate the configuration of Application Proxy using the Microsoft Graph API.](/graph/application-proxy-configure-api)

## <a name="see-also"></a>См. также

- [Агент локального](onpremisesagent.md)
- [Группа локального агента](onpremisesagentgroup.md)
- [Профиль локальной публикации](onpremisespublishingprofile.md)
- [Опубликованный ресурс](publishedresource.md)
- [Connector](connector.md)
- [Группа Connector](connectorgroup.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->