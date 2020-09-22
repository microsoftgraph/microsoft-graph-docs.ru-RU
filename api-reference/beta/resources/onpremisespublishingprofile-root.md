---
title: Локальные профили публикации
description: Различные службы Azure (например, сквозная проверка подлинности подключения Azure Active Directory, подготовка пользователей рабочего дня к Azure AD) обеспечивают условный доступ к различным локальным ресурсам извне корпоративной сети.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1e2403d057cc399279ec8ac3084e67798092705b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998658"
---
# <a name="on-premises-publishing-profiles"></a>Локальные профили публикации

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Различные службы Azure (например, [сквозная проверка подлинности](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta)подключения Azure Active Directory, подключение [рабочего дня к пользователям Azure AD](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)и [прокси приложения](https://aka.ms/whyappproxy)  — предоставление доступа к различным локальным ресурсам извне корпоративной сети). [Локальные агенты](onpremisesagent.md) (или [соединители](connector.md) для прокси-сервера приложения), установленные администратором клиента, можно настроить на маршрутизацию запросов к определенному [опубликованному ресурсу](publishedresource.md).
[Группы агентов](onpremisesagentgroup.md) (или [группы соединителей](connectorgroup.md) для прокси приложения) позволяют администратору клиента назначать определенные агенты для обслуживания определенных опубликованных локальных ресурсов. Администраторы клиентов могут объединить несколько агентов в группу, а затем назначить каждый опубликованный ресурс группе. Весь набор сущностей одного локального типа публикации представлен [онпремисеспублишингпрофиле](onpremisespublishingprofile.md).

Администратор клиента может настраивать для каждого **онпремисеспублишингпрофиле** [периода времени](updatewindow.md) , в течение которого агенты могут получать обновления или закладывать обновления для агентов. [Конфигурация обновления](hybridagentupdaterconfiguration.md) , указанная для **онпремисеспублишингпрофиле** , относится ко всем агентам в **онпремисеспублишингпрофиле**.

Руководство по настройке прокси приложения приведено в разделе [Автоматизация настройки прокси приложения с помощью API Microsoft Graph](https://docs.microsoft.com/graph/application-proxy-configure-api).

## <a name="see-also"></a>См. также

- [Локальный агент](onpremisesagent.md)
- [Локальная группа агентов](onpremisesagentgroup.md)
- [Профиль локальной публикации](onpremisespublishingprofile.md)
- [Опубликованный ресурс](publishedresource.md)
- [Connector](connector.md)
- [Группа соединителей](connectorgroup.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


