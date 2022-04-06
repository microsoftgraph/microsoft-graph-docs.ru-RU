---
title: Проверки доступа Azure AD
description: Используйте проверки доступа Azure AD для настройки однофакторной или повторяющейся проверки доступа для аттестации прав пользователя на доступ к ресурсам Azure AD.
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 7ab9d350c88ce1291a44e517d2c527110a08f7a3
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684734"
---
# <a name="azure-ad-access-reviews"></a>Проверки доступа Azure AD

Пространство имен: microsoft.graph

Используйте [проверки доступа Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) для настройки однофакторной или повторяющейся проверки доступа для аттестации прав пользователей на доступ к ресурсам Azure AD. К этим ресурсам Azure AD относятся группы, субъекты-службы, пакеты доступа и привилегированные роли.

Типичные сценарии клиентов для проверок доступа:

- Клиенты могут просматривать и сертифицировать доступ гостевых пользователей к группам с помощью членства в группах. Рецензенты могут использовать аналитические сведения, которые предоставляются, чтобы эффективно решить, должны ли гости иметь постоянный доступ.
- Клиенты могут просматривать и сертифицировать доступ сотрудников к ресурсам Azure AD.
- Клиенты могут просматривать и проводить аудит назначений привилегированным ролям Azure AD. Это поддерживает организации в управлении привилегированным доступом.

Функция проверки доступа, включая API, доступна только с действительной лицензией на покупку или пробную версию подписки Azure AD Premium P2 EMS E5. Дополнительные сведения о требованиях к лицензиям см. в разделе ["Требования к лицензиям для проверки доступа"](/azure/active-directory/governance/access-reviews-overview#license-requirements).

[!INCLUDE [GDPR-related-guidance](../../includes/accessreviews-gdpr-overview-note.md)]

## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с проверкой доступа.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
|**Расписания определений**| | |
|[Определения списков](../api/accessreviewset-list-definitions.md)|[Коллекция accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Получение списка объектов [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) и их свойств.|
|[Создание определений](../api/accessreviewset-post-definitions.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Создайте объект [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .|
|[Получение accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Чтение свойств и связей объекта [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .|
|[Обновление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Обновление свойств объекта [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .|
|[Удаление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md)|Никаких других изменений не происходит|Удаляет объект [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .|
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[Коллекция accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Возвращает все определения, в которых вызывающий пользователь является рецензентом любых экземпляров.|
|**Экземпляров**| | |
|[Перечисление экземпляров](../api/accessreviewscheduledefinition-list-instances.md)|[Коллекция accessReviewInstance](../resources/accessreviewinstance.md)|Получение списка объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств.|
|[Получение accessReviewInstance](../api/accessreviewinstance-get.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|Чтение свойств и связей объекта [accessReviewInstance](../resources/accessreviewinstance.md) .|
|[stop](../api/accessreviewinstance-stop.md)|Никаких других изменений не происходит|Вручную остановите accessReviewInstance.|
|[sendReminder](../api/accessreviewinstance-sendreminder.md)|Никаких других изменений не происходит|Отправьте напоминание рецензентам accessReviewInstance.|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|Никаких других изменений не происходит|Сбрасывает все элементы принятия решений в экземпляре на `notReviewed`|
|[applyDecisions](../api/accessreviewinstance-applydecisions.md)|Никаких других изменений не происходит|Вручную примените решение к accessReviewInstance.|
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md)|Никаких других изменений не происходит| Позволяет вызывающему пользователю принять рекомендацию по принятию решения для каждого объекта NotReviewInstanceDecisionItem, в котором он является рецензентом для определенного объекта accessReviewInstance.|
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|Никаких других изменений не происходит|Просмотрите пакеты субъектов или ресурсов за один вызов.|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[Коллекция accessReviewInstance](../resources/accessreviewinstance.md)|Возвращает все объекты экземпляра в определении, для которого вызывающий пользователь является рецензентом.|
|**Элементы принятия решений об экземпляре**| | |
|[Список решений](../api/accessreviewinstance-list-decisions.md)|[Коллекция accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Получение списка объектов [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) и их свойств.|
|[Получение объекта accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Чтение свойств и связей объекта [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .|
|[Обновление accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Обновление свойств объекта [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .|
|[accessReviewInstanceDecisionItem: filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[Коллекция accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Возвращает элементы принятия решений, для которых вызывающий пользователь является рецензентом.|
|**Определения журнала**| | |
|[Перечисление historyDefinitions](../api/accessreviewset-list-historydefinitions.md)|[Коллекция accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Получение списка объектов [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) и их свойств.|
|[Создание historyDefinitions](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Создайте объект [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|
|[Получение accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Чтение свойств и связей объекта [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|
|[generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|Создайте универсальный код ресурса (URI) для экземпляра, который можно использовать для получения данных журнала проверки.|
|[Перечисление экземпляров](../api/accessreviewhistorydefinition-list-instances.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|Получение списка объектов [accessReviewHistoryInstance](accessreviewhistoryinstance.md) и их свойств.|

## <a name="role-and-application-permission-authorization-checks"></a>Проверки авторизации разрешений ролей и приложений

Для управления [проверками доступа](/azure/active-directory/roles/permissions-reference) вызывающему пользователю требуются следующие роли Azure AD.

| Операция | Разрешения приложений | Требуемая роль каталога вызывающего пользователя |
|:------------------|:------------|:--------------------------------------------|
| Чтение | AccessReview.Read.All или AccessReview.ReadWrite.All | Глобальный администратор, глобальный читатель, администратор безопасности, читатель безопасности или администратор пользователей |
| Создание, обновление или удаление | AccessReview.ReadWrite.All | Глобальный администратор или администратор пользователей |

Кроме того, пользователь, который является назначенным рецензентом проверки доступа, может управлять своими решениями без необходимости быть в роли каталога.

## <a name="see-also"></a>См. также

- [Руководства по](/graph/accessreviews-overview) использованию API проверки доступа для проверки доступа к ресурсам Azure AD
- [Как администратор может управлять доступом пользователей с помощью проверок доступа Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Как администратор может управлять гостевым доступом с помощью проверок доступа Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
