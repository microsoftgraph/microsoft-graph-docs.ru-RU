---
title: Проверки доступа Azure AD (все ресурсы)
description: Вы можете использовать проверки доступа Azure AD, чтобы настроить однововременные или повторяющиеся проверки доступа для проверки прав доступа пользователя. Эта документация предназначена для устаревших API.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 0c616b20ac6c3dfc00ffdae319978a6bce60db5f
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292035"
---
# <a name="azure-ad-access-reviews-for-resources-excluding-groups"></a>Проверки доступа Azure AD (для ресурсов, кроме групп)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Вы можете использовать проверки [доступа Azure AD,](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) чтобы настроить однововременные или повторяющиеся проверки доступа для проверки прав доступа пользователя.

Типичные сценарии проверки доступа клиентов на членство в группах и доступ к приложениям:

- Клиенты могут просмотреть и сертифицировать доступ гостевых пользователей с помощью проверок доступа к приложениям и членствам в группах. Рецензенты могут использовать предоставленные сведения, чтобы эффективно решить, должны ли гости иметь постоянный доступ.

- Клиенты могут просмотреть и сертифицировать доступ сотрудников к приложениям и членствам в группах с помощью проверок доступа.

- Клиенты могут собирать средства контроля доступа в программы, релевантные для вашей организации, для отслеживания проверок соответствия требованиям или приложений, чувствительных к рискам.

Клиенты также могут просмотреть и сертифицировать назначения ролей административных пользователей, которым назначены роли Azure AD, такие как роли глобального администратора или подписки Azure.  Эта возможность включена в [Azure AD Privileged Identity Management.](privilegedidentitymanagement-root.md)

Обратите внимание, что функция проверки доступа, включая API, включена в Azure AD Premium P2.  У клиента, на котором создается проверка доступа, должна быть действительная приобретенная или пробная подписка на Azure AD Premium P2 или EMS E5.
Перед созданием проверки доступа, программы или управления программой администратор должен предварительно вошел в группу, чтобы подготовить ресурсы [programControlType](programcontroltype.md) и [businessFlowTemplate.](businessflowtemplate.md) Организация может присоединения к проверки доступа Azure AD или, в случае проверки доступа ролей Azure AD или ролей подписки Azure, Azure AD PIM.


## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с проверкой доступа.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
|[Get accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Получите отзыв о доступе с определенным ИД. |
|[Создание accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Создайте новый accessReview. |
|[Удаление accessReview](../api/accessreview-delete.md) | Нет.   | Удаление accessReview. |
|[Обновление accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Обновление accessReview. |
|[Список accessReviews](../api/accessreview-list.md) |    [Коллекция accessReview](accessreview.md) |    Список accessReviews для businessFlowTemplate. |
|[Список рецензентов accessReview](../api/accessreview-listreviewers.md) |      [Коллекция userIdentity](useridentity.md)| Получите проверяющих accessReview. |
|[Добавление рецензента accessReview](../api/accessreview-addreviewer.md) |      Нет.   |   Добавление рецензента в accessReview. |
|[Удаление рецензента accessReview](../api/accessreview-removereviewer.md) | Нет.  |   Удаление рецензента из accessReview. |
|[Список решений accessReview](../api/accessreview-listdecisions.md) |      [Коллекция accessReviewDecision](accessreviewdecision.md)| Получите решения accessReview.|
|[Список решений accessReview](../api/accessreview-listmydecisions.md) |     [Коллекция accessReviewDecision](accessreviewdecision.md)| Как рецензент получите мои решения по accessReview.|
|[Отправка напоминания accessReview](../api/accessreview-sendreminder.md) |        Нет.   |   Отправьте напоминание рецензентам accessReview. |
|[Остановка accessReview](../api/accessreview-stop.md) |     Нет.   |   Остановите accessReview. |
|[Сброс решений accessReview](../api/accessreview-reset.md) |     Нет.   |   Сброс решений в ходе выполнения accessReview.|
|[Применение решений accessReview](../api/accessreview-apply.md) |     Нет.   |   Применение решений из завершенного accessReview.|
|[Список businessFlowTemplates](../api/businessflowtemplate-list.md) | [Коллекция businessFlowTemplate](businessflowtemplate.md)| Получите шаблоны бизнес-потока, подходящие для получения доступа к отзывам.|
|[Создание программы](../api/program-create.md) |   [program](program.md)   |   Создайте новую программу.|
|[Удаление программы](../api/program-delete.md) |   Нет.   |   Удаление программы.|
|[Список программ](../api/program-list.md) |  [коллекция program](program.md)|   Получите коллекцию всех программ.|
|[Список programControls программы](../api/program-listcontrols.md) |      [Коллекция programControl](programcontrol.md)| Получите коллекцию элементов управления программы.|
|[Обновление программы](../api/program-update.md) |   [program](program.md)|  Обновление программы.|
|[Создание programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Добавьте programControl в программу.|
|[Удаление programControl](../api/programcontrol-delete.md) |     Нет.   |   Удалите programControl из программы.|
|[Список programControls](../api/programcontrol-list.md) | [Коллекция programControl](programcontrol.md)| Список элементов управления во всех программах в клиенте.|
|[Список programControlTypes](../api/programcontroltype-list.md) | [Коллекция programControlType](programcontroltype.md)| Список типов управления программой. |

## <a name="role-and-application-permission-authorization-checks"></a>Проверки авторизации разрешений ролей и приложений

Следующие роли каталога необходимы вызываемой пользователю для управления проверками доступа, программами и средствами управления.

| Целевой ресурс | Operation | Разрешения приложений | Требуемая роль каталога вызываемого пользователя |
|:----------------|:------------------|:------------|:--------------------------------------------|
|[accessReview](accessreview.md) роли Azure AD | Чтение | AccessReview.Read.All или AccessReview.ReadWrite.All | Глобальный администратор, глобальный читатель, администратор безопасности, читатель безопасности или администратор привилегированных ролей |
|[accessReview](accessreview.md) роли Azure AD | Создание, обновление или удаление | AccessReview.ReadWrite.All | Глобальный администратор или администратор привилегированных ролей |
|[accessReview](accessreview.md) группы или приложения | Чтение | AccessReview.Read.All, AccessReview.ReadWrite.Membership или AccessReview.ReadWrite.All | Глобальный администратор, глобальный читатель, администратор безопасности, читатель безопасности или администратор пользователя |
|[accessReview](accessreview.md) группы или приложения | Создание, обновление или удаление | AccessReview.ReadWrite.Membership или AccessReview.ReadWrite.All | Глобальный администратор или администратор пользователей |
| [program](program.md) и [programControl](programcontrol.md)| Чтение | ProgramControl.Read.All или ProgramControl.ReadWrite.All |  Глобальный администратор, глобальный читатель, администратор безопасности, читатель безопасности или администратор пользователя |
| [program](program.md) и [programControl](programcontrol.md) | Создание, обновление или удаление | ProgramControl.ReadWrite.All | Глобальный администратор или администратор пользователей |

Кроме того, пользователь, который является назначенным рецензентом проверки доступа, может управлять своими решениями без необходимости быть в роли каталога.

## <a name="see-also"></a>См. также

- [Как администратор может управлять доступом пользователей с помощью проверок доступа Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Как администратор может управлять гостевим доступом с помощью проверок доступа Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [Как администратор может управлять программами и средствами управления для проверки доступа Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


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


