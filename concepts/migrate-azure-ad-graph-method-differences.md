---
title: Различия в методах между Azure AD и Microsoft Graph
description: Описываются различия методов между API Graph Azure Active Directory (Azure AD) и API Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 00649e4f55a8bfcfd5354d2a75793447e3686109
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38656531"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Различия в методах между Azure AD и Microsoft Graph

Эта статья входит в *Шаг 1: Ознакомьтесь с различиями* в API [процесса переноса приложений](migrate-azure-ad-graph-planning-checklist.md).

Кроме того, изменилось несколько методов Azure AD Graph.  Если метод **не** отображается в этом списке, он уже доступен в [версии 1.0](/graph/api/overview?view=graph-rest-1.0) для Microsoft Graph, в котором используется то же имя, что и в Azure AD Graph.

|Azure AD Graph <br>метод (v 1.6) |Microsoft Graph<br>(ресурс/метод)|Примечания|
|---|---|---|
| жетаваилабликстенсионпропертиес | бета-версия _недоступна_ <br> Версия 1.0 — _недоступна_ |  |
| жетобжектсбйобжектид | бета&nbsp;-&nbsp;-версия каталога/жетбидс <br> v 1.0-Directory/Жетбидс | |
| invalidateAllRefreshTokens | бета-Ревокесигнинсессионс <br> Версия 1.0 — Ревокесигнинсессионс | |
| исмембероф | бета-версия _не запланирована_ <br> v 1.0 — _не запланировано_ | Вместо этого используйте Чеккмемберграупс. |
| restore | &nbsp;-&nbsp;восстановление&nbsp;бета-версии (&nbsp;приложения,&nbsp;пользователи&nbsp;и группы)<br> &nbsp;-&nbsp;восстановление&nbsp;версии 1.0 (пользователи&nbsp;и&nbsp;группы) | Вы также можете просматривать удаленные приложения, пользователей и группы, а также окончательно удалять их. |

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте, как [анализировать различия API](migrate-azure-ad-graph-audit-api-use.md) в приложении между Azure AD Graph и Microsoft Graph.
- Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .
- Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .
