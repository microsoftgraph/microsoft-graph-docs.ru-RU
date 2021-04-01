---
title: Отзывы о доступе к Azure AD — устаревшие
description: Вы можете использовать обзоры доступа Azure AD для настройки одновеких или повторяющихся обзоров доступа для проверки прав доступа пользователя. Эта документация служит устаревшим API.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: dcdfc94b3605b701f09f559c19e8975acf73a63d
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51474091"
---
# <a name="azure-ad-access-reviews-legacy"></a>Обзоры доступа к Azure AD (устаревшие)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Вы можете использовать обзоры доступа [Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) для настройки одновеких или повторяющихся обзоров доступа для проверки прав доступа пользователя.

Типичные сценарии клиентского доступа к отзывам о членстве в группе и доступе к приложениям:

- Клиенты могут просмотреть и сертифицировать гостевой доступ пользователей с помощью обзоров доступа к приложениям и членствам групп. Рецензенты могут использовать сведения, предоставляемые для эффективного решения о том, следует ли гостям иметь постоянный доступ.

- Клиенты могут просмотреть и сертифицировать доступ сотрудников к приложениям и членам групп с помощью отзывов о доступе.

- Клиенты могут собирать элементы управления обзором доступа в программы, релевантные для организации, для отслеживания отзывов на соответствие требованиям или приложений, чувствительных к риску.

Кроме того, клиенты могут выполнять проверку и сертификацию назначений ролей административных пользователей, которым назначены роли Azure AD, такие как роли глобального администратора или подписки Azure.  Эта возможность включена в [Azure AD Privileged Identity Management.](privilegedidentitymanagement-root.md)

Обратите внимание, что функция обзоров доступа, включая API, включена в Azure AD Premium P2.  Клиент, на котором создается обзор доступа, должен иметь допустимую приобретенную или пробную подписку Azure AD Premium P2 или EMS E5.
Перед созданием обзора доступа, управления программой или программой администратор должен быть ранее на борту, чтобы подготовить ресурсы [programControlType](programcontroltype.md) и [businessFlowTemplate.](businessflowtemplate.md) Организация может получать отзывы о доступе к Azure AD или в случае отзывов доступа к ролям Azure AD или ролям подписки Azure AD PIM.


## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с обзором доступа.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
|[Получить accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Получите обзор доступа с определенным ИД. |
|[Создание accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Создание нового accessReview. |
|[Удаление accessReview](../api/accessreview-delete.md) | Нет.   | Удаление accessReview. |
|[Обновление accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Обновление accessReview. |
|[AccessReviews списка](../api/accessreview-list.md) |    [коллекция accessReview](accessreview.md) |    Список accessReviews для businessFlowTemplate. |
|[Рецензенты списка accessReview](../api/accessreview-listreviewers.md) |      [коллекция userIdentity](useridentity.md)| Получите рецензентов accessReview. |
|[Добавление рецензента accessReview](../api/accessreview-addreviewer.md) |      Нет.   |   Добавление рецензента в accessReview. |
|[Удаление рецензента accessReview](../api/accessreview-removereviewer.md) | Нет.  |   Удаление рецензента из accessReview. |
|[Списки решений accessReview](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md) collection| Получите решения accessReview.|
|[Список решений accessReview](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md) collection| Как рецензент, получите мои решения accessReview.|
|[Отправка напоминания accessReview](../api/accessreview-sendreminder.md) |        Нет.   |   Отправьте напоминание рецензентам accessReview. |
|[Остановка accessReview](../api/accessreview-stop.md) |     Нет.   |   Остановите accessReview. |
|[Сброс решений accessReview](../api/accessreview-reset.md) |     Нет.   |   Сброс решений в ходе выполнения accessReview.|
|[Применение решений accessReview](../api/accessreview-apply.md) |     Нет.   |   Применение решений из завершенного accessReview.|
|[Список businessFlowTemplates](../api/businessflowtemplate-list.md) | [коллекция businessFlowTemplate](businessflowtemplate.md)| Получите шаблоны бизнес-потока, подходящие для доступа к отзывам.|
|[Создание программы](../api/program-create.md) |   [программа](program.md)   |   Создание новой программы.|
|[Удаление программы](../api/program-delete.md) |   Нет.   |   Удаление программы.|
|[Списки программ](../api/program-list.md) |  [коллекция](program.md) программ|   Получите коллекцию всех программ.|
|[Список программКонтроли программы](../api/program-listcontrols.md) |      [коллекция programControl](programcontrol.md)| Получите коллекцию элементов управления программы.|
|[Программа обновления](../api/program-update.md) |   [программа](program.md)|  Обновление программы.|
|[Создание programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Добавьте программуControl в программу.|
|[Удаление программыControl](../api/programcontrol-delete.md) |     Нет.   |   Удаление программыControl из программы.|
|[List programControls](../api/programcontrol-list.md) | [коллекция programControl](programcontrol.md)| Элементы управления списками для всех программ в клиенте.|
|[List programControlTypes](../api/programcontroltype-list.md) | [коллекция programControlType](programcontroltype.md)| Типы управления программами списка. |

## <a name="role-and-application-permission-authorization-checks"></a>Проверки авторизации ролей и разрешений на приложения

Для управления отзывами, программами и средствами управления пользователями доступа требуются следующие роли каталога.

| Целевой ресурс | Операция | Разрешения приложений | Роль требуемого каталога вызываемого пользователя |
|:----------------|:------------------|:------------|:--------------------------------------------|
|[accessReview](accessreview.md) роли Azure AD | Чтение | AccessReview.Read.All или AccessReview.ReadWrite.All | Глобальный администратор, глобальный читатель, администратор безопасности, читатель безопасности или администратор привилегированных ролей |
|[accessReview](accessreview.md) роли Azure AD | Создание, обновление или удаление | AccessReview.ReadWrite.All | Глобальный администратор или администратор привилегированных ролей |
|[accessReview](accessreview.md) группы или приложения | Чтение | AccessReview.Read.All, AccessReview.ReadWrite.Membership или AccessReview.ReadWrite.All | Глобальный администратор, глобальный читатель, администратор безопасности, читатель безопасности или администратор пользователей |
|[accessReview](accessreview.md) группы или приложения | Создание, обновление или удаление | AccessReview.ReadWrite.Membership или AccessReview.ReadWrite.All | Глобальный администратор или администратор пользователей |
| [program](program.md) and [programControl](programcontrol.md)| Чтение | ProgramControl.Read.All или ProgramControl.ReadWrite.All |  Глобальный администратор, глобальный читатель, администратор безопасности, читатель безопасности или администратор пользователей |
| [program](program.md) and [programControl](programcontrol.md) | Создание, обновление или удаление | ProgramControl.ReadWrite.All | Глобальный администратор или администратор пользователей |

Кроме того, пользователь, которому назначен рецензент обзора доступа, может управлять своими решениями без необходимости быть в роли каталога.

## <a name="see-also"></a>См. также

- [Управление доступом к пользователю с помощью отзывов о доступе к Azure AD администратору](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Управление гостевых доступом администратора с помощью отзывов о доступе к Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [Управление программами и средствами управления для отзывов о доступе к Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


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


