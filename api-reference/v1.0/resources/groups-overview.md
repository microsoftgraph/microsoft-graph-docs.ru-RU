---
title: Работа с группами в Microsoft Graph
description: Группы — это коллекции пользователей и других субъектов, у которых есть совместный доступ к ресурсам в службах Майкрософт или в вашем приложении. Microsoft Graph предоставляет интерфейсы API, с помощью которых можно создавать разнообразные группы и их функции, а также управлять ими в соответствии с конкретным случаем. Для всех операций с группами в Microsoft Graph необходимо согласие администратора.
author: dkershaw10
ms.openlocfilehash: f3d18fd2ebf579c878e50bfae66e3987b6ef1a84
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301689"
---
# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="f7fb4-105">Работа с группами в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f7fb4-105">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="f7fb4-106">Группы — это коллекции [пользователей](user.md) и других субъектов, у которых есть совместный доступ к ресурсам в службах Майкрософт или в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-106">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="f7fb4-107">Microsoft Graph предоставляет интерфейсы API, с помощью которых можно создавать разнообразные группы и их функции, а также управлять ими в соответствии с конкретным случаем.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-107">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="f7fb4-108">Для всех операций с группами в Microsoft Graph необходимо согласие администратора.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-108">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="f7fb4-109">**Примечание.** Создавать группы можно только с помощью рабочих или учебных учетных записей.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-109">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="f7fb4-110">Личные учетные записи Майкрософт не поддерживают группы.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-110">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="f7fb4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f7fb4-111">Type</span></span>              | <span data-ttu-id="f7fb4-112">Вариант использования</span><span class="sxs-lookup"><span data-stu-id="f7fb4-112">Use case</span></span> | <span data-ttu-id="f7fb4-113">groupType</span><span class="sxs-lookup"><span data-stu-id="f7fb4-113">groupType</span></span> | <span data-ttu-id="f7fb4-114">Поддержка почты</span><span class="sxs-lookup"><span data-stu-id="f7fb4-114">mail-enabled</span></span> | <span data-ttu-id="f7fb4-115">Поддержка защиты</span><span class="sxs-lookup"><span data-stu-id="f7fb4-115">security-enabled</span></span> | <span data-ttu-id="f7fb4-116">Возможность создания с помощью API</span><span class="sxs-lookup"><span data-stu-id="f7fb4-116">Can be created via API?</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="f7fb4-117">Группы Office 365</span><span class="sxs-lookup"><span data-stu-id="f7fb4-117">Office 365 groups</span></span>](#office-365-groups) | <span data-ttu-id="f7fb4-118">Обеспечение совместной работы пользователей с общими ресурсами Майкрософт в Интернете.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-118">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | `false` | <span data-ttu-id="f7fb4-119">Да</span><span class="sxs-lookup"><span data-stu-id="f7fb4-119">Yes</span></span> |
| [<span data-ttu-id="f7fb4-120">Группы безопасности</span><span class="sxs-lookup"><span data-stu-id="f7fb4-120">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="f7fb4-121">Управление доступом пользователей к ресурсам в приложении.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-121">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="f7fb4-122">Да</span><span class="sxs-lookup"><span data-stu-id="f7fb4-122">Yes</span></span> |
| [<span data-ttu-id="f7fb4-123">Группы безопасности, поддерживающие почту</span><span class="sxs-lookup"><span data-stu-id="f7fb4-123">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="f7fb4-124">Управление доступом пользователей к ресурсам в приложении с общим почтовым ящиком группы.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-124">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="f7fb4-125">Нет</span><span class="sxs-lookup"><span data-stu-id="f7fb4-125">No</span></span> |
| <span data-ttu-id="f7fb4-126">Группы рассылки</span><span class="sxs-lookup"><span data-stu-id="f7fb4-126">Distribution groups</span></span> | <span data-ttu-id="f7fb4-127">Рассылка почты участникам группы.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-127">Distributing mail to the members of the group.</span></span> <span data-ttu-id="f7fb4-128">Рекомендуем использовать группы Office 365, так как они предоставляют более широкий выбор ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-128">It is recommended to use Office 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="f7fb4-129">Нет</span><span class="sxs-lookup"><span data-stu-id="f7fb4-129">No</span></span> |

## <a name="office-365-groups"></a><span data-ttu-id="f7fb4-130">Группы Office 365</span><span class="sxs-lookup"><span data-stu-id="f7fb4-130">Office 365 groups</span></span>
<span data-ttu-id="f7fb4-131">Группы Office 365 лучше всего проявляют себя при совместной работе над проектом или в команде.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-131">The power of Office 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="f7fb4-132">Они создаются с ресурсами, доступными всем участникам, включая:</span><span class="sxs-lookup"><span data-stu-id="f7fb4-132">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="f7fb4-133">беседы Outlook;</span><span class="sxs-lookup"><span data-stu-id="f7fb4-133">Outlook conversations</span></span>
- <span data-ttu-id="f7fb4-134">календарь Outlook;</span><span class="sxs-lookup"><span data-stu-id="f7fb4-134">Outlook calendar</span></span>
- <span data-ttu-id="f7fb4-135">файлы SharePoint;</span><span class="sxs-lookup"><span data-stu-id="f7fb4-135">SharePoint files</span></span>
- <span data-ttu-id="f7fb4-136">записную книжку OneNote;</span><span class="sxs-lookup"><span data-stu-id="f7fb4-136">OneNote notebook</span></span>
- <span data-ttu-id="f7fb4-137">сайт группы SharePoint;</span><span class="sxs-lookup"><span data-stu-id="f7fb4-137">SharePoint team site</span></span>
- <span data-ttu-id="f7fb4-138">планы для планировщика;</span><span class="sxs-lookup"><span data-stu-id="f7fb4-138">Planner plans</span></span>
- <span data-ttu-id="f7fb4-139">средства управления устройствами Intune.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-139">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="f7fb4-140">Пример группы в Outlook</span><span class="sxs-lookup"><span data-stu-id="f7fb4-140">Group in Outlook example</span></span>

<span data-ttu-id="f7fb4-141">Ниже показано представление групп Outlook в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-141">The following is a JSON representation of groups in Outlook.</span></span> 

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
<span data-ttu-id="f7fb4-142">Дополнительные сведения о группах Office 365 и интерфейсах для администраторов см. в статье [Дополнительные сведения о группах Office 365](https://support.office.com/en-us/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span><span class="sxs-lookup"><span data-stu-id="f7fb4-142">To learn more about Office 365 groups and the administrator experiences, see [Learn about Office 365 Groups](https://support.office.com/en-us/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="f7fb4-143">Группы безопасности (обычные и поддерживающие почту)</span><span class="sxs-lookup"><span data-stu-id="f7fb4-143">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="f7fb4-144">Группы безопасности предназначены для управления доступом пользователей к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-144">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="f7fb4-145">Проверяя, является ли пользователь членом группы безопасности, приложение может принимать решения касательно авторизации, когда пользователь пытается получить доступ к защищенным ресурсам в приложении.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-145">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="f7fb4-146">Членами групп безопасности могут быть как пользователи, так и другие группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-146">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="f7fb4-147">Группы безопасности, поддерживающие почту, используются так же, как и обычные группы безопасности, но включают общий почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-147">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="f7fb4-148">Группы безопасности, поддерживающие почту, нельзя создавать через API, но с ними можно выполнять все остальные операции для групп.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-148">Mail-enabled security groups can't be created through the API, but other group operations work.</span></span>  <span data-ttu-id="f7fb4-149">Группы безопасности, поддерживающие почту, доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-149">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="f7fb4-150">Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange](https://technet.microsoft.com/en-us/library/bb123521%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="f7fb4-150">Learn more in the [Manage mail-enabled security groups Exchange article](https://technet.microsoft.com/en-us/library/bb123521%28v=exchg.160%29.aspx).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="f7fb4-151">Пример группы безопасности</span><span class="sxs-lookup"><span data-stu-id="f7fb4-151">Security group example</span></span>

<span data-ttu-id="f7fb4-152">Ниже показано представление группы безопасности в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-152">The following is a JSON representation of a security group.</span></span> 

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
## <a name="dynamic-membership"></a><span data-ttu-id="f7fb4-153">Динамическое членство</span><span class="sxs-lookup"><span data-stu-id="f7fb4-153">Dynamic membership</span></span> 

<span data-ttu-id="f7fb4-154">Для любых групп можно задавать правила динамического членства, которые автоматически добавляют или удаляют членов группы в соответствии со свойствами пользователей.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-154">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="f7fb4-155">Например, группа "Marketing employees" (Сотрудники маркетингового отдела) должна включать всех пользователей, для которых в свойстве отдела задано значение "Marketing" (Маркетинг). Новые сотрудники этого отдела должны автоматически добавляться в группу, а сотрудники, покидающие отдел, — автоматически удаляться из нее.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-155">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="f7fb4-156">Это правило можно указать в поле membershipRule во время создания группы, используя следующий формат: `"membershipRule": 'user.department -eq "Marketing"'`.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-156">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="f7fb4-157">Значение GroupType также должно включать строку `"DynamicMembership"`.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-157">GroupType must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="f7fb4-158">Приведенный ниже запрос создает группу Office 365 для сотрудников маркетингового отдела.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-158">The following request creates a new Office 365 group for the marketing employees:</span></span> 

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
    "membershipRule": 'user.department -eq "Marketing"',
    "membershipRuleProcessingState": "on"
}
```

<span data-ttu-id="f7fb4-159">Дополнительные сведения о составлении правил членства см. в статье [Создание правил на основе атрибутов для динамического членства в группах в Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="f7fb4-159">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="f7fb4-160">**Примечание.** Чтобы правила динамического членства работали, у клиента должна быть лицензия на уровне [Azure Active Directory Premium P1](https://azure.microsoft.com/en-us/pricing/details/active-directory/) или выше.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-160">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/en-us/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="f7fb4-161">Группы других типов</span><span class="sxs-lookup"><span data-stu-id="f7fb4-161">Other types of groups</span></span>

<span data-ttu-id="f7fb4-162">Группы Office 365 в Yammer используются для организации совместной работы пользователей с помощью записей Yammer.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-162">Office 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="f7fb4-163">Группы такого типа можно возвращать с помощью запроса на чтение, но записи из них недоступны через API.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-163">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="f7fb4-164">Если в группе включены записи и каналы бесед Yammer, то стандартные групповые беседы Office 365 отключены.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-164">When Yammer posts and conversation feeds are enabled on a group, default Office 365 group conversations are disabled.</span></span> <span data-ttu-id="f7fb4-165">Дополнительные сведения см. в [документах, посвященных API Yammer для разработчиков](https://developer.yammer.com/docs).</span><span class="sxs-lookup"><span data-stu-id="f7fb4-165">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="f7fb4-166">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="f7fb4-166">Common use cases</span></span>

<span data-ttu-id="f7fb4-167">Ниже перечислены некоторые распространенные операции, которые можно выполнять с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-167">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="f7fb4-168">**Варианты использования**</span><span class="sxs-lookup"><span data-stu-id="f7fb4-168">**Use cases**</span></span>  | <span data-ttu-id="f7fb4-169">**Ресурсы REST**</span><span class="sxs-lookup"><span data-stu-id="f7fb4-169">**REST resources**</span></span> | <span data-ttu-id="f7fb4-170">**См. также**</span><span class="sxs-lookup"><span data-stu-id="f7fb4-170">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="f7fb4-171">**Объект и методы группы**</span><span class="sxs-lookup"><span data-stu-id="f7fb4-171">**Group object and methods**</span></span> | | |
| <span data-ttu-id="f7fb4-172">Создание новых групп и получение существующих, обновление свойств и удаление групп.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-172">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="f7fb4-173">В настоящее время с помощью API можно создавать только группы безопасности и группы Outlook.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-173">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="f7fb4-174">group</span><span class="sxs-lookup"><span data-stu-id="f7fb4-174">group</span></span>](group.md) | [<span data-ttu-id="f7fb4-175">Создание групп</span><span class="sxs-lookup"><span data-stu-id="f7fb4-175">Create new groups</span></span>](../api/group-post-groups.md) <br/> [<span data-ttu-id="f7fb4-176">Перечисление групп</span><span class="sxs-lookup"><span data-stu-id="f7fb4-176">List groups</span></span>](../api/group-list.md) <br/> [<span data-ttu-id="f7fb4-177">Обновление групп</span><span class="sxs-lookup"><span data-stu-id="f7fb4-177">Update groups</span></span>](../api/group-update.md) <br/> [<span data-ttu-id="f7fb4-178">Удаление групп</span><span class="sxs-lookup"><span data-stu-id="f7fb4-178">Delete groups</span></span>](../api/group-delete.md) |
| <span data-ttu-id="f7fb4-179">**Методы для членства в группах**</span><span class="sxs-lookup"><span data-stu-id="f7fb4-179">**Group membership methods**</span></span> | | |
| <span data-ttu-id="f7fb4-180">Перечисление, добавление и удаление членов групп.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-180">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="f7fb4-181">user</span><span class="sxs-lookup"><span data-stu-id="f7fb4-181">user</span></span>](user.md) <br/> [<span data-ttu-id="f7fb4-182">group</span><span class="sxs-lookup"><span data-stu-id="f7fb4-182">group</span></span>](group.md)| [<span data-ttu-id="f7fb4-183">Перечисление членов</span><span class="sxs-lookup"><span data-stu-id="f7fb4-183">List members</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="f7fb4-184">Добавление члена</span><span class="sxs-lookup"><span data-stu-id="f7fb4-184">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="f7fb4-185">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="f7fb4-185">Remove member</span></span>](../api/group-delete-members.md)|
| <span data-ttu-id="f7fb4-186">Проверка членства пользователя в группе, получение всех групп, в которых состоит пользователь.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-186">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="f7fb4-187">user</span><span class="sxs-lookup"><span data-stu-id="f7fb4-187">user</span></span>](user.md) <br/> [<span data-ttu-id="f7fb4-188">group</span><span class="sxs-lookup"><span data-stu-id="f7fb4-188">group</span></span>](group.md)| [<span data-ttu-id="f7fb4-189">Проверка членства в группах</span><span class="sxs-lookup"><span data-stu-id="f7fb4-189">Check member groups</span></span>](../api/group-checkmembergroups.md) <br/> [<span data-ttu-id="f7fb4-190">Получение групп пользователя</span><span class="sxs-lookup"><span data-stu-id="f7fb4-190">Get member groups</span></span>](../api/group-getmembergroups.md)|
| <span data-ttu-id="f7fb4-191">Перечисление, добавление и удаление владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="f7fb4-191">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="f7fb4-192">user</span><span class="sxs-lookup"><span data-stu-id="f7fb4-192">user</span></span>](user.md) <br/> [<span data-ttu-id="f7fb4-193">group</span><span class="sxs-lookup"><span data-stu-id="f7fb4-193">group</span></span>](group.md)| [<span data-ttu-id="f7fb4-194">Перечисление владельцев</span><span class="sxs-lookup"><span data-stu-id="f7fb4-194">List owners</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="f7fb4-195">Добавление члена</span><span class="sxs-lookup"><span data-stu-id="f7fb4-195">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="f7fb4-196">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="f7fb4-196">Remove member</span></span>](../api/group-delete-members.md)|
