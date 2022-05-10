---
title: Работа с группами в Microsoft Graph
description: Группы — это коллекции участников с совместным доступом к ресурсам в службах Майкрософт или ваших приложениях. В состав групп могут входить различные участники, такие как пользователи, другие группы, устройства и приложения. Использование групп помогает избежать работы с отдельными участниками и упрощает управление доступом к ресурсам.
author: psaffaie
ms.localizationpriority: high
ms.prod: groups
doc_type: conceptualPageType
ms.openlocfilehash: 87288533896622d6e9765f9572540fb8632725d5
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296523"
---
# <a name="working-with-groups-in-microsoft-graph"></a>Работа с группами в Microsoft Graph

Группы — это коллекции участников с совместным доступом к ресурсам в службах Майкрософт или ваших приложениях. В состав групп могут входить различные участники, такие как пользователи, другие группы, устройства и приложения. Использование групп помогает избежать работы с отдельными участниками и упрощает управление доступом к ресурсам.

Microsoft Graph предоставляет API групп для создания и управления различными типами групп и функциональностью групп. 

> [!NOTE]
> 1. Группы можно создавать только с помощью рабочих или учебных учетных записей. Личные учетные записи Майкрософт не поддерживают группы.
> 2. Для всех операций с группами в Microsoft Graph необходимо согласие администратора.

## <a name="group-types-in-azure-ad-and-microsoft-graph"></a>Типы групп в Azure AD и Microsoft Graph

Azure Active Directory (Azure AD) поддерживает следующие типы групп.

- Группы Microsoft 365
- Группы безопасности
- группы безопасности с включенной поддержкой почты.
- Группы рассылки

> [!NOTE]
> Microsoft также поддерживает [динамические группы рассылки](/exchange/recipients/dynamic-distribution-groups/dynamic-distribution-groups?view=exchserver-2019), которыми нельзя управлять или извлекать их через Microsoft Graph.

Через API групп Microsoft Graph можно управлять только Microsoft 365 и группами безопасности. Почтовые группы и группы рассылки доступны только для чтения через Microsoft Graph.

В Microsoft Graph тип группы можно определить с помощью параметров ее свойств **groupType**, **mailEnabled** и **securityEnabled**, как указано в таблице ниже.

