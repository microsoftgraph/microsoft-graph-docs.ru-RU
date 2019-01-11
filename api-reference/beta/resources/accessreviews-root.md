---
title: Дается обзор доступа Microsoft Azure AD
description: Можно использовать Azure AD доступ к обзоры для настройки доступа однократное или повторяющееся обзоры для аттестации права доступа.
localization_priority: Normal
ms.openlocfilehash: 259a88bf95bfe0796e0ee46dd2d0a64c68831a64
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860790"
---
# <a name="azure-ad-access-reviews"></a>Дается обзор доступа Microsoft Azure AD

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

[Дается обзор Azure AD access](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) можно использовать для настройки одноразовый или дается обзор повторяющихся доступа для аттестации права доступа.

Рассматриваются типичные клиента сценарии для доступа к членства в группе и доступ к приложениям:
   
- Клиенты можно просматривать и сертификация гостевой доступ пользователей с помощью access обзоры их доступа к приложениям и членство в группах для группы. Рецензенты могут использовать средствами, которые предоставляются для эффективно решить, следует ли гости имеют постоянный доступ.
      
- Клиенты можно просматривать и сертификация сотрудников доступ к приложениям и членство в группах с обзоры доступа.
   
- Пользователи могут собирать Обзор управления доступом в программ, которые относятся к вашей организации для отслеживания обзоры для соответствия требованиям или риска-приложений.

Это также связанных с ними возможность для клиентов для просмотра и сертификация назначения роли администратора пользователей, которым назначена ролям Azure AD, такие как роли глобального администратора или Azure подписки.  Эта возможность включена в [Azure AD привилегированной управления удостоверениями](privilegedidentitymanagement-root.md).

Обратите внимание, что функции проверки доступа, в том числе к интерфейсам API, включен в P2 Azure AD Premium. 

## <a name="methods"></a>Methods

Ниже приведен список методов, предоставляемых Azure AD доступ к обзоры.  

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Получите обзор доступа с определенным идентификатором. |
|[Создание accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Создание нового accessReview. |
|[Удаление accessReview](../api/accessreview-delete.md) | Нет.   | Удалите accessReview. |
|[Обновление accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Обновление accessReview. |
|[Список accessReview рецензентов](../api/accessreview-listreviewers.md) |      Коллекция [удостоверению пользователя](useridentity.md)| Получите рецензентов accessReview. |
|[Добавление accessReview редактор](../api/accessreview-addreviewer.md) |      Нет.   |   Добавьте проверяющий accessReview. |
|[Удаление accessReview редактор](../api/accessreview-removereviewer.md) | Нет.  |   Удаление рецензента из accessReview. |
|[Список accessReview решения](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md) коллекции| Получите решения accessReview.|
|[Мои accessReview решения](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md) коллекции| В качестве читателя получите Мои решения accessReview.|
|[Отправлять напоминание accessReview](../api/accessreview-sendreminder.md) |        Нет.   |   Отправьте напоминание, чтобы проверяющие accessReview. |
|[Остановка accessReview](../api/accessreview-stop.md) |     Нет.   |   Остановите accessReview. |
|[Сброс accessReview решения](../api/accessreview-reset.md) |     Нет.   |   Сброс решения, принимаемые при accessReview в хода выполнения.|
|[Применение accessReview решения](../api/accessreview-apply.md) |     Нет.   |   Применение решения из завершенных accessReview.|
|[Список businessFlowTemplates](../api/businessflowtemplate-list.md) | [businessFlowTemplate](businessflowtemplate.md) коллекции| Получение шаблонов поток business подходят для доступа к обзоры.|
|[Создание программы](../api/program-create.md) |   [Программа](program.md)   |   Создание программы.|
|[Удаление программы](../api/program-delete.md) |   Нет.   |   Удаление программы.|
|[Список программ](../api/program-list.md) |  [программа](program.md) семейства сайтов|   Получите коллекцию всех программ.|
|[Список programControls программы](../api/program-listcontrols.md) |      [programControl](programcontrol.md) коллекции| Получите коллекцию элементов управления из программы.|
|[Обновите программу](../api/program-update.md) |   [Программа](program.md)|  Обновите программу.|
|[Создание programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Добавьте programControl программы.|
|[Удаление programControl](../api/programcontrol-delete.md) |     Нет.   |   Удалите programControl из программы.|
|[Список programControls](../api/programcontrol-list.md) | [programControl](programcontrol.md) коллекции| Список элементов управления для всех программ в клиентов.|
|[Список programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md) коллекции| Список типов элементов управления программы. |


## <a name="see-also"></a>См. также

- [Как администратор может управлять доступом пользователей с доступом Azure AD дается обзор](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Как администратор может управлять гостевой доступ с доступом Azure AD дается обзор](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [Как администратор может управлять программы и обзоры доступ к элементам управления для Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
