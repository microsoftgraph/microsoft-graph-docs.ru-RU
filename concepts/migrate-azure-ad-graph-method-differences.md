---
title: Различия метода между Azure AD и Microsoft Graph
description: Описывает различия методов между API графа Azure Active Directory (Azure AD) и API Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 95acfccc83fee798d5b06d78bbf10f02c128a640
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760674"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Различия метода между Azure AD и Microsoft Graph

Эта статья является *частью шага 1: просмотрите различия API* процесса переноса [приложений.](migrate-azure-ad-graph-planning-checklist.md)

Несколько методов Azure AD Graph также изменились.  Если метод  не отображается в этом списке, он уже доступен в [версии v1.0](/graph/api/overview?view=graph-rest-1.0) Microsoft Graph с точно таким же именем, как в Azure AD Graph.

|Azure AD Graph <br>(v1.6) метод |Microsoft Graph<br>(ресурс/метод)|Комментарии|
|---|---|---|
| getAvailableExtensionProperties | &nbsp; - &nbsp; _бета-версия недоступна_ <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties?view=graph-rest-1.0) |  |
| getObjectsByObjectId | beta &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) | |
| invalidateAllRefreshTokens | &nbsp; - &nbsp; [бета-revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) | |
| isMemberOf | &nbsp; - &nbsp; _бета-версия не запланирована_ <br> v1.0 &nbsp; - &nbsp; _Не планируется_ | Вместо [этого используйте checkMemberGroups.](/graph/api/user-checkmembergroups?view=graph-rest-1.0) |
| restore | восстановление &nbsp; - &nbsp; [ &nbsp; бета-версии (приложения, &nbsp; пользователи &nbsp; и &nbsp; группы)](/graph/api/directory-deleteditems-restore?view=graph-rest-beta)<br> восстановление v1.0 &nbsp; - &nbsp; [ &nbsp; (приложения, &nbsp; пользователи &nbsp; и &nbsp; группы)](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0) | Вы также можете просматривать удаленные приложения, пользователей и группы и удалять их навсегда. |

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте, как [изучить различия API](migrate-azure-ad-graph-audit-api-use.md) в приложении между Azure AD Graph и Microsoft graph.
- Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.
