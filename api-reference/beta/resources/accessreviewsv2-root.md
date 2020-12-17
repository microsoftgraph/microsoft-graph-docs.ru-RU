---
title: Проверки доступа Azure AD — членство в группах
description: Вы можете использовать проверки доступа Azure AD, чтобы настроить однововременные или повторяющиеся проверки доступа для проверки прав доступа пользователя. В этой документации используется 2-я версия API.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 5c5cbe43c75e5f0ac0ea552c380b294c7725907e
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705956"
---
# <a name="azure-ad-access-reviews-group-memberships"></a>Проверки доступа Azure AD (членство в группах)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>Эта документация относится к проверке доступа к членству в группах. Обзоры доступа для всех других поддерживаемых типов ресурсов см. в отзывах [Access (все ресурсы).](accessreviews-root.md)
>
>В настоящее время этот API поддерживает только проверки доступа членства в группах.

Вы можете использовать проверки [доступа Azure AD,](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) чтобы настроить однововременные или повторяющиеся проверки доступа для проверки прав доступа пользователей.

Типичные сценарии проверки доступа клиентов на членство в группах и доступ к приложениям:

- Клиенты могут просмотреть и сертифицировать доступ гостевых пользователей с помощью проверок доступа к приложениям и членствам в группах. Рецензенты могут использовать предоставленные сведения, чтобы эффективно решить, должны ли гости иметь постоянный доступ.

- Клиенты могут просмотреть и сертифицировать доступ сотрудников к приложениям и членству в группах с помощью проверок доступа.

- Клиенты могут собирать средства контроля доступа в программы, релевантные для вашей организации, для отслеживания проверок соответствия требованиям или приложений, чувствительных к рискам.

Клиенты также могут просмотреть и сертифицировать назначения ролей административных пользователей, которым назначены роли Azure AD, такие как роли глобального администратора или подписки Azure.  Эта возможность включена в [Azure AD Privileged Identity Management.](privilegedidentitymanagement-root.md)

Обратите внимание, что функция проверки доступа, включая API, включена в Azure AD Premium P2.  У клиента, на котором создается проверка доступа, должна быть действительная приобретенная или пробная подписка на Azure AD Premium P2 или EMS E5.


## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с проверкой доступа.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
|[Список accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-list.md) | [Коллекция accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Перечисляет все `accessReviewScheduleDefinition` . Не включает связанные `accessReviewInstance` экземпляры в списки. |
|[Get accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Get an `accessReviewScheduleDefinition` with a specified id. |
|[Создание accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-create.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Создание объекта `accessReviewScheduleDefinition`. |
|[Удаление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Нет. | Удаление с `accessReviewScheduleDefinition` указанным ИД. |
|[Обновление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Нет. | Обновление свойств объекта с `accessReviewScheduleDefinition` указанным ИД. |
|[Список accessReviewInstance](../api/accessreviewinstance-list.md) | [Коллекция accessReviewInstance](accessreviewinstance.md) | Перечисляет `accessReviewInstance` каждый из них для определенного `accessReviewScheduleDefinition` . Не включает связанные `accessReviewInstanceDecisionItem` s в листинги. |
|[Get accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Возвращает для `accessReviewInstance` `accessReviewScheduleDefinition` . Не включает связанные `accessReviewInstanceDecisionItem` s в объект. |
|[Список ожидающих утверждения accessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [коллекция accessReviewInstance;](accessreviewinstance.md) | Получите `accessReviewInstance` все, что назначено вызываемму пользователю. |
|[Отправка напоминания accessReviewInstance](../api/accessreviewinstance-sendreminder.md) | Нет. | Отправьте напоминание рецензентам. `accessReviewInstance` |
|[Остановка accessReviewInstance](../api/accessreviewinstance-stop.md) | Нет. | Вручную остановите `accessReviewInstance` . |
|[Принятие рекомендаций](../api/accessreviewinstance-acceptrecommendations.md) | Нет. | Позволяет вызываемой пользователю принять рекомендации по принятию решений для каждого notReviewed, в которых он является рецензентом для `accessReviewInstanceDecisionItem` определенного `accessReviewInstance` . |
|[Применение решений](../api/accessreviewinstance-applydecisions.md) | Нет. | Вручную применить решение по `accessReviewInstance` . |
|[Список accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [Коллекция accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Перечисляет `accessReviewInstanceDecisionItem` каждый из них для определенного `accessReviewInstance` . |
|[Список accessReviewInstanceDecisionItems, ожидающих утверждения](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [коллекция accessReviewInstanceDecisionItem;](accessreviewinstancedecisionitem.md) | Получите `accessReviewInstanceDecisionItems` все, что назначено вызываемму пользователю, для конкретного `accessReviewInstance` пользователя. |
|[Обновление accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Нет. | Если вызывающий пользователь назначен рецензенту, вызывающий пользователь может записать решение, внося `accessReviewInstanceDecisionItems` исправления в объект решения. |

## <a name="role-and-application-permission-authorization-checks"></a>Проверки авторизации разрешений ролей и приложений

Следующие роли каталога необходимы вызываемой пользователю для управления проверками доступа. Обратите внимание, что в настоящее время с помощью API Microsoft Graph поддерживаются только проверки доступа для групп.

| Операция | Разрешения приложений | Требуемая роль каталога вызываемого пользователя |
|:------------------|:------------|:--------------------------------------------|
| Чтение | AccessReview.Read.All или AccessReview.ReadWrite.All | Глобальный администратор, глобальный читатель, администратор безопасности, читатель безопасности или администратор пользователя |
| Создание, обновление или удаление | AccessReview.ReadWrite.All | Глобальный администратор или администратор пользователей |

Кроме того, пользователь, который является назначенным рецензентом проверки доступа, может управлять своими решениями без необходимости быть в роли каталога.

## <a name="see-also"></a>См. также

- [Как администратор может управлять доступом пользователей с помощью проверок доступа Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Как администратор может управлять гостевим доступом с помощью проверок доступа Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)


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


