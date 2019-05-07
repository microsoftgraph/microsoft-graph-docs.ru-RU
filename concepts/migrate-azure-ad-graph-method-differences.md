---
title: Различия в методах между Azure AD и Microsoft Graph
description: Описываются различия методов между API Graph Azure Active Directory (Azure AD) и API Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 35f97a6c24e0b72200dcd4a37b6fba42ad7ce03d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630239"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Различия в методах между Azure AD и Microsoft Graph

Эта статья входит в *Шаг 1: ознакомьтесь* с различиями в API [процесса переноса приложений](migrate-azure-ad-graph-planning-checklist.md).

Кроме того, изменилось несколько методов Azure AD Graph.  Если метод не отображается в этом списке, он уже доступен в [версии 1.0](/graph/api/overview?view=graph-rest-1.0) для Microsoft Graph, в котором используется то же имя, что и в Azure AD Graph.

|Azure AD Graph <br>метод (v 1.6) |Microsoft Graph<br>(ресурс/метод)|Comments|
|---|---|---|
| Жетобжектсбйобжектид | бета&nbsp;-&nbsp;-версия каталога/жетбидс <br> v 1.0-Directory/Жетбидс | |
| restore | &nbsp;-&nbsp;восстановление&nbsp;бета-версии (&nbsp;приложения,&nbsp;пользователи&nbsp;и группы)<br> &nbsp;-&nbsp;восстановление&nbsp;версии 1.0 (пользователи&nbsp;и&nbsp;группы) | Вы также можете просматривать удаленные приложения, пользователей и группы, а также окончательно удалять их. |
| invalidateAllRefreshTokens | бета-Инвалидатесигнинсессионс <br> Версия 1.0 _еще_ недоступна | |
| Жетаваилабликстенсионпропертиес | бета-версия _не запланирована_ <br> v 1.0 — _не запланировано_ | В настоящее время не запланировано; можно повторно посетить на основе запроса. |
| Исмембероф | бета-версия _не запланирована_ <br> v 1.0 — _не запланировано_ | Вместо этого используйте Чеккмемберграупс. |
| Аддкэй | бета-версия _еще_ недоступна <br> Версия 1.0 _еще_ недоступна | Запланировано, но пока недоступно. | 
| Ремовекэй | бета-версия _еще_ недоступна <br> Версия 1.0 _еще_ недоступна | Запланировано, но пока недоступно. | 
| Аддпассворд | бета-Аддпассворд <br> Версия 1.0 _еще_ недоступна | |
| Ремовепассворд | бета-Ремовепассворд <br> Версия 1.0 _еще_ недоступна | |

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте, как [анализировать различия API](migrate-azure-ad-graph-audit-api-use.md) в приложении между Azure AD Graph и Microsoft Graph.
- Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .
- Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .
