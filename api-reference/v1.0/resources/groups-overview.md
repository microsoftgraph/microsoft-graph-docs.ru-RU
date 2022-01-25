---
title: Работа с группами в Microsoft Graph
description: Группы — это коллекции пользователей и других субъектов, у которых есть общий доступ к ресурсам в службах Майкрософт или в вашем приложении. Microsoft Graph предоставляет интерфейсы API, с помощью которых можно создавать разнообразные группы и их функции, а также управлять ими в соответствии с конкретным случаем. Для всех операций с группами в Microsoft Graph необходимо согласие администратора.
author: Jordanndahl
ms.localizationpriority: high
ms.prod: groups
doc_type: conceptualPageType
ms.openlocfilehash: bb455ffde8ab93ed0c93fcb35cdb088f2ce6979f
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201696"
---
# <a name="working-with-groups-in-microsoft-graph"></a>Работа с группами в Microsoft Graph

Группы — это коллекции [пользователей](user.md) и других субъектов, у которых есть общий доступ к ресурсам в службах Майкрософт или в вашем приложении. Microsoft Graph предоставляет интерфейсы API, с помощью которых можно создавать разнообразные группы и их функции, а также управлять ими в соответствии с конкретным случаем. Для всех операций с группами в Microsoft Graph необходимо согласие администратора.

> **Примечание.** Создавать группы можно только с помощью рабочих или учебных учетных записей. Личные учетные записи Майкрософт не поддерживают группы.

## <a name="group-types-in-azure-ad-and-microsoft-graph"></a>Типы групп в Azure AD и Microsoft Graph

Azure AD поддерживает следующие типы групп.

+ Группы Microsoft 365
+ Группы безопасности
+ группы безопасности с включенной поддержкой почты.
+ Группы рассылки

Дополнительные сведения о группах Azure AD см. в разделе [Сравнение групп в Azure AD](/microsoft-365/admin/create-groups/compare-groups).

В Microsoft Graph тип группы можно определить с помощью параметров ее свойств **groupType**, **mailEnabled** и **securityEnabled**, как указано в таблице ниже.

