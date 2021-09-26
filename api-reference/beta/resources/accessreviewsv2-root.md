---
title: Проверки доступа Azure AD
description: Вы можете использовать обзоры доступа Azure AD для настройки одновеких или повторяющихся обзоров доступа для проверки прав доступа пользователя. Эта документация служит 2-й версии API.
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 4f0b9e5172e3ea6f5eb4c0d73c08362f6e5f06ef
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767477"
---
# <a name="azure-ad-access-reviews"></a>Проверки доступа Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Используйте обзоры доступа [Azure AD,](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) чтобы настроить разовую или повторяемую проверку доступа для проверки прав пользователей на доступ к ресурсам Azure AD. Эти ресурсы Azure AD включают группы, директора служб, пакеты доступа и привилегированные роли.

Типичные сценарии для отзывов о доступе:

- Клиенты могут просмотреть и сертифицировать гостевой доступ пользователей к группам с помощью членства в группе. Рецензенты могут использовать сведения, предоставляемые для эффективного решения о том, следует ли гостям иметь постоянный доступ.
- Клиенты могут просмотреть и сертифицировать доступ сотрудников к ресурсам Azure AD.
- Клиенты могут проверять и проверять назначения в привилегированные роли Azure AD. Это поддерживает организации в управлении привилегированным доступом.

Обратите внимание, что функция обзоров доступа, включая API, включена в Azure AD Premium P2.  Клиент, на котором создается обзор доступа, должен иметь допустимую подписку на Azure AD Premium P2 или EMS E5.


## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с обзором доступа.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
|**Определение расписания**| | |
|[Список accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [accessReviewScheduleDefinition collection](accessreviewscheduledefinition.md) | Получите список объектов [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) и их свойств. |
|[Получить accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Получите объект accessReviewScheduleDefinition и его свойства. |
|[Создание accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-post.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Создание нового accessReviewScheduleDefinition. |
|[Удаление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Нет. | Удаление accessReviewScheduleDefinition. |
|[Обновление accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Нет. | Обновление свойств accessReviewScheduleDefinition с указанным идентификатором. |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[accessReviewScheduleDefinition collection](../resources/accessreviewscheduledefinition.md)|Извлекает все определения, для которых вызываемая пользователь является рецензентом в одном или более экземплярах.|
|**Экземпляры**| | |
|[Список accessReviewInstances](../api/accessreviewinstance-list.md) | [accessReviewInstance](accessreviewinstance.md) collection | Получите список объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств. |
|[Получить accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstance.](../resources/accessreviewinstance.md) |
|[sendReminder](../api/accessreviewinstance-sendreminder.md) | Нет. | Отправьте напоминание рецензентам accessReviewInstance. |
|[stop](../api/accessreviewinstance-stop.md) | Нет. | Вручную остановите accessReviewInstance. |
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md) | Нет. | Позволяет вызываемой пользователю принять рекомендацию по принятию решений для каждого notReviewed accessReviewInstanceDecisionItem, на которых он является рецензентом для определенного accessReviewInstance. |
|[applyDecisions](../api/accessreviewinstance-applydecisions.md) | Нет. | Вручную применять решения для accessReviewInstance. |
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|Нет|Просмотр пакетов принципов или ресурсов в одном вызове.|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|Нет|Сброс всех элементов решений в экземпляре `notReviewed` в .|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) collection|Возвращает все экземпляры в данном [accessReviewScheduleDefinition,](accessreviewscheduledefinition.md) для которого вызываемая пользователь является рецензентом одного или более решений.|
|**Элементы решения экземпляра**| | |
|[List accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection | Получите список объектов [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) и их свойств.|
|[Get accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)|
|[Обновление accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Нет. | Для любого accessReviewInstanceDecisionItems, на который вызывается пользователь, на который назначен рецензент, вызывающий пользователь может записать решение, заплатив объект решения. |
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Извлекает все [объекты accessReviewInstanceDecisionItems,](accessreviewinstancedecisionitem.md) где использование вызовов является рецензентом для данного [accessReviewInstance.](accessreviewinstance.md)|
|[listPendingApproval](../api/accessreviewinstancedecisionitem-listpendingapproval.md) (отклонено) | [accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) | Получите все accessReviewInstanceDecisionItems, назначенные вызываемой пользователю, для определенного accessReviewInstance. Этот метод отстает и заменяется [accessReviewInstanceDecisionItem: filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md). |
|**Определения истории**| | |
|[Список accessReviewHistoryDefinitions](../api/accessreviewhistorydefinition-list.md)|[accessReviewHistoryDefinition collection](accessreviewhistorydefinition.md)|Получите список объектов [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) и их свойств.|
|[Создание accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-post.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Создайте новый [объект accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)|
|[Получить accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)|
|[generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Создание URI, который можно использовать для получения данных истории отзывов.|
|**Policy**| | |
|[Получить accessReviewPolicy](../api/accessreviewpolicy-get.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewPolicy.](../resources/accessreviewpolicy.md)|
|[Обновление accessReviewPolicy](../api/accessreviewpolicy-update.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Обновление свойств объекта [accessReviewPolicy.](../resources/accessreviewpolicy.md)|
|[Определения списка, ожидающих утверждения](../api/accessreviewscheduledefinition-filterbycurrentuser.md) (неподготовленные)|[accessReviewScheduleDefinition collection](../resources/accessreviewscheduledefinition.md)|Извлекает все определения, для которых вызываемая пользователь является рецензентом в одном или более экземплярах. Этот метод отстает и заменяется [accessReviewScheduleDefinition: filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md).|
|[Список ожидающихAccessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) (обесценив) | [accessReviewInstance collection.](accessreviewinstance.md) | Получите все ожидающих accessReviewInstance ресурсы, назначенные вызываемой пользователю. Этот метод отстает и заменяется [accessReviewInstance: filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md). |

## <a name="role-and-application-permission-authorization-checks"></a>Проверки авторизации ролей и разрешений на приложения

Для управления отзывами доступа для вызываемой пользователя требуются следующие роли [Azure AD.](/azure/active-directory/roles/permissions-reference)

| Операция | Разрешения приложений | Роль требуемого каталога вызываемого пользователя |
|:------------------|:------------|:--------------------------------------------|
| Чтение | AccessReview.Read.All или AccessReview.ReadWrite.All | Глобальный администратор, глобальный читатель, администратор безопасности, читатель безопасности или администратор пользователей |
| Создание, обновление или удаление | AccessReview.ReadWrite.All | Глобальный администратор или администратор пользователей |

Кроме того, пользователь, которому назначен рецензент обзора доступа, может управлять своими решениями без необходимости быть в роли каталога.

## <a name="see-also"></a>См. также

- [Учебники,](/graph/accessreviews-overview) чтобы узнать, как использовать API обзоров доступа для проверки доступа к ресурсам Azure AD
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

