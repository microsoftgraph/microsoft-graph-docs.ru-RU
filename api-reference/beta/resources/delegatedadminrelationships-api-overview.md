---
title: Подробный обзор API делегированных привилегий администратора (GDAP)
description: Детализированные делегированные права администратора (GDAP) позволяют партнерам Майкрософт настраивать и запрашивать детализированный и ограниченный по времени доступ к средам своих клиентов, позволяя клиентам применять минимальный уровень доступа для партнеров Майкрософт.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 1916627207c8b4c9d8f3a36f400d66a4e4577b9b
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855635"
---
# <a name="granular-delegated-admin-privileges-gdap-api-overview"></a>Подробный обзор API делегированных привилегий администратора (GDAP)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В рамках экосистемы Центра партнеров Майкрософт партнеры Майкрософт в рамках программы "Поставщик облачных решений", "Торговый посредник с добавленной ценностью" или "Помощник" могут выполнять административные операции с клиентами, чтобы управлять службами клиента, например Azure AD и Microsoft 365. Эта возможность ранее позволяет партнерам на неограниченное время выполнять роль глобального администратора в клиенте клиента, создавая потенциальные уязвимости для системы безопасности и ограничив потенциал рынка.

Детализированные делегированные права администратора **(GDAP)** предоставляют партнерам с минимальными привилегиями доступ к своим клиентам после модели кибербезопасности "Никому не [доверяй"](/security/zero-trust/). С помощью GDAP партнеры настраивают и запрашивают детализированный и ограниченный по времени доступ к средам своих клиентов, и клиенты должны явным образом предоставить партнерам этот наименее привилегированный доступ. Кроме того, партнеры должны запрашивать определенные роли для администрирования клиента в течение определенного периода времени. Этот элемент управления избавляет партнеров от необходимости иметь роль глобального администратора в клиенте клиента, но вместо этого у них теперь есть менее привилегированные разрешения, которые им абсолютно необходимы для делегированных административных задач.

Дополнительные сведения о GDAP см. в следующих статьях:
+ [Введение в детализированные делегированные права администратора (GDAP)](/partner-center/gdap-introduction)
+ [Роли с минимальными привилегиями по задачам](/partner-center/gdap-least-privileged-roles-by-task)

## <a name="use-cases-for-gdap-apis"></a>Варианты использования API GDAP

В этом разделе описаны способы, с помощью которых партнеры Майкрософт могут использовать API GDAP для программного управления делегированными отношениями администратора для своих клиентов.

### <a name="delegated-admin-relationship"></a>Отношение делегированного администратора

| Варианты использования | Интерфейсы API |
|--|--|
| Создание нового делегированного отношения администратора для утверждения любым клиентом <br/> Создание новой делегированной связи администратора для утверждения конкретным клиентом | [Создание delegatedAdminRelationship](../api/tenantrelationship-post-delegatedadminrelationships.md) |
| Вывод списка всех делегированных отношений администратора партнера <br/> Вывод списка всех делегированных отношений администратора для конкретного клиента | [Перечисление объектов delegatedAdminRelationship](../api/tenantrelationship-list-delegatedadminrelationships.md) |
| Получение делегированных отношений администратора по идентификатору | [Получение delegatedAdminRelationship](../api/delegatedadminrelationship-get.md)  |
| Удаление отношения делегированного администратора | [Удаление delegatedAdminRelationship](../api/delegatedadminrelationship-delete.md) |

### <a name="delegated-admin-relationship-request"></a>Запрос отношения делегированного администратора

| Варианты использования | Интерфейсы API |
|--|--|
| Создайте запрос на делегированное отношение администратора, чтобы заблокировать связь для утверждения клиента или завершить существующую связь. | [Создание запросов](../api/delegatedadminrelationship-post-requests.md) |
| Получение запроса на отношение делегированного администратора по идентификатору | [Получение delegatedAdminRelationshipRequest](../api/delegatedadminrelationshiprequest-get.md) |
| Вывод списка всех запросов делегированных отношений администратора для заданной связи | [Перечисление запросов](../api/delegatedadminrelationship-list-requests.md) |


### <a name="role-assignments"></a>Назначения ролей

| Варианты использования | Интерфейсы API |
|--|--|
| Создание нового делегированного назначения доступа администратора для отношения делегированного администратора | [Создание accessAssignments](../api/delegatedadminrelationship-post-accessassignments.md) |
| Перечисление назначений доступа для делегированных отношений администратора | [Перечисление объектов accessAssignment](../api/delegatedadminrelationship-list-accessassignments.md) |
| Получение делегированного назначения доступа к отношениям администратора по идентификатору | [Получение delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-get.md) |
| Удаление назначения доступа делегированной связи администратора | [Удаление delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-delete.md) |
| Обновление назначений ролей для делегированного назначения доступа к отношениям администратора | [Обновление delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-update.md) |

### <a name="long-running-operations"></a>Длительные операции

| Варианты использования | Интерфейсы API |
|--|--|
| Вывод списка всех длительных операций делегированного отношения администратора | [Операции со списком](../api/delegatedadminrelationship-list-operations.md) |
| Получение длительной операции делегированного отношения администратора | [Получение delegatedAdminRelationshipOperation](../api/delegatedadminrelationshipoperation-get.md) |


### <a name="delegated-admin-customers"></a>Делегированные клиенты-администраторы

| Варианты использования | Интерфейсы API |
|--|--|
| Перечисление всех полномочного администратора клиентов | [Перечисление delegatedAdminCustomers](../api/tenantrelationship-list-delegatedadmincustomers.md)|
| Получение одного полномочного администратора по идентификатору | [Получение delegatedAdminCustomer](../api/delegatedadmincustomer-get.md) |
| Получение сведений об управлении службами для полномочного администратора клиента | [Перечисление serviceManagementDetails](../api/delegatedadmincustomer-list-servicemanagementdetails.md) |


## <a name="gdap-workflow"></a>Рабочий процесс GDAP

### <a name="gdap-relationship-status-transition"></a>Переход состояния связи GDAP

Состояние делегированного Администратор переходит следующим образом:

![Схема перехода состояния Администратор делегированных данных](relationship-status-transitions.png)

1. [Создание delegatedAdminRelationship](../api/tenantrelationship-post-delegatedadminrelationships.md)
2. [Обновление delegatedAdminRelationship](../api/delegatedadminrelationship-update.md)
3. [Create delegatedAdminRelationshipRequest](../api/delegatedadminrelationship-post-requests.md) (action: lockForApproval)
4. [Create delegatedAdminRelationshipRequest](../api/delegatedadminrelationship-post-requests.md) (action: terminate)

### <a name="gdap-relationship-access-assignment-status-transition"></a>Переход состояния назначения доступа к отношениям GDAP

Состояние делегированного Администратор доступа. Переходы состояния выполняются следующим образом:

![Схема перехода Администратор назначения делегированного доступа](access-assignment-status-transitions.png)

1. [Создание delegatedAdminAccessAssignment](../api/delegatedadminrelationship-post-accessassignments.md)
2. [Удаление delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-delete.md)

## <a name="permissions"></a>Разрешения

Для управления отношениями делегированного администратора вызывающий субъект должен находиться в клиенте партнера и иметь соответствующие детализированные делегированные разрешения [администратора](/graph/permissions-reference#granular-delegated-admin-privileges-gdap-permissions).


## <a name="see-also"></a>См. также

+ [Введение в детализированные делегированные права администратора (GDAP)](/partner-center/gdap-introduction)