---
title: Проверки доступа Azure AD
description: Вы можете использовать обзоры доступа Azure AD для настройки одновеких или повторяющихся обзоров доступа для проверки прав доступа пользователя. Эта документация служит 2-й версии API.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: facc1cd9f51d9e638b01fa0bcf5efce5f846e727
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579720"
---
# <a name="azure-ad-access-reviews"></a>Проверки доступа Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]


Вы можете использовать обзоры доступа [Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) для настройки одновеких или повторяющихся обзоров доступа для проверки прав доступа пользователя.

Типичные сценарии клиентского доступа к отзывам о членстве в группе и доступе к приложениям:

- Клиенты могут просмотреть и сертифицировать гостевой доступ пользователей с помощью обзоров доступа к приложениям и членствам групп. Рецензенты могут использовать сведения, предоставляемые для эффективного решения о том, следует ли гостям иметь постоянный доступ.

- Клиенты могут просмотреть и сертифицировать доступ сотрудников к приложениям и членам групп с помощью отзывов о доступе.

- Клиенты могут собирать элементы управления обзором доступа в программы, релевантные для организации, для отслеживания отзывов на соответствие требованиям или приложений, чувствительных к риску.

Кроме того, клиенты могут выполнять проверку и сертификацию назначений ролей административных пользователей, которым назначены роли Azure AD, такие как роли глобального администратора или подписки Azure.  Эта возможность включена в [Azure AD управление привилегированными пользователями.](privilegedidentitymanagement-root.md)

Обратите внимание, что функция обзоров доступа, включая API, включена в Azure AD Premium P2.  Клиент, на котором создается обзор доступа, должен иметь допустимую приобретенную или пробную подписку Azure AD Premium P2 или EMS E5.


## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с обзором доступа.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
|[Список accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-list.md) | [accessReviewScheduleDefinition collection](accessreviewscheduledefinition.md) | Списки `accessReviewScheduleDefinition` каждый . Не включает связанные `accessReviewInstance` экземпляры в списки. |
|[Получить accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Получите `accessReviewScheduleDefinition` указанный id. |
|[Создание accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-post.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Создание объекта `accessReviewScheduleDefinition`. |
|[Удаление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Нет. | Удаление `accessReviewScheduleDefinition` указанного ID. |
|[Обновление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Нет. | Обновление свойств объекта `accessReviewScheduleDefinition` с указанным ИД. |
|[List accessReviewInstance](../api/accessreviewinstance-list.md) | [accessReviewInstance](accessreviewinstance.md) collection | Списки каждого `accessReviewInstance` для определенного `accessReviewScheduleDefinition` . Не включает связанные `accessReviewInstanceDecisionItem` s в списки. |
|[Получить accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Возвращает `accessReviewInstance` для `accessReviewScheduleDefinition` . Не включает связанные `accessReviewInstanceDecisionItem` s в объекте. |
|[Список accessReviewInstances до утверждения](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [accessReviewInstance collection.](accessreviewinstance.md) | Получите все `accessReviewInstance` назначены пользователю вызова. |
|[Отправка напоминания accessReviewInstance](../api/accessreviewinstance-sendreminder.md) | Нет. | Отправьте напоминание рецензентам `accessReviewInstance` . |
|[Остановка accessReviewInstance](../api/accessreviewinstance-stop.md) | Нет. | Вручную остановить `accessReviewInstance` . |
|[Принятие рекомендаций](../api/accessreviewinstance-acceptrecommendations.md) | Нет. | Позволяет вызываемой пользователь принять рекомендацию по решению для каждого notReviewed, что они являются `accessReviewInstanceDecisionItem` рецензентом для определенного `accessReviewInstance` . |
|[Применение решений](../api/accessreviewinstance-applydecisions.md) | Нет. | Вручную применить решение по `accessReviewInstance` . |
|[List accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection | Списки каждого `accessReviewInstanceDecisionItem` для определенного `accessReviewInstance` . |
|[Список accessReviewInstanceDecisionItems до утверждения](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) | Получите `accessReviewInstanceDecisionItems` все, назначенное вызываемой пользователю, для определенного `accessReviewInstance` . |
|[Обновление accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Нет. | Для любого пользователя, на который назначен рецензент, вызывающий пользователь может записать `accessReviewInstanceDecisionItems` решение, заплатив объект решения. |

## <a name="role-and-application-permission-authorization-checks"></a>Проверки авторизации ролей и разрешений на приложения

Для управления отзывами доступа для вызываемой пользователя требуются следующие роли каталога. 

| Operation | Разрешения приложений | Роль требуемого каталога вызываемого пользователя |
|:------------------|:------------|:--------------------------------------------|
| Чтение | AccessReview.Read.All или AccessReview.ReadWrite.All | Глобальный администратор, глобальный читатель, администратор безопасности, читатель безопасности или администратор пользователей |
| Создание, обновление или удаление | AccessReview.ReadWrite.All | Глобальный администратор или администратор пользователей |

Кроме того, пользователь, которому назначен рецензент обзора доступа, может управлять своими решениями без необходимости быть в роли каталога.

## <a name="see-also"></a>См. также

- [Управление доступом к пользователю с помощью отзывов о доступе к Azure AD администратору](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Управление гостевых доступом администратора с помощью отзывов о доступе к Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)


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


