---
title: Проверки доступа Azure AD
description: Используйте обзоры доступа Azure AD, чтобы настроить разовую или повторяемую проверку доступа для проверки прав пользователя на доступ к ресурсам Azure AD.
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 8bdf2a99e0b26adfaa5b00d207397ce225599478
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722864"
---
# <a name="azure-ad-access-reviews"></a>Проверки доступа Azure AD

Пространство имен: microsoft.graph

Используйте [обзоры доступа Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) , чтобы настроить разовую или повторяемую проверку доступа для проверки прав пользователей на доступ к ресурсам Azure AD. Эти ресурсы Azure AD включают группы, директора служб, пакеты доступа и привилегированные роли.

Типичные сценарии для отзывов о доступе:

- Клиенты могут просмотреть и сертифицировать гостевой доступ пользователей к группам с помощью членства в группе. Рецензенты могут использовать сведения, предоставляемые для эффективного решения о том, следует ли гостям иметь постоянный доступ.
- Клиенты могут просмотреть и сертифицировать доступ сотрудников к ресурсам Azure AD.
- Клиенты могут проверять и проверять назначения в привилегированные роли Azure AD. Это поддерживает организации в управлении привилегированным доступом.

Функция обзоров доступа, в том числе API, доступна только с действительной лицензией на покупку или пробную лицензию подписки Azure AD Premium P2 emS E5. Дополнительные сведения о требованиях к лицензиям см. в обзоре [требований к лицензии Access](/azure/active-directory/governance/access-reviews-overview#license-requirements).

## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с обзором доступа.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
|**Определение расписания**| | |
|[Определения списков](../api/accessreviewset-list-definitions.md)|[accessReviewScheduleDefinition collection](../resources/accessreviewscheduledefinition.md)|Получите список объектов [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) и их свойств.|
|[Создание определений](../api/accessreviewset-post-definitions.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Создайте новый [объект accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .|
|[Получить accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .|
|[Обновление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Обновление свойств объекта [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .|
|[Удаление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md)|Отсутствует|Удаляет объект [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .|
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[accessReviewScheduleDefinition collection](../resources/accessreviewscheduledefinition.md)|Возвращает все определения, в которых пользователь вызовов является рецензентом любых экземпляров.|
|**Экземпляры**| | |
|[Перечисление экземпляров](../api/accessreviewscheduledefinition-list-instances.md)|[accessReviewInstance](../resources/accessreviewinstance.md) collection|Получите список объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств.|
|[Получить accessReviewInstance](../api/accessreviewinstance-get.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstance](../resources/accessreviewinstance.md) .|
|[stop](../api/accessreviewinstance-stop.md)|Отсутствует|Вручную остановите accessReviewInstance.|
|[sendReminder](../api/accessreviewinstance-sendreminder.md)|Отсутствует|Отправьте напоминание рецензентам accessReviewInstance.|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|Отсутствует|Сброс всех элементов решений в экземпляре `notReviewed`|
|[applyDecisions](../api/accessreviewinstance-applydecisions.md)|Нет|Вручную применить решение для accessReviewInstance.|
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md)|Нет| Позволяет вызываемой пользователю принять рекомендацию по принятию решений для каждого notReviewed accessReviewInstanceDecisionItem, на которых он является рецензентом для определенного accessReviewInstance.|
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|Нет|Просмотр пакетов принципов или ресурсов в одном вызове.|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) collection|Возвращает все объекты экземпляра в определение, для которого вызываемая пользователь является рецензентом.|
|**Элементы решения экземпляра**| | |
|[Список решений](../api/accessreviewinstance-list-decisions.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Получите список объектов [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) и их свойств.|
|[Get accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .|
|[Обновление accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Обновление свойств объекта [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .|
|[accessReviewInstanceDecisionItem: filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Возвращает элементы решения, для которых пользователь вызовов является рецензентом.|
|**Определения истории**| | |
|[Список historyDefinitions](../api/accessreviewset-list-historydefinitions.md)|[accessReviewHistoryDefinition collection](accessreviewhistorydefinition.md)|Получите список объектов [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) и их свойств.|
|[Создание historyDefinitions](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Создайте новый [объект accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|
|[Получить accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|
|[generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|Создание URI для экземпляра, который можно использовать для получения данных истории отзывов.|
|[Перечисление экземпляров](../api/accessreviewhistorydefinition-list-instances.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|Извлечение списка [объектов accessReviewHistoryInstance](accessreviewhistoryinstance.md) и их свойств.|

## <a name="role-and-application-permission-authorization-checks"></a>Проверки авторизации ролей и разрешений на приложения

Для управления отзывами доступа для вызываемой пользователя требуются следующие роли [Azure AD](/azure/active-directory/roles/permissions-reference) .

| Операция | Разрешения приложений | Роль требуемого каталога вызываемого пользователя |
|:------------------|:------------|:--------------------------------------------|
| Чтение | AccessReview.Read.All или AccessReview.ReadWrite.All | Глобальный администратор, глобальный читатель, администратор безопасности, читатель безопасности или администратор пользователей |
| Создание, обновление или удаление | AccessReview.ReadWrite.All | Глобальный администратор или администратор пользователей |

Кроме того, пользователь, которому назначен рецензент обзора доступа, может управлять своими решениями без необходимости быть в роли каталога.

## <a name="see-also"></a>См. также

- [Учебники](/graph/accessreviews-overview) , чтобы узнать, как использовать API обзоров доступа для проверки доступа к ресурсам Azure AD
- [Управление доступом к пользователю с помощью отзывов о доступе к Azure AD администратору](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Управление гостевых доступом администратора с помощью отзывов о доступе к Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
