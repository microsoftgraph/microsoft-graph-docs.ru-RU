---
title: Различия в методах между Azure AD и Microsoft Graph
description: Описываются различия методов между API Graph Azure Active Directory (Azure AD) и API Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8179dcc797086e26d4351d17d7a5675b5d012722
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863721"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Различия в методах между Azure AD и Microsoft Graph

Эта статья входит в *Шаг 1: Ознакомьтесь с различиями* в API [процесса переноса приложений](migrate-azure-ad-graph-planning-checklist.md).

Кроме того, изменилось несколько методов Azure AD Graph.  Если метод **не** отображается в этом списке, он уже доступен в [версии 1.0](/graph/api/overview?view=graph-rest-1.0) для Microsoft Graph, в котором используется то же имя, что и в Azure AD Graph.

|Azure AD Graph <br>метод (v 1.6) |Microsoft Graph<br>(ресурс/метод)|Комментарии|
|---|---|---|
| жетаваилабликстенсионпропертиес | бета-версия &nbsp; - &nbsp; _недоступна_ <br> Версия 1.0 &nbsp; - &nbsp; _недоступна_ |  |
| жетобжектсбйобжектид | бета-версия &nbsp; - &nbsp; [директорйобжектс/жетбидс](/graph/api/directoryobject-getbyids?view=graph-rest-beta) <br> Версия 1.0 &nbsp; - &nbsp; [директорйобжектс/жетбидс](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) | |
| invalidateAllRefreshTokens | бета- &nbsp; - &nbsp; [ревокесигнинсессионс](/graph/api/user-revokesigninsessions?view=graph-rest-beta) <br> Версия 1.0 &nbsp; - &nbsp; [ревокесигнинсессионс](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) | |
| исмембероф | бета-версия &nbsp; - &nbsp; _не запланирована_ <br> Версия 1.0 &nbsp; - &nbsp; _не запланирована_ | Вместо этого используйте Чеккмемберграупс. |
| restore | Восстановление бета-версии &nbsp; - &nbsp; [ &nbsp; (приложения, &nbsp; Пользователи &nbsp; и &nbsp; группы)](/graph/api/directory-deleteditems-restore?view=graph-rest-beta)<br> восстановление версии 1.0 &nbsp; - &nbsp; [ &nbsp; (приложения, &nbsp; Пользователи &nbsp; и &nbsp; группы)](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0) | Вы также можете просматривать удаленные приложения, пользователей и группы, а также окончательно удалять их. |

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте, как [анализировать различия API](migrate-azure-ad-graph-audit-api-use.md) в приложении между Azure AD Graph и Microsoft Graph.
- Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .
- Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .
