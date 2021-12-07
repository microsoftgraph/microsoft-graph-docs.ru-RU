---
title: Настройка конфиденциальности для аналитики пользователей в Microsoft Graph
description: Узнайте, как настроить параметры аналитики пользователей на уровне организации с помощью API Microsoft GRAPH.
author: anthona
ms.localizationpriority: high
ms.prod: insights
ms.custom: scenarios:getting-started
ms.openlocfilehash: e0495f4206023c6d7c8a46f094172e5732c08df4
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322728"
---
# <a name="customizing-people-insights-privacy-in-microsoft-graph-preview"></a>Настройка конфиденциальности для аналитики пользователей в Microsoft Graph (предварительная версия)

Аналитика пользователей содержит сведения о связях между сотрудниками, которые [релевантны друг относительно друга или вместе работают](people-example.md#including-a-person-as-relevant-or-working-with) в пределах организации, на основе отношений между людьми. Эти сведения могут отображаться в Delve и карточке профиля, и их возвращает [API People](/graph/api/user-list-people?view=graph-rest-beta&preserve-view=true).


## <a name="customizing-people-insights-for-an-organization"></a>Настройка аналитики пользователей в организации

По умолчанию для организации включено отображение или возврат аналитики пользователей. Администраторы с ролью глобального администратора могут настроить эти параметры для своей организации с помощью API REST и соответствующих разрешений. Для этого свойства ресурса [insightsSettings](/graph/api/resources/insightssettings?view=graph-rest-beta&preserve-view=true) устанавливаются следующим образом:

- Чтобы отключить аналитику пользователей для всех сотрудников организации, нужно задать для свойства **isEnabledInOrganization** ресурса **insightsSettings** значение `false`. (По умолчанию для свойства **isEnabledInOrganization** задано значение `true`.)

- Чтобы отключить аналитику пользователей для некоторого подмножества пользователей, нужно назначить их группе Azure Active Directory (Azure AD) и установить для свойства **disabledForGroup** значение идентификатора этой группы. Подробнее о [создании групп и добавлении пользователей в качестве участников](/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal). 

Настроить свойства **isEnabledInOrganization** и **disabledForGroup** аналитики пользователей можно с помощью операции обновления [update](/graph/api/insightssettings-update?view=graph-rest-beta&preserve-view=true). 

При обновлении параметров элемента Insights учитывайте следующее: 
* Параметры аналитики пользователей доступны только в бета-версии конечной точки. 
* Операция обновления не проверяет существование группы. Убедитесь, что получили правильный идентификатор группы Azure AD с портала Azure, а также проверьте ее существование и тот факт, что в нее добавлены необходимые пользователи. Если группа не существует, в параметры пользователей организации не будет внесено никаких изменений. 
* При обновлении **insightsSettings** отображение изменений может занять до 24 часов, а иногда дольше. 

## <a name="behavior-changes-in-the-microsoft-365-ui-and-people-api"></a>Изменения поведения в пользовательском интерфейсе Microsoft 365 и API People 

Отключение аналитики пользователей означает, что соответствующие данные для указанного пользователя не создаются. Это никак не затрагивает поиск и ранжирование результатов.

При настройке конфиденциальности для аналитики пользователей можно наблюдать изменения поведения в следующих областях:
* [Карточка профиля](https://support.microsoft.com/office/profile-cards-in-microsoft-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) Microsoft 365
* Профиль пользователя в Delve
* [Списки релевантных пользователей](/graph/api/user-list-people?view=graph-rest-beta&preserve-view=true)

