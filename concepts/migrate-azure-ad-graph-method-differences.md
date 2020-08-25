---
title: Различия в методах между Azure AD и Microsoft Graph
description: Описываются различия методов между API Graph Azure Active Directory (Azure AD) и API Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 577167a306c98ba51c1ba13d9240570df202f083
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872917"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Различия в методах между Azure AD и Microsoft Graph

Эта статья входит в *Шаг 1: Ознакомьтесь с различиями* в API [процесса переноса приложений](migrate-azure-ad-graph-planning-checklist.md).

Кроме того, изменилось несколько методов Azure AD Graph.  Если метод **не** отображается в этом списке, он уже доступен в [версии 1.0](/graph/api/overview?view=graph-rest-1.0) для Microsoft Graph, в котором используется то же имя, что и в Azure AD Graph.

|Azure AD Graph <br>метод (v 1.6) |Microsoft Graph<br>(ресурс/метод)|Комментарии|
|---|---|---|
| жетаваилабликстенсионпропертиес | бета-версия &nbsp; - &nbsp; _недоступна_ <br> Версия 1.0 &nbsp; - &nbsp; [директорйобжектс/жетаваилабликстенсионпропертиес](/graph/api/directoryobject-getavailableextensionproperties?view=graph-rest-1.0) |  |
| жетобжектсбйобжектид | бета-версия &nbsp; - &nbsp; [директорйобжектс/жетбидс](/graph/api/directoryobject-getbyids?view=graph-rest-beta) <br> Версия 1.0 &nbsp; - &nbsp; [директорйобжектс/жетбидс](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) | |
| invalidateAllRefreshTokens | бета- &nbsp; - &nbsp; [ревокесигнинсессионс](/graph/api/user-revokesigninsessions?view=graph-rest-beta) <br> Версия 1.0 &nbsp; - &nbsp; [ревокесигнинсессионс](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) | |
| исмембероф | бета-версия &nbsp; - &nbsp; _не запланирована_ <br> Версия 1.0 &nbsp; - &nbsp; _не запланирована_ | Вместо этого используйте [чеккмемберграупс](/graph/api/user-checkmembergroups?view=graph-rest-1.0) . |
| restore | Восстановление бета-версии &nbsp; - &nbsp; [ &nbsp; (приложения, &nbsp; Пользователи &nbsp; и &nbsp; группы)](/graph/api/directory-deleteditems-restore?view=graph-rest-beta)<br> восстановление версии 1.0 &nbsp; - &nbsp; [ &nbsp; (приложения, &nbsp; Пользователи &nbsp; и &nbsp; группы)](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0) | Вы также можете просматривать удаленные приложения, пользователей и группы, а также окончательно удалять их. |

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте, как [анализировать различия API](migrate-azure-ad-graph-audit-api-use.md) в приложении между Azure AD Graph и Microsoft Graph.
- Снова просмотрите [Контрольный список](migrate-azure-ad-graph-planning-checklist.md) .
