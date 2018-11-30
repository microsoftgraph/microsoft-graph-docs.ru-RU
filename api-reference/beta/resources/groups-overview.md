---
title: Работа с группами в Microsoft Graph
description: Группы — это коллекции пользователей и других субъектов, у которых есть совместный доступ к ресурсам в службах Майкрософт или в вашем приложении. Microsoft Graph предоставляет интерфейсы API, с помощью которых можно создавать разнообразные группы и их функции, а также управлять ими в соответствии с конкретным случаем. Для всех операций с группами в Microsoft Graph необходимо согласие администратора.
ms.openlocfilehash: f60d3faf8fd26c5ec4d1e962d11a4c29f4c1bf73
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079104"
---
# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="e71e6-105">Работа с группами в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e71e6-105">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="e71e6-106">Группы — это коллекции [пользователей](user.md) и других субъектов, у которых есть совместный доступ к ресурсам в службах Майкрософт или в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="e71e6-106">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="e71e6-107">Microsoft Graph предоставляет интерфейсы API, с помощью которых можно создавать разнообразные группы и их функции, а также управлять ими в соответствии с конкретным случаем.</span><span class="sxs-lookup"><span data-stu-id="e71e6-107">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="e71e6-108">Для всех операций с группами в Microsoft Graph необходимо согласие администратора.</span><span class="sxs-lookup"><span data-stu-id="e71e6-108">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="e71e6-109">**Примечание.** Создавать группы можно только с помощью рабочих или учебных учетных записей.</span><span class="sxs-lookup"><span data-stu-id="e71e6-109">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="e71e6-110">Личные учетные записи Майкрософт не поддерживают группы.</span><span class="sxs-lookup"><span data-stu-id="e71e6-110">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="e71e6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e71e6-111">Type</span></span>              | <span data-ttu-id="e71e6-112">Вариант использования</span><span class="sxs-lookup"><span data-stu-id="e71e6-112">Use case</span></span> | <span data-ttu-id="e71e6-113">groupType</span><span class="sxs-lookup"><span data-stu-id="e71e6-113">groupType</span></span> | <span data-ttu-id="e71e6-114">Поддержка почты</span><span class="sxs-lookup"><span data-stu-id="e71e6-114">mail-enabled</span></span> | <span data-ttu-id="e71e6-115">Поддержка защиты</span><span class="sxs-lookup"><span data-stu-id="e71e6-115">security-enabled</span></span> | <span data-ttu-id="e71e6-116">Возможность создания с помощью API</span><span class="sxs-lookup"><span data-stu-id="e71e6-116">Can be created via API?</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="e71e6-117">Группы Office 365</span><span class="sxs-lookup"><span data-stu-id="e71e6-117">Office 365 groups</span></span>](#office-365-groups) | <span data-ttu-id="e71e6-118">Обеспечение совместной работы пользователей с общими ресурсами Майкрософт в Интернете.</span><span class="sxs-lookup"><span data-stu-id="e71e6-118">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | `false` | <span data-ttu-id="e71e6-119">Да</span><span class="sxs-lookup"><span data-stu-id="e71e6-119">Yes</span></span> |
| [<span data-ttu-id="e71e6-120">Группы безопасности</span><span class="sxs-lookup"><span data-stu-id="e71e6-120">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="e71e6-121">Управление доступом пользователей к ресурсам в приложении.</span><span class="sxs-lookup"><span data-stu-id="e71e6-121">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="e71e6-122">Да</span><span class="sxs-lookup"><span data-stu-id="e71e6-122">Yes</span></span> |
| [<span data-ttu-id="e71e6-123">Группы безопасности, поддерживающие почту</span><span class="sxs-lookup"><span data-stu-id="e71e6-123">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="e71e6-124">Управление доступом пользователей к ресурсам в приложении с общим почтовым ящиком группы.</span><span class="sxs-lookup"><span data-stu-id="e71e6-124">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="e71e6-125">Нет</span><span class="sxs-lookup"><span data-stu-id="e71e6-125">No</span></span> |
| <span data-ttu-id="e71e6-126">Группы рассылки</span><span class="sxs-lookup"><span data-stu-id="e71e6-126">Distribution groups</span></span> | <span data-ttu-id="e71e6-127">Рассылка почты участникам группы.</span><span class="sxs-lookup"><span data-stu-id="e71e6-127">Distributing mail to the members of the group.</span></span> <span data-ttu-id="e71e6-128">Рекомендуем использовать группы Office 365, так как они предоставляют более широкий выбор ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e71e6-128">It is recommended to use Office 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="e71e6-129">Нет</span><span class="sxs-lookup"><span data-stu-id="e71e6-129">No</span></span> |

## <a name="office-365-groups"></a><span data-ttu-id="e71e6-130">Группы Office 365</span><span class="sxs-lookup"><span data-stu-id="e71e6-130">Office 365 groups</span></span>
<span data-ttu-id="e71e6-131">Группы Office 365 лучше всего проявляют себя при совместной работе над проектом или в команде.</span><span class="sxs-lookup"><span data-stu-id="e71e6-131">The power of Office 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="e71e6-132">Они создаются с ресурсами, доступными всем участникам, включая:</span><span class="sxs-lookup"><span data-stu-id="e71e6-132">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="e71e6-133">беседы Outlook;</span><span class="sxs-lookup"><span data-stu-id="e71e6-133">Outlook conversations</span></span>
- <span data-ttu-id="e71e6-134">календарь Outlook;</span><span class="sxs-lookup"><span data-stu-id="e71e6-134">Outlook calendar</span></span>
- <span data-ttu-id="e71e6-135">файлы SharePoint;</span><span class="sxs-lookup"><span data-stu-id="e71e6-135">SharePoint files</span></span>
- <span data-ttu-id="e71e6-136">записную книжку OneNote;</span><span class="sxs-lookup"><span data-stu-id="e71e6-136">OneNote notebook</span></span>
- <span data-ttu-id="e71e6-137">сайт группы SharePoint;</span><span class="sxs-lookup"><span data-stu-id="e71e6-137">SharePoint team site</span></span>
- <span data-ttu-id="e71e6-138">планы для планировщика;</span><span class="sxs-lookup"><span data-stu-id="e71e6-138">Planner plans</span></span>
- <span data-ttu-id="e71e6-139">средства управления устройствами Intune.</span><span class="sxs-lookup"><span data-stu-id="e71e6-139">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="e71e6-140">Пример группы в Outlook</span><span class="sxs-lookup"><span data-stu-id="e71e6-140">Group in Outlook example</span></span>

<span data-ttu-id="e71e6-141">Ниже показано представление групп Outlook в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e71e6-141">The following is a JSON representation of groups in Outlook.</span></span> 

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
<span data-ttu-id="e71e6-142">Дополнительные сведения о группах Office 365 и интерфейсах для администраторов см. в статье [Дополнительные сведения о группах Office 365](https://support.office.com/en-us/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span><span class="sxs-lookup"><span data-stu-id="e71e6-142">To learn more about Office 365 groups and the administrator experiences, see [Learn about Office 365 Groups](https://support.office.com/en-us/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="e71e6-143">Группы безопасности (обычные и поддерживающие почту)</span><span class="sxs-lookup"><span data-stu-id="e71e6-143">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="e71e6-144">Группы безопасности предназначены для управления доступом пользователей к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="e71e6-144">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="e71e6-145">Проверяя, является ли пользователь членом группы безопасности, приложение может принимать решения касательно авторизации, когда пользователь пытается получить доступ к защищенным ресурсам в приложении.</span><span class="sxs-lookup"><span data-stu-id="e71e6-145">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="e71e6-146">Членами групп безопасности могут быть как пользователи, так и другие группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="e71e6-146">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="e71e6-147">Группы безопасности, поддерживающие почту, используются так же, как и обычные группы безопасности, но включают общий почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="e71e6-147">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="e71e6-148">Группы безопасности, поддерживающие почту, нельзя создавать через API, но с ними можно выполнять все остальные операции для групп.</span><span class="sxs-lookup"><span data-stu-id="e71e6-148">Mail-enabled security groups can't be created through the API, but other group operations work.</span></span> <span data-ttu-id="e71e6-149">Группы безопасности, поддерживающие почту, доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e71e6-149">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="e71e6-150">Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange](https://technet.microsoft.com/en-us/library/bb123521%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="e71e6-150">Learn more in the [Manage mail-enabled security groups Exchange article](https://technet.microsoft.com/en-us/library/bb123521%28v=exchg.160%29.aspx).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="e71e6-151">Пример группы безопасности</span><span class="sxs-lookup"><span data-stu-id="e71e6-151">Security group example</span></span>

<span data-ttu-id="e71e6-152">Ниже показано представление группы безопасности в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e71e6-152">The following is a JSON representation of a security group.</span></span> 

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
## <a name="dynamic-membership"></a><span data-ttu-id="e71e6-153">Динамическое членство</span><span class="sxs-lookup"><span data-stu-id="e71e6-153">Dynamic membership</span></span> 

<span data-ttu-id="e71e6-154">Для любых групп можно задавать правила динамического членства, которые автоматически добавляют или удаляют членов группы в соответствии со свойствами пользователей.</span><span class="sxs-lookup"><span data-stu-id="e71e6-154">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="e71e6-155">Например, группа "Marketing employees" (Сотрудники маркетингового отдела) должна включать всех пользователей, для которых в свойстве отдела задано значение "Marketing" (Маркетинг). Новые сотрудники этого отдела должны автоматически добавляться в группу, а сотрудники, покидающие отдел, — автоматически удаляться из нее.</span><span class="sxs-lookup"><span data-stu-id="e71e6-155">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="e71e6-156">Это правило можно указать в поле membershipRule во время создания группы, используя следующий формат: `"membershipRule": 'user.department -eq "Marketing"'`.</span><span class="sxs-lookup"><span data-stu-id="e71e6-156">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="e71e6-157">Значение GroupType также должно включать строку `"DynamicMembership"`.</span><span class="sxs-lookup"><span data-stu-id="e71e6-157">GroupType must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="e71e6-158">Приведенный ниже запрос создает группу Office 365 для сотрудников маркетингового отдела.</span><span class="sxs-lookup"><span data-stu-id="e71e6-158">The following request creates a new Office 365 group for the marketing employees:</span></span> 

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

<span data-ttu-id="e71e6-159">Дополнительные сведения о составлении правил членства см. в статье [Создание правил на основе атрибутов для динамического членства в группах в Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="e71e6-159">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="e71e6-160">**Примечание.** Чтобы правила динамического членства работали, у клиента должна быть лицензия на уровне [Azure Active Directory Premium P1](https://azure.microsoft.com/en-us/pricing/details/active-directory/) или выше.</span><span class="sxs-lookup"><span data-stu-id="e71e6-160">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/en-us/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="e71e6-161">Группы других типов</span><span class="sxs-lookup"><span data-stu-id="e71e6-161">Other types of groups</span></span>

<span data-ttu-id="e71e6-162">Группы Office 365 в Yammer используются для организации совместной работы пользователей с помощью записей Yammer.</span><span class="sxs-lookup"><span data-stu-id="e71e6-162">Office 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="e71e6-163">Группы такого типа можно возвращать с помощью запроса на чтение, но записи из них недоступны через API.</span><span class="sxs-lookup"><span data-stu-id="e71e6-163">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="e71e6-164">Если в группе включены записи и каналы бесед Yammer, то стандартные групповые беседы Office 365 отключены.</span><span class="sxs-lookup"><span data-stu-id="e71e6-164">When Yammer posts and conversation feeds are enabled on a group, default Office 365 group conversations are disabled.</span></span> <span data-ttu-id="e71e6-165">Дополнительные сведения см. в [документах, посвященных API Yammer для разработчиков](https://developer.yammer.com/docs).</span><span class="sxs-lookup"><span data-stu-id="e71e6-165">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="group-based-licensing"></a><span data-ttu-id="e71e6-166">Группа лицензирования</span><span class="sxs-lookup"><span data-stu-id="e71e6-166">Group-based licensing</span></span> 

<span data-ttu-id="e71e6-167">Групповые лицензирования возможность можно использовать для назначения лицензий продукта к группе Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e71e6-167">Group-based licensing capability can be used to assign one or more product licenses to an Azure AD group.</span></span> <span data-ttu-id="e71e6-168">Azure AD гарантирует, что лицензии назначаются всем членам группы.</span><span class="sxs-lookup"><span data-stu-id="e71e6-168">Azure AD ensures that the licenses are assigned to all members of the group.</span></span> <span data-ttu-id="e71e6-169">Новые члены, которые присоединиться к группе назначены соответствующие лицензии.</span><span class="sxs-lookup"><span data-stu-id="e71e6-169">Any new members who join the group are assigned the appropriate licenses.</span></span> <span data-ttu-id="e71e6-170">При их выхода из группы, которые удаляются.</span><span class="sxs-lookup"><span data-stu-id="e71e6-170">When they leave the group, those licenses are removed.</span></span> <span data-ttu-id="e71e6-171">Компонент может использоваться только с группами безопасности и Office 365 группы, имеющие securityEnabled = TRUE.</span><span class="sxs-lookup"><span data-stu-id="e71e6-171">The feature can only be used with security groups, and Office 365 groups that have securityEnabled=TRUE.</span></span> <span data-ttu-id="e71e6-172">Для получения дополнительных сведений о лицензировании см. групповые [здесь](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="e71e6-172">To learn more about group-based licensing see [here](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="e71e6-173">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="e71e6-173">Common use cases</span></span>

<span data-ttu-id="e71e6-174">Ниже перечислены некоторые распространенные операции, которые можно выполнять с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e71e6-174">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="e71e6-175">**Варианты использования**</span><span class="sxs-lookup"><span data-stu-id="e71e6-175">**Use cases**</span></span>  | <span data-ttu-id="e71e6-176">**Ресурсы REST**</span><span class="sxs-lookup"><span data-stu-id="e71e6-176">**REST resources**</span></span> | <span data-ttu-id="e71e6-177">**См. также**</span><span class="sxs-lookup"><span data-stu-id="e71e6-177">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="e71e6-178">**Объект и методы группы**</span><span class="sxs-lookup"><span data-stu-id="e71e6-178">**Group object and methods**</span></span> | | |
| <span data-ttu-id="e71e6-179">Создание новых групп и получение существующих, обновление свойств и удаление групп.</span><span class="sxs-lookup"><span data-stu-id="e71e6-179">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="e71e6-180">В настоящее время с помощью API можно создавать только группы безопасности и группы Outlook.</span><span class="sxs-lookup"><span data-stu-id="e71e6-180">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="e71e6-181">group</span><span class="sxs-lookup"><span data-stu-id="e71e6-181">group</span></span>](group.md) | [<span data-ttu-id="e71e6-182">Создание групп</span><span class="sxs-lookup"><span data-stu-id="e71e6-182">Create new groups</span></span>](../api/group-post-groups.md) <br/> [<span data-ttu-id="e71e6-183">Перечисление групп</span><span class="sxs-lookup"><span data-stu-id="e71e6-183">List groups</span></span>](../api/group-list.md) <br/> [<span data-ttu-id="e71e6-184">Обновление групп</span><span class="sxs-lookup"><span data-stu-id="e71e6-184">Update groups</span></span>](../api/group-update.md) <br/> [<span data-ttu-id="e71e6-185">Удаление групп</span><span class="sxs-lookup"><span data-stu-id="e71e6-185">Delete groups</span></span>](../api/group-delete.md) |
| <span data-ttu-id="e71e6-186">**Методы для членства в группах**</span><span class="sxs-lookup"><span data-stu-id="e71e6-186">**Group membership methods**</span></span> | | |
| <span data-ttu-id="e71e6-187">Перечисление, добавление и удаление членов групп.</span><span class="sxs-lookup"><span data-stu-id="e71e6-187">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="e71e6-188">user</span><span class="sxs-lookup"><span data-stu-id="e71e6-188">user</span></span>](user.md) <br/> [<span data-ttu-id="e71e6-189">group</span><span class="sxs-lookup"><span data-stu-id="e71e6-189">group</span></span>](group.md)| [<span data-ttu-id="e71e6-190">Перечисление членов</span><span class="sxs-lookup"><span data-stu-id="e71e6-190">List members</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="e71e6-191">Добавление члена</span><span class="sxs-lookup"><span data-stu-id="e71e6-191">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="e71e6-192">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="e71e6-192">Remove member</span></span>](../api/group-delete-members.md)|
| <span data-ttu-id="e71e6-193">Проверка членства пользователя в группе, получение всех групп, в которых состоит пользователь.</span><span class="sxs-lookup"><span data-stu-id="e71e6-193">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="e71e6-194">user</span><span class="sxs-lookup"><span data-stu-id="e71e6-194">user</span></span>](user.md) <br/> [<span data-ttu-id="e71e6-195">group</span><span class="sxs-lookup"><span data-stu-id="e71e6-195">group</span></span>](group.md)| [<span data-ttu-id="e71e6-196">Проверка членства в группах</span><span class="sxs-lookup"><span data-stu-id="e71e6-196">Check member groups</span></span>](../api/group-checkmembergroups.md) <br/> [<span data-ttu-id="e71e6-197">Получение групп пользователя</span><span class="sxs-lookup"><span data-stu-id="e71e6-197">Get member groups</span></span>](../api/group-getmembergroups.md)|
| <span data-ttu-id="e71e6-198">Перечисление, добавление и удаление владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="e71e6-198">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="e71e6-199">user</span><span class="sxs-lookup"><span data-stu-id="e71e6-199">user</span></span>](user.md) <br/> [<span data-ttu-id="e71e6-200">group</span><span class="sxs-lookup"><span data-stu-id="e71e6-200">group</span></span>](group.md)| [<span data-ttu-id="e71e6-201">Перечисление владельцев</span><span class="sxs-lookup"><span data-stu-id="e71e6-201">List owners</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="e71e6-202">Добавление члена</span><span class="sxs-lookup"><span data-stu-id="e71e6-202">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="e71e6-203">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="e71e6-203">Remove member</span></span>](../api/group-delete-members.md)|
