---
title: Azure Active Directory запросов на согласие
description: Используйте запросы на согласие Azure AD для управления процессом запроса для пользователей, пытающихся получить доступ к приложениям, для которых требуется согласие администратора.
ms.localizationpriority: medium
author: psignoret
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 796a0101d4c0b0649e7cd9cfbaf9ec4c556cdede
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049671"
---
# <a name="azure-active-directory-consent-requests"></a>Azure Active Directory запросов на согласие

Пространство имен: microsoft.graph

Azure Active Directory (Azure AD) помогают управлять процессом запроса для пользователей, пытающихся получить доступ к приложениям, которые требуют утверждения администратора.

Чтобы разрешить пользователям запрашивать доступ или согласие администратора для приложений, которые им не разрешается предоставлять свое согласие, сначала ввести рабочий процесс запроса на согласие. 

>[!NOTE]
>Текущие API ограничиваются настройкой рабочего процесса и чтением списка запросов. В настоящее время нет никаких методов, доступных для программного утверждения или отказа запроса. Однако содержимое запроса можно использовать для воссоздания URL-адреса, который можно использовать для предоставления согласия администратора и утверждения запроса.

Типы ресурсов запроса на согласие включают:

* [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md): указывает политику, с помощью которой можно создавать и управлять запросами на согласие приложений для всего клиента. Существует один **администраторConsentRequestPolicy для** каждого клиента.
* [appConsentRequest:](../resources/appconsentrequest.md)запрос, представляюща коллекцию объектов **userConsentRequest** для определенного приложения.
* [userConsentRequest:](../resources/userconsentrequest.md)запрос, созданный пользователем для использования приложения, для доступа к нему требуется согласие администратора.
* [appConsentRequestScope](../resources/appconsentrequestscope.md): ресурс, содержащий сведения о динамических области разрешений, запрашиваемой для приложения.  

## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами запроса на согласие.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
|[Получить adminConsentRequestPolicy](../api/adminconsentrequestpolicy-get.md) | [коллекция adminConsentRequestPolicy](adminconsentrequestpolicy.md) | Ознакомьтесь с свойствами [администратораConsentRequestPolicy](adminconsentrequestpolicy.md). |
|[Обновление adminConsentRequestPolicy](../api/adminconsentrequestpolicy-update.md) | [коллекция adminConsentRequestPolicy](adminconsentrequestpolicy.md) | Установите конфигурации для [adminConsentRequestPolicy.](adminconsentrequestpolicy.md) |
|[Список appConsentRequests ](../api/appconsentrequest-list.md) | [коллекция appConsentRequest](appconsentrequest.md) | Извлечение коллекции [объектов appConsentRequest.](appconsentrequest.md) |
|[Get appConsentRequests ](../api/appconsentrequest-get.md) | [коллекция appConsentRequest](appconsentrequest.md) | Чтение [объекта appConsentRequest.](appconsentrequest.md) |
|[appConsentRequest: filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md) | [коллекция appConsentRequests](../resources/appconsentrequest.md) | Ознакомьтесь с свойствами объектов [appConsentRequest,](../resources/appconsentrequest.md) для которых текущий пользователь является рецензентом, и состояние запроса на согласие пользователя `InProgress` . |
|[Get userConsentRequest ](../api/userconsentrequest-get.md) | [коллекция userConsentRequest](userconsentrequest.md) | Чтение [объекта userConsentRequest](userconsentrequest.md) для [appConsentRequest](appconsentrequest.md). |
|[Список userConsentRequests ](../api/userconsentrequest-list.md) | [коллекция userConsentRequest](userconsentrequest.md) | Извлечение коллекции [объектов userConsentRequest](userconsentrequest.md) для [приложенияConsentRequest.](appconsentrequest.md) |
|[userConsentRequest: filterByCurrentUser](../api/userconsentrequest-filterByCurrentUser.md) | [коллекция appConsentRequests](../resources/userconsentrequest.md) | Ознакомьтесь с свойствами [объектов userConsentRequest,](../resources/userconsentrequest.md) для которых текущий пользователь является рецензентом. |

## <a name="role-and-delegated-permission-authorization-checks"></a>Проверка роли и делегирования разрешений

Для управления рабочий процессом запросов или чтения списка запросов требуются следующие роли каталога.

| Эксплуатация | Делегированные разрешения | Роль требуемого каталога вызываемого пользователя |
|:------------------|:------------|:--------------------------------------------|
| Чтение | ConsentRequest.Read.All, ConsentRequest.ReadWrite.All | Глобальный администратор, глобальный читатель, администратор облачных приложений и администратор приложений |

## <a name="see-also"></a>См. также

- [Настройка рабочего процесса согласия администратора (предварительный просмотр)](/azure/active-directory/manage-apps/configure-admin-consent-workflow?preserve-view=true)


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
