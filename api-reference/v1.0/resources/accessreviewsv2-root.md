---
title: Проверки доступа Azure AD
description: Используйте обзоры доступа Azure AD, чтобы настроить разовую или повторяемую проверку доступа для проверки прав пользователя на доступ к ресурсам Azure AD.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 2158986ccae423614c8af3e54bc79a2f019102a0
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030316"
---
# <a name="azure-ad-access-reviews"></a>Проверки доступа Azure AD

Пространство имен: microsoft.graph


Используйте обзоры доступа [Azure AD,](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) чтобы настроить разовую или повторяемую проверку доступа для проверки прав пользователя на доступ к ресурсам Azure AD.

Типичные сценарии клиентского доступа к отзывам о членстве в группах и приложениях и доступе к роли Azure AD:

- Клиенты могут просмотреть и сертифицировать гостевой доступ пользователей к приложениям, роли Azure AD и членство в группах. Рецензенты могут использовать сведения, предоставляемые для эффективного решения о том, следует ли гостям иметь постоянный доступ.

- Клиенты могут просмотреть и сертифицировать доступ сотрудников к приложениям, ролям Azure AD и членству в группах с отзывами о доступе.

Функция обзоров доступа, включая API, доступна только с действительной лицензией на покупку или пробную лицензию подписки Azure AD Premium P2 emS E5.


## <a name="methods"></a>Methods

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с обзором доступа.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
|[Список accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md)|[accessReviewScheduleDefinition collection](../resources/accessreviewscheduledefinition.md)|Получите список объектов [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) и их свойств.|
|[Создание accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-post.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Создайте новый [объект accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)|
|[Получить accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)|
|[Обновление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Обновление свойств объекта [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)|
|[Удаление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md)|Нет|Удаляет объект [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)|
|[accessReviewScheduleDefinition: filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[accessReviewScheduleDefinition collection](../resources/accessreviewscheduledefinition.md)|Возвращает все определения, в которых пользователь вызовов является рецензентом любых экземпляров.|
|[Список accessReviewInstances](../api/accessreviewinstance-list.md)|[accessReviewInstance](../resources/accessreviewinstance.md) collection|Получите список объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств.|
|[Получить accessReviewInstance](../api/accessreviewinstance-get.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstance.](../resources/accessreviewinstance.md)|
|[accessReviewInstance: остановка](../api/accessreviewinstance-stop.md)|Нет|Вручную остановите accessReviewInstance.|
|[accessReviewInstance: sendReminder](../api/accessreviewinstance-sendreminder.md)|Нет|Отправьте напоминание рецензентам accessReviewInstance.|
|[accessReviewInstance: resetDecisions](../api/accessreviewinstance-resetdecisions.md)|Нет|Сброс всех элементов решений в экземпляре `notReviewed`|
|[accessReviewInstance: applyDecisions](../api/accessreviewinstance-applydecisions.md)|Нет|Вручную применить решение для accessReviewInstance.|
|[accessReviewInstance: acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md)|Нет| Позволяет вызываемой пользователю принять рекомендацию по принятию решений для каждого notReviewed accessReviewInstanceDecisionItem, на которых он является рецензентом для определенного accessReviewInstance.|
|[accessReviewInstance: batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|Нет|Просмотр пакетов принципов или ресурсов в одном вызове.|
|[accessReviewInstance: filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) collection|Возвращает все объекты экземпляра в определение, для которого вызываемая пользователь является рецензентом.|
|[List accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Получите список объектов [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) и их свойств.|
|[Get accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)|
|[Обновление accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Обновление свойств объекта [accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)|
|[accessReviewInstanceDecisionItem: filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Возвращает элементы решения, для которых пользователь вызовов является рецензентом.|


## <a name="role-and-application-permission-authorization-checks"></a>Проверки авторизации ролей и разрешений на приложения

Для управления отзывами доступа для вызываемой пользователя требуются следующие роли каталога. 

| Операция | Разрешения приложений | Роль требуемого каталога вызываемого пользователя |
|:------------------|:------------|:--------------------------------------------|
| Чтение | AccessReview.Read.All или AccessReview.ReadWrite.All | Глобальный администратор, глобальный читатель, администратор безопасности, читатель безопасности или администратор пользователей |
| Создание, обновление или удаление | AccessReview.ReadWrite.All | Глобальный администратор или администратор пользователей |

Кроме того, пользователь, которому назначен рецензент обзора доступа, может управлять своими решениями без необходимости быть в роли каталога.

## <a name="see-also"></a>См. также

- [Управление доступом к пользователю с помощью отзывов о доступе к Azure AD администратору](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Управление гостевых доступом администратора с помощью отзывов о доступе к Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
