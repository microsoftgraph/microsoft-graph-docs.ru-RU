---
title: Обзоры Azure AD Access — бета-версия обновления
description: Вы можете использовать обзоры Azure AD, чтобы настроить однократные или повторяющиеся проверки доступа для подтверждения прав доступа пользователя. Эта документация служит второй версией API.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 44bdd534aeb36ad85133fe1ab26006150328e926
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001039"
---
# <a name="azure-ad-access-reviews"></a>Проверки доступа Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>В этой документации представлена последняя поддерживаемая версия API просмотров Access для рецензирования в группах Microsoft 365. Обзоры других ресурсов можно найти в статьях [API для рецензирования Access](accessreviews-root.md).
>
>В настоящее время API Microsoft Graph поддерживает только обзоры доступа к группам.

Вы можете использовать [обзоры Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) , чтобы настроить однократные или повторяющиеся проверки доступа для подтверждения прав доступа пользователя.

Типичные сценарии клиентов для проверки членства в группах и доступа к приложениям:

- Пользователи могут просматривать и сертифицировать гостевой доступ, используя обзоры доступа к приложениям и группам. Проверяющие могут использовать аналитику, которая позволяет эффективно определять, должен ли гостям доступ.

- Пользователи могут просматривать и сертифицировать доступ сотрудников к приложениям и членству в группах с помощью рецензирования Access.

- Пользователи могут собирать элементы управления проверкой доступа в программы, которые соответствуют требованиям организации для отслеживания проверок на соответствие требованиям и приложениям, учитывающим риск.

Кроме того, у пользователей есть возможность просматривать и сертифицировать назначения ролей для пользователей, которым назначены роли Azure AD, такие как глобальный администратор или роли подписки Azure.  Эта возможность включена в [Azure AD с правами привилегированного управления идентификацией](privilegedidentitymanagement-root.md).

Обратите внимание, что функция рецензирования доступа, включая API, включена в Azure AD Premium P2.  Клиент, на котором создается проверка доступа, должен иметь допустимую приобретенную или пробную подписку на Azure AD Premium P2 или EMS.


## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с проверкой доступа.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
|[Список Акцессревиевсчедуледефинитион](../api/accessreviewscheduledefinition-list.md) | Коллекция [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) | Перечисляет все `accessReviewScheduleDefinition` . Не включает связанные `accessReviewInstance` экземпляры в вхождениях. |
|[Получение Акцессревиевсчедуледефинитион](../api/accessreviewscheduledefinition-get.md) | [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) | Получение объекта `accessReviewScheduleDefinition` с указанным идентификатором. |
|[Создание Акцессревиевсчедуледефинитион](../api/accessreviewscheduledefinition-create.md) | [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) | Создание объекта `accessReviewScheduleDefinition`. |
|[Удаление Акцессревиевсчедуледефинитион](../api/accessreviewscheduledefinition-delete.md) | Нет. | Удаление объекта `accessReviewScheduleDefinition` с указанным идентификатором. |
|[Обновление Акцессревиевсчедуледефинитион](../api/accessreviewscheduledefinition-update.md) | Нет. | Обновление свойств объекта `accessReviewScheduleDefinition` с указанным идентификатором. |
|[Список Акцессревиевинстанце](../api/accessreviewinstance-list.md) | Коллекция [акцессревиевинстанце](accessreviewinstance.md) | Перечисляет все `accessReviewInstance` для определенных `accessReviewScheduleDefinition` . Не включает связанные `accessReviewInstanceDecisionItem` с s элементы s в вхождения. |
|[Получение Акцессревиевинстанце](../api/accessreviewinstance-get.md) | [акцессревиевинстанце](accessreviewinstance.md) | Возвращает значение `accessReviewInstance` `accessReviewScheduleDefinition` . Не включает связанные `accessReviewInstanceDecisionItem` элементы s в объект. |
|[Список ожидающих утверждения Акцессревиевинстанцес](../api/accessreviewinstance-pendingaccessreviewinstances.md) | Коллекция [акцессревиевинстанце](accessreviewinstance.md) . | Получение всех `accessReviewInstance` пользователей, назначенных вызывающему пользователю. |
|[Отправка напоминания о Акцессревиевинстанце](../api/accessreviewinstance-sendreminder.md) | Нет. | Отправка напоминания рецензентам `accessReviewInstance` . |
|[Остановить Акцессревиевинстанце](../api/accessreviewinstance-stop.md) | Нет. | Вручную остановить `accessReviewInstance` . |
|[Принятие рекомендаций](../api/accessreviewinstance-acceptrecommendations.md) | Нет. | Позволяет вызывающему пользователю принимать рекомендации по решению для каждого Нотревиевед `accessReviewInstanceDecisionItem` , для которого они являются проверяющими для определенного `accessReviewInstance` . |
|[Применение решений](../api/accessreviewinstance-applydecisions.md) | Нет. | Вручную примените решение для `accessReviewInstance` . |
|[Список АкцессревиевинстанцедеЦисионитемс](../api/accessreviewinstancedecisionitem-list.md) | Коллекция [акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem.md) | Перечисляет все `accessReviewInstanceDecisionItem` для определенных `accessReviewInstance` . |
|[Список ожидающих утверждения АкцессревиевинстанцедеЦисионитемс](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | Коллекция [акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem.md) . | Получение всех `accessReviewInstanceDecisionItems` пользователей, назначенных вызывающему пользователю, для определенного пользователя `accessReviewInstance` . |
|[Обновление АкцессревиевинстанцедеЦисионитем](../api/accessreviewinstancedecisionitem-update.md) | Нет. | Для того `accessReviewInstanceDecisionItems` , чтобы вызывающий пользователь был назначен проверяющему, вызываемый пользователь может записать решение путем исправления объекта решения. |

## <a name="role-and-application-permission-authorization-checks"></a>Проверки авторизации разрешений для ролей и приложений

Чтобы вызывающий пользователь управлялся проверками доступа, необходимо иметь следующие роли каталогов. Обратите внимание, что в настоящее время в API Microsoft Graph поддерживаются только обзоры для доступа к группам.

| Операция | Разрешения приложений | Требуемая роль каталога вызывающего пользователя |
|:------------------|:------------|:--------------------------------------------|
| Чтение | Акцессревиев. Read. ALL или Акцессревиев. ReadWrite. ALL | Глобальный администратор, глобальный читатель, администратор безопасности, средство чтения безопасности или администратор пользователей |
| Создание, обновление или удаление | AccessReview.ReadWrite.All | Глобальный администратор или администратор пользователей |

Кроме того, пользователь, который является назначенным рецензентом проверки доступа, может управлять своими решениями без необходимости их использования в роли каталога.

## <a name="see-also"></a>См. также

- [Как администратор может управлять доступом пользователей с помощью проверок доступа Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Как администратор может управлять гостевым доступом с помощью проверок Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)


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