| Тип |groupType | mailEnabled | securityEnabled | Создано и управляется с помощью API групп |
|--|--|--|--|--|
| [Группы Microsoft 365](#microsoft-365-groups) | `["Unified"]` | `true` | `true` или `false` | Да |
| [Группы безопасности](#security-groups-and-mail-enabled-security-groups) | `[]` | `false` | `true` | Да |
| [Группы безопасности, поддерживающие почту](#security-groups-and-mail-enabled-security-groups) | `[]` | `true` | `true` | Нет |
| Группы рассылки | `[]` | `true` | `false` | Нет |

Дополнительные сведения о группах см. в разделах ниже. Дополнительные сведения о группах в Azure AD см. в разделе [Сравнение групп в Azure AD](/microsoft-365/admin/create-groups/compare-groups).

## <a name="microsoft-365-groups"></a>Группы Microsoft 365

Группы Microsoft 365 лучше всего проявляют себя при совместной работе над проектом или в команде. Они создаются с ресурсами, доступными всем участникам, включая:

- беседы Outlook;
- календарь Outlook;
- файлы SharePoint;
- записную книжку OneNote;
- сайт группы SharePoint;
- планы для планировщика;
- средства управления устройствами Intune.

В следующем объекте JSON показано примерное представление группы при вызове API групп Microsoft Graph.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "4c5ee71b-e6a5-4343-9e2c-4244bc7e0938",
    "deletedDateTime": null,
    "classification": "MBI",
    "createdDateTime": "2016-08-23T14:46:56Z",
    "description": "This is a group in Outlook",
    "displayName": "OutlookGroup101",
    "groupTypes": [
        "Unified"
    ],
    "mail": "outlookgroup101@service.microsoft.com",
    "mailEnabled": true,
    "mailNickname": "outlookgroup101",
    "preferredLanguage": null,
    "proxyAddresses": [
        "smtp:outlookgroup101@microsoft.onmicrosoft.com",
        "SMTP:outlookgroup101@service.microsoft.com"
    ],
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```

Дополнительные сведения о группах Microsoft 365 и интерфейсах для администраторов см. в статье [Дополнительные сведения о группах Microsoft 365](https://support.office.com/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).

## <a name="security-groups-and-mail-enabled-security-groups"></a>Группы безопасности (обычные и поддерживающие почту)

**Группы безопасности** предназначены для управления доступом пользователей к ресурсам. Проверяя, является ли пользователь членом группы безопасности, приложение может принимать решения касательно авторизации, когда пользователь пытается получить доступ к защищенным ресурсам в приложении. В группы безопасности могут входить пользователи, другие группы безопасности, устройства и субъекты-службы.

**Группы безопасности с включенной поддержкой почты** используются так же, как и группы безопасности, но с добавленной функцией общего почтового ящика. Группы безопасности с включенной поддержкой почты нельзя создавать или обновлять с помощью API. Вместо этого они доступны только для чтения. Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange](/Exchange/recipients/mail-enabled-security-groups).

В следующем объекте JSON показано примерное представление группы при вызове API групп Microsoft Graph.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.group",
    "id": "f87faa71-57a8-4c14-91f0-517f54645106",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2016-07-20T09:21:23Z",
    "description": "This group is a Security Group",
    "displayName": "SecurityGroup101",
    "groupTypes": [],
    "mail": null,
    "mailEnabled": false,
    "mailNickname": "",
    "preferredLanguage": null,
    "proxyAddresses": [],
    "securityEnabled": true
}
```

## <a name="dynamic-membership"></a>Динамическое членство

Для любых групп можно задавать правила динамического членства, которые автоматически добавляют или удаляют членов группы в соответствии со свойствами участников. Например, группа «Сотрудники по маркетингу» может определить правило динамического членства, согласно которому только пользователи со свойством отдела, установленным на «Маркетинг», могут быть членами группы. В этом случае любой пользователь, покидающий отдел, автоматически удаляется из группы. 

Правила динамического членства задаются с помощью свойства **membershipRule** во время создания группы. Например, `"membershipRule": 'user.department -eq "Marketing"'`. Свойство **groupType** также должно включать значение `"DynamicMembership"` в коллекцию. Правило динамического членства можно включить или отключить с помощью свойства **membershipRuleProcessingState**.

В следующем примере запроса создается новая группа Microsoft 365, в которую могут входить только сотрудники отдела маркетинга.

```http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json

{
    "description": "Marketing department folks",
    "displayName": "Marketing department",
    "groupTypes": [
        "Unified",
        "DynamicMembership"
    ],
    "mailEnabled": true,
    "mailNickname": "marketing",
    "securityEnabled": false,
    "membershipRule": "'user.department -eq 'Marketing'",
    "membershipRuleProcessingState": "on"
}
```

Дополнительные сведения о составлении правил участия см. в статье [Правила динамического членства для групп в Azure Active Directory](/azure/active-directory/enterprise-users/groups-dynamic-membership).

> **Примечание**. Правила динамического членства требуют, чтобы у клиента была как минимум лицензия Azure AD Premium P1 для каждого уникального пользователя, являющегося членом одной или нескольких динамических групп.

## <a name="other-types-of-groups"></a>Группы других типов

Группы Microsoft 365 в Yammer используются для организации совместной работы пользователей с помощью записей Yammer. Группы такого типа можно возвращать с помощью запроса на чтение, но записи из них недоступны через API. Если в группе включены записи и каналы бесед Yammer, то стандартные групповые беседы Microsoft 365 отключены. Дополнительные сведения см. в [документах, посвященных API Yammer для разработчиков](https://developer.yammer.com/docs).

## <a name="group-search-limitations-for-guest-users-in-organizations"></a>Ограничения на поиск групп для гостевых пользователей в организациях

Функции поиска групп позволяют приложению найти любую группу в каталоге организации с помощью запросов для ресурса `/groups` (например, `https://graph.microsoft.com/beta/groups`). Эта возможность доступна администраторам и пользователям, которые являются участниками. Однако это недоступно гостевым пользователям.

Если пользователь вошел как гость, в зависимости от предоставленных приложению разрешений оно может прочитать профиль определенной группы (например, `https://graph.microsoft.com/beta/group/fc06287e-d082-4aab-9d5e-d6fd0ed7c8bc`). Но оно не может отправлять ресурсу `/groups` запросы, способные возвращать несколько ресурсов.

При наличии подходящих разрешений приложение может читать профили групп, которые оно получает благодаря ссылкам в свойствах навигации (например, `/groups/{id}/members`).

Дополнительные сведения о том, что гостевые пользователи могут делать с группами, см. в разделе [Сравнение стандартных разрешений участника и гостя](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions).

## <a name="group-based-licensing"></a>Лицензирование на основе групп

С помощью возможности лицензирования на основе групп можно назначить одну или несколько лицензий на продукты группе Azure AD. Azure AD обеспечит назначение лицензий всем участникам этой группы. Всем новым участникам, присоединившимся к группе, назначаются соответствующие лицензии. При выходе участников из группы эти лицензии удаляются. Эту возможность можно использовать только с группами безопасности и группами Microsoft 365, в которых для свойства **securityEnabled** задано значение `true`. Дополнительные сведения о лицензировании на основе групп см. в статье [Что такое лицензии групп в Azure Active Directory?](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal?context=/azure/active-directory/enterprise-users/context/ugr-context).

## <a name="common-use-cases-for-the-groups-api-in-microsoft-graph"></a>Распространенные варианты использования API групп в Microsoft Graph

Ниже перечислены некоторые распространенные операции с группами, которые можно выполнять с помощью Microsoft Graph.

| **Варианты использования** | **Ресурсы REST** | **См. также** |
|:-|:-|:-|
| **Создание групп, управление характеристиками групп** |  |  |
| Создание новых групп и получение существующих, обновление свойств и удаление групп. В настоящее время с помощью API можно создавать только группы безопасности и группы Outlook. | [group](group.md) | [Создание групп](../api/group-post-groups.md) <br/> [Перечисление групп](../api/group-list.md) <br/> [Обновление групп](../api/group-update.md) <br/> [Удаление групп](../api/group-delete.md) |
| **Управление членством в группах** |  |  |
| Перечисление, добавление и удаление членов групп. | [user](user.md) <br/> [group](group.md) | [Перечисление членов](../api/group-list-members.md) <br/> [Добавление члена](../api/group-post-members.md) <br/> [Удаление члена](../api/group-delete-members.md) |
| Проверка членства пользователя в группе, получение всех групп, в которых состоит пользователь. | [user](user.md) <br/> [group](group.md) <br/> [servicePrincipal](serviceprincipal.md) <br/> [orgContact](orgcontact.md) | [Проверка членства в группах](../api/directoryobject-checkmembergroups.md) <br/> [Получение групп пользователя](../api/directoryobject-getmembergroups.md) |
| Перечисление, добавление и удаление владельцев группы. | [user](user.md) <br/> [group](group.md) | [Перечисление владельцев](../api/group-list-members.md) <br/> [Добавление члена](../api/group-post-members.md) <br/> [Удаление участника](../api/group-delete-members.md) |

## <a name="whats-new"></a>Новые возможности

Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для API групп.