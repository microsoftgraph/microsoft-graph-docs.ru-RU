---
title: Настройка конфиденциальности для аналитики пользователей в Microsoft Graph (предварительная версия)
description: Узнайте о настройке аналитики пользователей на уровне организации с помощью Microsoft Graph insightsSettings API.
author: anthona
ms.localizationpriority: high
ms.prod: insights
ms.custom: scenarios:getting-started
ms.openlocfilehash: da5306a4bc92a0e475c4785eea124f78d18f9fed
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438292"
---
# <a name="customize-people-insights-privacy-in-microsoft-graph-preview"></a>Настройка конфиденциальности для аналитики пользователей в Microsoft Graph (предварительная версия)

Аналитика пользователей содержит сведения о связях между сотрудниками, которые [релевантны друг относительно друга или вместе работают](people-example.md#including-a-person-as-relevant-or-working-with) в пределах организации, на основе отношений между людьми. Эти сведения могут отображаться в Delve и карточке профиля, и их возвращает [API People](/graph/api/user-list-people).


## <a name="customize-people-insights-for-an-organization"></a>Настройка аналитики пользователей в организации

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
* [Списки релевантных пользователей](/graph/api/user-list-people)