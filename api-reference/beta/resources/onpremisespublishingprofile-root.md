---
title: Локальные профили публикации
description: Различные службы Azure (например, сквозная проверка подлинности подключения Azure Active Directory, подготовка пользователей рабочего дня к Azure AD) обеспечивают условный доступ к различным локальным ресурсам извне корпоративной сети.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ae3b31de8a8d4121c836126c09921ef7574301ce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522209"
---
# <a name="on-premises-publishing-profiles"></a>Локальные профили публикации

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Различные службы Azure (например, сквозная проверка подлинности подключения Azure Active Directory, подготовка пользователей рабочего дня к Azure AD) обеспечивают условный доступ к различным локальным ресурсам извне корпоративной сети. [Локальные агенты](onpremisesagent.md) , установленные администратором клиента, можно настроить для доступа к определенному [опубликованному ресурсу](publishedresource.md)или обработки запросов.
[Группы агентов](onpremisesagentgroup.md) позволяют администратору клиента назначать определенные агенты для обслуживания определенных опубликованных локальных ресурсов. Администраторы клиентов могут объединить несколько агентов в группу, а затем назначить каждый опубликованный ресурс группе. Весь набор сущностей одного локального типа публикации представлен [онпремисеспублишингпрофиле](onpremisespublishingprofile.md).

Администратор клиента может настраивать для каждого **онпремисеспублишингпрофиле** [периода времени](updatewindow.md) , в течение которого агенты могут получать обновления или закладывать обновления для агентов. [Конфигурация обновления](hybridagentupdaterconfiguration.md) , указанная для **онпремисеспублишингпрофиле** , относится ко всем агентам в **онпремисеспублишингпрофиле**.

## <a name="see-also"></a>См. также

- [Локальный агент](onpremisesagent.md)
- [Локальная группа агентов](onpremisesagentgroup.md)
- [Профиль локальной публикации](onpremisespublishingprofile.md)
- [Опубликованный ресурс](publishedresource.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