| Тип              | Вариант использования | groupType | mailEnabled | securityEnabled | Создано и управляется с помощью API |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [Группы Microsoft 365](#microsoft-365-groups) | Обеспечение совместной работы пользователей с общими ресурсами Майкрософт в Интернете. | `["Unified"]` | `true` | `true` или `false` | Да |
| [Группы безопасности](#security-groups-and-mail-enabled-security-groups) | Управление доступом пользователей к ресурсам в приложении. | `[]` | `false` | `true` | Да |
| [Группы безопасности, поддерживающие почту](#security-groups-and-mail-enabled-security-groups) | Управление доступом пользователей к ресурсам в приложении с общим почтовым ящиком группы. | `[]` | `true` | `true` | Нет |
| Группы рассылки | Рассылка почты участникам группы. Рекомендуем использовать группы Microsoft 365, так как они предоставляют более широкий выбор ресурсов. | `[]` | `true` | `false` | Нет |


## <a name="microsoft-365-groups"></a>Группы Microsoft 365
Группы Microsoft 365 лучше всего проявляют себя при совместной работе над проектом или в команде. Они создаются с ресурсами, доступными всем участникам, включая:

- беседы Outlook;
- календарь Outlook;
- файлы SharePoint;
- записную книжку OneNote;
- сайт группы SharePoint;
- планы для планировщика;
- средства управления устройствами Intune.

### <a name="group-in-outlook-example"></a>Пример группы в Outlook

Ниже показано представление групп Outlook в формате JSON.

```http

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
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

Группы безопасности предназначены для управления доступом пользователей к ресурсам. Проверяя, является ли пользователь членом группы безопасности, приложение может принимать решения касательно авторизации, когда пользователь пытается получить доступ к защищенным ресурсам в приложении. Членами групп безопасности могут быть как пользователи, так и другие группы безопасности.

Группы безопасности, поддерживающие почту, используются так же, как и обычные группы безопасности, но включают общий почтовый ящик. Группы безопасности, поддерживающие почту, доступны только для чтения. Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange](/Exchange/recipients/mail-enabled-security-groups).

### <a name="security-group-example"></a>Пример группы безопасности

Ниже показано представление группы безопасности в формате JSON.

```http
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

Для любых групп можно задавать правила динамического членства, которые автоматически добавляют или удаляют членов группы в соответствии со свойствами пользователей. Например, группа "Marketing employees" (Сотрудники маркетингового отдела) должна включать всех пользователей, для которых в свойстве отдела задано значение "Marketing" (Маркетинг). Новые сотрудники этого отдела должны автоматически добавляться в группу, а сотрудники, покидающие отдел, — автоматически удаляться из нее. Это правило можно указать в поле membershipRule во время создания группы, используя следующий формат: `"membershipRule": 'user.department -eq "Marketing"'`. Значение GroupTypes также должно включать строку `"DynamicMembership"`. Приведенный ниже запрос создает группу Microsoft 365 для сотрудников маркетингового отдела.

```http
POST https://graph.microsoft.com/beta/groups
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
    "membershipRule": "user.department -eq \"Marketing\"",
    "membershipRuleProcessingState": "on"
}
```

Дополнительные сведения о составлении правил членства см. в статье [Создание правил на основе атрибутов для динамического членства в группах в Azure Active Directory](/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).

> **Примечание.** Чтобы правила динамического членства работали, у клиента должна быть лицензия на уровне [Azure Active Directory Premium P1](https://azure.microsoft.com/pricing/details/active-directory/) или выше.

## <a name="other-types-of-groups"></a>Группы других типов

Группы Microsoft 365 в Yammer используются для организации совместной работы пользователей с помощью записей Yammer. Группы такого типа можно возвращать с помощью запроса на чтение, но записи из них недоступны через API. Если в группе включены записи и каналы бесед Yammer, то стандартные групповые беседы Microsoft 365 отключены. Дополнительные сведения см. в [документах, посвященных API Yammer для разработчиков](https://developer.yammer.com/docs).

## <a name="group-based-licensing"></a>Лицензирование на основе групп

С помощью лицензирования на основе групп вы можете назначить одну или несколько лицензий на продукты группе Azure AD. Azure AD обеспечит назначение лицензий всем участникам этой группы. Всем новым участникам, присоединившимся к группе, назначаются соответствующие лицензии. При выходе участников из группы эти лицензии удаляются. Эта возможность доступна только для групп безопасности и групп Microsoft 365 с параметром `securityEnabled=TRUE`. Дополнительные сведения о лицензировании на основе групп см. в статье [Что такое лицензии групп в Azure Active Directory?](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).

## <a name="common-use-cases"></a>Основные варианты использования

Ниже перечислены некоторые распространенные операции, которые можно выполнять с помощью Microsoft Graph.

| **Варианты использования**  | **Ресурсы REST** | **См. также** |
|:---------------|:--------|:----------|
| **Объект и методы группы** | | |
| Создание новых групп и получение существующих, обновление свойств и удаление групп. В настоящее время с помощью API можно создавать только группы безопасности и группы Outlook. | [group](group.md) | [Создание групп](../api/group-post-groups.md) <br/> [Перечисление групп](../api/group-list.md) <br/> [Обновление групп](../api/group-update.md) <br/> [Удаление групп](../api/group-delete.md) |
| **Методы для членства в группах** | | |
| Перечисление, добавление и удаление членов групп. | [user](user.md) <br/> [group](group.md)| [Перечисление членов](../api/group-list-members.md) <br/> [Добавление члена](../api/group-post-members.md) <br/> [Удаление члена](../api/group-delete-members.md)|
| Проверка членства пользователя в группе, получение всех групп, в которых состоит пользователь. | [user](user.md) <br/> [group](group.md) <br/> [servicePrincipal](serviceprincipal.md) <br/> [orgContact](orgcontact.md)| [Проверка членства в группах](../api/directoryobject-checkmembergroups.md) <br/> [Получение групп пользователя](../api/directoryobject-getmembergroups.md)|
| Перечисление, добавление и удаление владельцев группы. | [user](user.md) <br/> [group](group.md)| [Перечисление владельцев](../api/group-list-members.md) <br/> [Добавление члена](../api/group-post-members.md) <br/> [Удаление участника](../api/group-delete-members.md)|

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.
