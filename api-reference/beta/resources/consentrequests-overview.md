---
title: Запросы на согласие Azure Active Directory
description: Используйте Azure AD согласия для управления рабочим процессом запроса для пользователей, которые пытаются получить доступ к приложениям, которым требуется согласие администратора.
ms.localizationpriority: medium
author: psignoret
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: b3e5832a46277412ddfb27081ffd5044b1053acb
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437893"
---
# <a name="azure-active-directory-consent-requests"></a>Запросы на согласие Azure Active Directory

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [GDPR-related-guidance](../../includes/gdpr-msgraph-export-note.md)]

Запросы согласия Azure Active Directory (Azure AD) помогают управлять рабочим процессом запроса для пользователей, пытающихся получить доступ к приложениям, которым требуется утверждение администратора.

Чтобы разрешить пользователям запрашивать доступ или согласие администратора для приложений, которым не разрешено предоставлять согласие для себя, сначала включите рабочий процесс запроса согласия. 

>[!NOTE]
>Текущие API ограничены настройкой рабочего процесса и чтением списка запросов. В настоящее время нет доступных методов для программного утверждения или отклонения запроса. Однако содержимое запроса можно использовать для повторного создания URL-адреса, который можно использовать для предоставления согласия администратора и утверждения запроса.

К типам ресурсов запроса согласия относятся:

* [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md): указывает политику, с помощью которой запросы на согласие приложения можно создавать и управлять для всего клиента. Существует один **adminConsentRequestPolicy для** каждого клиента.
* [appConsentRequest](../resources/appconsentrequest.md): запрос, представляющий коллекцию **объектов userConsentRequests** для конкретного приложения.
* [userConsentRequest](../resources/userconsentrequest.md): запрос, созданный пользователем для использования приложения, требующее согласия администратора для доступа.
* [appConsentRequestScope](../resources/appconsentrequestscope.md): ресурс, содержащий сведения о динамических областях разрешений, запрашиваемых для приложения.  

## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами запроса согласия.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
|[Получение adminConsentRequestPolicy](../api/adminconsentrequestpolicy-get.md) | [Коллекция adminConsentRequestPolicy](adminconsentrequestpolicy.md) | Чтение свойств [adminConsentRequestPolicy](adminconsentrequestpolicy.md). |
|[Обновление adminConsentRequestPolicy](../api/adminconsentrequestpolicy-update.md) | [Коллекция adminConsentRequestPolicy](adminconsentrequestpolicy.md) | Задайте конфигурации [для adminConsentRequestPolicy](adminconsentrequestpolicy.md). |
|[Перечисление объектов appConsentRequests ](../api/appconsentapprovalroute-list-appconsentrequests.md) | [Коллекция appConsentRequest](appconsentrequest.md) | Получение коллекции объектов [appConsentRequest](appconsentrequest.md) и их свойств. |
|[Получение appConsentRequest ](../api/appconsentrequest-get.md) | [Коллекция appConsentRequest](appconsentrequest.md) | Чтение объекта [appConsentRequest](appconsentrequest.md) . |
|[appConsentRequests: filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md) | [Коллекция appConsentRequest](../resources/appconsentrequest.md) | Прочитайте свойства объектов [appConsentRequest](../resources/appconsentrequest.md) , для которых текущий пользователь является рецензентом и состояние запроса согласия пользователя `InProgress`. |
|[Получение объекта userConsentRequest ](../api/userconsentrequest-get.md) | [Коллекция userConsentRequest](userconsentrequest.md) | Чтение объекта [userConsentRequest](userconsentrequest.md) для [объекта appConsentRequest](appconsentrequest.md). |
|[Перечисление объектов userConsentRequests ](../api/appconsentrequest-list-userconsentrequests.md) | [Коллекция userConsentRequest](userconsentrequest.md) | Получение коллекции объектов [userConsentRequest](userconsentrequest.md) для [объекта appConsentRequest](appconsentrequest.md). |
|[userConsentRequest: filterByCurrentUser](../api/userconsentrequest-filterByCurrentUser.md) | [Коллекция appConsentRequests](../resources/userconsentrequest.md) | Чтение свойств объектов [userConsentRequest](../resources/userconsentrequest.md) для [объекта appConsentRequest](appconsentrequest.md) , для которого текущий пользователь является рецензентом. |

## <a name="role-and-delegated-permission-authorization-checks"></a>Проверки авторизации ролей и делегированных разрешений

Следующие роли каталога необходимы вызывающему пользователю для управления рабочим процессом запросов или чтения списка запросов.

| Operation | Делегированные разрешения | Требуемая роль каталога вызывающего пользователя |
|:------------------|:------------|:--------------------------------------------|
| Чтение | ConsentRequest.Read.All, ConsentRequest.ReadWrite.All | Глобальный администратор, глобальный читатель, администратор облачных приложений и администратор приложений |

## <a name="see-also"></a>См. также

- [Настройка рабочего процесса предоставления согласия администратора (предварительная версия)](/azure/active-directory/manage-apps/configure-admin-consent-workflow?preserve-view=true)


<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
