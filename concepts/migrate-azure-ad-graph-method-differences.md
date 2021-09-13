---
title: Различия метода между Azure Active Directory (Azure AD) Graph и Microsoft Graph
description: Описывает различия методов между Azure Active Directory (Azure AD) Graph API и API microsoft Graph (REST).
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: fab1da340ca4a7703f2434f0d3a30b8e1b08821d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139095"
---
# <a name="method-differences-between-azure-active-directory-azure-ad-and-microsoft-graph"></a>Различия метода между Azure Active Directory (Azure AD) и Microsoft Graph

Эта статья является *частью шага 1: просмотрите различия API* процесса переноса [приложений.](migrate-azure-ad-graph-planning-checklist.md)

Несколько методов Azure AD Graph также изменились.  Если метод  не отображается в этом списке, он уже доступен в [версии v1.0](/graph/api/overview) Microsoft Graph с точно таким же именем, как в Azure AD Graph.

|Azure AD Graph <br>(v1.6) метод |Microsoft Graph<br>(ресурс/метод)|Комментарии|
|---|---|---|
| getAvailableExtensionProperties | &nbsp; - &nbsp; _бета-версия недоступна_ <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties) |  |
| getObjectsByObjectId | beta &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids) | |
| invalidateAllRefreshTokens | &nbsp; - &nbsp; [бета-revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions) | |
| isMemberOf | &nbsp; - &nbsp; _бета-версия не запланирована_ <br> v1.0 &nbsp; - &nbsp; _Не планируется_ | Вместо [этого используйте checkMemberGroups.](/graph/api/user-checkmembergroups) |
| restore | восстановление &nbsp; - &nbsp; [ &nbsp; бета-версии (приложения, &nbsp; пользователи &nbsp; и &nbsp; группы)](/graph/api/directory-deleteditems-restore?view=graph-rest-beta&preserve-view=true)<br> восстановление v1.0 &nbsp; - &nbsp; [ &nbsp; (приложения, &nbsp; пользователи &nbsp; и &nbsp; группы)](/graph/api/directory-deleteditems-restore) | Вы также можете просматривать удаленные приложения, пользователей и группы и удалять их навсегда. |

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте, как [изучить различия API](migrate-azure-ad-graph-audit-api-use.md) в приложении между azure AD Graph и Microsoft graph.
- Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.
