---
title: Проверки доступа Azure AD
description: Проверки доступа Azure AD можно использовать для настройки однофакторной или повторяющейся проверки доступа для аттестации прав доступа пользователя. Эта документация обслуживает 2-ю версию API.
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 141021e58e995e5939ad1dec2b915fbacfbddf21
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436612"
---
# <a name="azure-ad-access-reviews"></a>Проверки доступа Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Используйте [Azure AD проверки доступа](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) для настройки однофакторной или повторяющейся проверки доступа для аттестации прав пользователей на доступ к Azure AD ресурсам. К Azure AD ресурсов относятся группы, субъекты-службы, пакеты доступа и привилегированные роли.

Типичные сценарии клиентов для проверок доступа:

- Клиенты могут просматривать и сертифицировать доступ гостевых пользователей к группам с помощью членства в группах. Рецензенты могут использовать аналитические сведения, которые предоставляются, чтобы эффективно решить, должны ли гости иметь постоянный доступ.
- Клиенты могут просматривать и сертифицировать доступ сотрудников к Azure AD ресурсам.
- Клиенты могут просматривать и проводить аудит назначений Azure AD привилегированных ролей. Это поддерживает организации в управлении привилегированным доступом.

Обратите внимание, что функция проверки доступа, включая API, включена в Azure AD Premium P2.  Клиент, в котором создается проверка доступа, должен иметь допустимую приобретенную или пробную Azure AD Premium P2 или подписку EMS E5. Дополнительные сведения о требованиях к лицензиям см. в разделе ["Требования к лицензиям для проверки доступа"](/azure/active-directory/governance/access-reviews-overview#license-requirements).

[!INCLUDE [GDPR-related-guidance](../../includes/gdpr-msgraph-export-note.md)]

## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с проверкой доступа.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
|**Расписания определений**| | |
|[Определения списков](../api/accessreviewset-list-definitions.md) | [Коллекция accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Получение списка объектов [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) и их свойств. |
|[Получение accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Получение объекта accessReviewScheduleDefinition и его свойств. |
|[Создание определений](../api/accessreviewset-post-definitions.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Создайте новый accessReviewScheduleDefinition. |
|[Удаление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Нет. | Удаление объекта accessReviewScheduleDefinition. |
|[Обновление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Нет. | Обновление свойств объекта accessReviewScheduleDefinition с помощью указанного идентификатора. |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[Коллекция accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Извлекает все определения, для которых вызывающий пользователь является рецензентом в одном или нескольких экземплярах.|
|**Экземпляров**| | |
|[Перечисление экземпляров](../api/accessreviewscheduledefinition-list-instances.md) | [Коллекция accessReviewInstance](accessreviewinstance.md) | Получение списка объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств. |
|[Получение accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Чтение свойств и связей объекта [accessReviewInstance](../resources/accessreviewinstance.md) . |
|[sendReminder](../api/accessreviewinstance-sendreminder.md) | Нет. | Отправьте напоминание рецензентам accessReviewInstance. |
|[stop](../api/accessreviewinstance-stop.md) | Нет. | Вручную остановите accessReviewInstance. |
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md) | Нет. | Позволяет вызывающему пользователю принять рекомендацию по принятию решения для каждого объекта NotReviewInstanceDecisionItem, в котором он является рецензентом для определенного объекта accessReviewInstance. |
|[applyDecisions](../api/accessreviewinstance-applydecisions.md) | Нет. | Вручную примените решения к accessReviewInstance. |
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|Нет|Просмотрите пакеты субъектов или ресурсов за один вызов.|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|Нет|Сбрасывает все элементы принятия решений в экземпляре в значение `notReviewed`.|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[Коллекция accessReviewInstance](../resources/accessreviewinstance.md)|Возвращает все экземпляры в заданном [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) , для которого вызывающий пользователь является рецензентом одного или нескольких решений.|
|**Элементы принятия решений об экземпляре**| | |
|[Список решений](../api/accessreviewinstance-list-decisions.md) | [Коллекция accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Получение списка объектов [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) и их свойств.|
|[Получение объекта accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Чтение свойств и связей объекта [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .|
|[Обновление accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Нет. | Для любых объектов accessReviewInstanceDecisionItems, для которых вызывающему пользователю назначен рецензент, вызывающий пользователь может записать решение, исправив объект принятия решения. |
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[Коллекция accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Извлекает все [объекты accessReviewInstanceDecisionItems](accessreviewinstancedecisionitem.md) , где вызывающее использование является рецензентом для данного [объекта accessReviewInstance](accessreviewinstance.md).|
|[listPendingApproval](../api/accessreviewinstancedecisionitem-listpendingapproval.md) (не рекомендуется) | [коллекция accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . | Получение всех объектов accessReviewInstanceDecisionItems, назначенных вызывающему пользователю, для определенного объекта accessReviewInstance. Этот метод является устаревшим и заменяется [accessReviewInstanceDecisionItem: filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md). |
|**Определения журнала**| | |
|[Перечисление historyDefinitions](../api/accessreviewset-list-historydefinitions.md)|[Коллекция accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Получение списка объектов [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) и их свойств.|
|[Создание historyDefinitions](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Создайте объект [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|
|[Получение accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Чтение свойств и связей объекта [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|
|[generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|Создайте универсальный код ресурса (URI) для экземпляра, который можно использовать для получения данных журнала проверки.|
|[Перечисление экземпляров](../api/accessreviewhistorydefinition-list-instances.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|Получение списка объектов [accessReviewHistoryInstance](accessreviewhistoryinstance.md) и их свойств.|
|**Политика**| | |
|[Получение accessReviewPolicy](../api/accessreviewpolicy-get.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Чтение свойств и связей объекта [accessReviewPolicy](../resources/accessreviewpolicy.md) .|
|[Обновление accessReviewPolicy](../api/accessreviewpolicy-update.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Обновление свойств объекта [accessReviewPolicy](../resources/accessreviewpolicy.md) .|
|[Список определений, ожидающих утверждения](../api/accessreviewscheduledefinition-filterbycurrentuser.md) (не рекомендуется)|[Коллекция accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Извлекает все определения, для которых вызывающий пользователь является рецензентом в одном или нескольких экземплярах. Этот метод является устаревшим и заменяется [accessReviewScheduleDefinition: filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md).|
|[Перечисление pendingAccessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) (не рекомендуется) | [коллекция accessReviewInstance](accessreviewinstance.md) . | Получение всех ожидающих ресурсов accessReviewInstance, назначенных вызывающему пользователю. Этот метод является устаревшим и заменяется [accessReviewInstance: filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md). |

## <a name="role-and-application-permission-authorization-checks"></a>Проверки авторизации разрешений ролей и приложений

Для [управления проверками доступа вызывающему](/azure/active-directory/roles/permissions-reference) пользователю требуются следующие Azure AD роли.

| Operation | Разрешения приложений | Требуемая роль каталога вызывающего пользователя |
|:------------------|:------------|:--------------------------------------------|
| Чтение | AccessReview.Read.All или AccessReview.ReadWrite.All | Глобальный администратор, глобальный читатель, администратор безопасности, читатель безопасности или администратор пользователей |
| Создание, обновление или удаление | AccessReview.ReadWrite.All | Глобальный администратор или администратор пользователей |

Кроме того, пользователь, который является назначенным рецензентом проверки доступа, может управлять своими решениями без необходимости быть в роли каталога.

## <a name="see-also"></a>См. также

- [Руководства по](/graph/accessreviews-overview) использованию API проверок доступа для проверки доступа к Azure AD ресурсам
- [Как администратор может управлять доступом пользователей с помощью Azure AD доступа](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Как администратор может управлять гостевым доступом с помощью Azure AD доступа](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)


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

