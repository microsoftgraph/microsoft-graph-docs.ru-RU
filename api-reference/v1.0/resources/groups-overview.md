# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="d128c-101">Работа с группами в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d128c-101">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="d128c-102">Группы — это коллекции [пользователей](user.md) и других субъектов, у которых есть совместный доступ к ресурсам в службах Майкрософт или в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="d128c-102">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="d128c-103">Microsoft Graph предоставляет интерфейсы API, с помощью которых можно создавать разнообразные группы и их функции, а также управлять ими в соответствии с конкретным случаем.</span><span class="sxs-lookup"><span data-stu-id="d128c-103">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="d128c-104">Для всех операций с группами в Microsoft Graph необходимо согласие администратора.</span><span class="sxs-lookup"><span data-stu-id="d128c-104">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="d128c-105">**Примечание.** Создавать группы можно только с помощью рабочих или учебных учетных записей.</span><span class="sxs-lookup"><span data-stu-id="d128c-105">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="d128c-106">Личные учетные записи Майкрософт не поддерживают группы.</span><span class="sxs-lookup"><span data-stu-id="d128c-106">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="d128c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d128c-107">Type</span></span>              | <span data-ttu-id="d128c-108">Вариант использования</span><span class="sxs-lookup"><span data-stu-id="d128c-108">Use case</span></span> | <span data-ttu-id="d128c-109">groupType</span><span class="sxs-lookup"><span data-stu-id="d128c-109">groupType</span></span> | <span data-ttu-id="d128c-110">Поддержка почты</span><span class="sxs-lookup"><span data-stu-id="d128c-110">mail-enabled</span></span> | <span data-ttu-id="d128c-111">Поддержка защиты</span><span class="sxs-lookup"><span data-stu-id="d128c-111">security-enabled</span></span> | <span data-ttu-id="d128c-112">Возможность создания с помощью API</span><span class="sxs-lookup"><span data-stu-id="d128c-112">Can be created via API?</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="d128c-113">Группы Office 365</span><span class="sxs-lookup"><span data-stu-id="d128c-113">Office 365 groups</span></span>](#office-365-groups) | <span data-ttu-id="d128c-114">Обеспечение совместной работы пользователей с общими ресурсами Майкрософт в Интернете.</span><span class="sxs-lookup"><span data-stu-id="d128c-114">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | `false` | <span data-ttu-id="d128c-115">Да</span><span class="sxs-lookup"><span data-stu-id="d128c-115">Yes</span></span> |
| [<span data-ttu-id="d128c-116">Группы безопасности</span><span class="sxs-lookup"><span data-stu-id="d128c-116">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="d128c-117">Управление доступом пользователей к ресурсам в приложении.</span><span class="sxs-lookup"><span data-stu-id="d128c-117">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="d128c-118">Да</span><span class="sxs-lookup"><span data-stu-id="d128c-118">Yes</span></span> |
| [<span data-ttu-id="d128c-119">Группы безопасности, поддерживающие почту</span><span class="sxs-lookup"><span data-stu-id="d128c-119">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="d128c-120">Управление доступом пользователей к ресурсам в приложении с общим почтовым ящиком группы.</span><span class="sxs-lookup"><span data-stu-id="d128c-120">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="d128c-121">Нет</span><span class="sxs-lookup"><span data-stu-id="d128c-121">No</span></span> |
| <span data-ttu-id="d128c-122">Группы рассылки</span><span class="sxs-lookup"><span data-stu-id="d128c-122">Distribution groups</span></span> | <span data-ttu-id="d128c-123">Рассылка почты участникам группы.</span><span class="sxs-lookup"><span data-stu-id="d128c-123">Distributing mail to the members of the group.</span></span> <span data-ttu-id="d128c-124">Рекомендуем использовать группы Office 365, так как они предоставляют более широкий выбор ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d128c-124">It is recommended to use Office 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="d128c-125">Нет</span><span class="sxs-lookup"><span data-stu-id="d128c-125">No</span></span> |

## <a name="office-365-groups"></a><span data-ttu-id="d128c-126">Группы Office 365</span><span class="sxs-lookup"><span data-stu-id="d128c-126">Office 365 groups</span></span>
<span data-ttu-id="d128c-127">Группы Office 365 лучше всего проявляют себя при совместной работе над проектом или в команде.</span><span class="sxs-lookup"><span data-stu-id="d128c-127">The power of Office 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="d128c-128">Они создаются с ресурсами, доступными всем участникам, включая:</span><span class="sxs-lookup"><span data-stu-id="d128c-128">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="d128c-129">беседы Outlook;</span><span class="sxs-lookup"><span data-stu-id="d128c-129">Outlook conversations</span></span>
- <span data-ttu-id="d128c-130">календарь Outlook;</span><span class="sxs-lookup"><span data-stu-id="d128c-130">Outlook calendar</span></span>
- <span data-ttu-id="d128c-131">файлы SharePoint;</span><span class="sxs-lookup"><span data-stu-id="d128c-131">SharePoint files</span></span>
- <span data-ttu-id="d128c-132">записную книжку OneNote;</span><span class="sxs-lookup"><span data-stu-id="d128c-132">OneNote notebook</span></span>
- <span data-ttu-id="d128c-133">сайт группы SharePoint;</span><span class="sxs-lookup"><span data-stu-id="d128c-133">SharePoint team site</span></span>
- <span data-ttu-id="d128c-134">планы для планировщика;</span><span class="sxs-lookup"><span data-stu-id="d128c-134">Planner plans</span></span>
- <span data-ttu-id="d128c-135">средства управления устройствами Intune.</span><span class="sxs-lookup"><span data-stu-id="d128c-135">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="d128c-136">Пример группы в Outlook</span><span class="sxs-lookup"><span data-stu-id="d128c-136">Group in Outlook example</span></span>

<span data-ttu-id="d128c-137">Ниже показано представление групп Outlook в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d128c-137">The following is a JSON representation of groups in Outlook.</span></span> 

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
<span data-ttu-id="d128c-138">Дополнительные сведения о группах Office 365 и интерфейсах для администраторов см. в статье [Дополнительные сведения о группах Office 365](https://support.office.com/ru-RU/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span><span class="sxs-lookup"><span data-stu-id="d128c-138">To learn more about Office 365 groups and the administrator experiences, see [Learn about Office 365 Groups](https://support.office.com/ru-RU/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="d128c-139">Группы безопасности (обычные и поддерживающие почту)</span><span class="sxs-lookup"><span data-stu-id="d128c-139">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="d128c-140">Группы безопасности предназначены для управления доступом пользователей к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="d128c-140">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="d128c-141">Проверяя, является ли пользователь членом группы безопасности, приложение может принимать решения касательно авторизации, когда пользователь пытается получить доступ к защищенным ресурсам в приложении.</span><span class="sxs-lookup"><span data-stu-id="d128c-141">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="d128c-142">Членами групп безопасности могут быть как пользователи, так и другие группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="d128c-142">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="d128c-143">Группы безопасности, поддерживающие почту, используются так же, как и обычные группы безопасности, но включают общий почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="d128c-143">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="d128c-144">Группы безопасности, поддерживающие почту, нельзя создавать через API, но с ними можно выполнять все остальные операции для групп.</span><span class="sxs-lookup"><span data-stu-id="d128c-144">Mail-enabled security groups can't be created through the API, but other group operations will still work here.</span></span>  <span data-ttu-id="d128c-145">Группы безопасности, поддерживающие почту, доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d128c-145">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="d128c-146">Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange](https://technet.microsoft.com/ru-RU/library/bb123521%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="d128c-146">Learn more in the [Manage mail-enabled security groups Exchange article](https://technet.microsoft.com/ru-RU/library/bb123521%28v=exchg.160%29.aspx).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="d128c-147">Пример группы безопасности</span><span class="sxs-lookup"><span data-stu-id="d128c-147">Security group example</span></span>

<span data-ttu-id="d128c-148">Ниже показано представление группы безопасности в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d128c-148">The following is a JSON representation of a security group.</span></span> 

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
## <a name="dynamic-membership"></a><span data-ttu-id="d128c-149">Динамическое членство</span><span class="sxs-lookup"><span data-stu-id="d128c-149">Dynamic membership</span></span> 

<span data-ttu-id="d128c-150">Для любых групп можно задавать правила динамического членства, которые автоматически добавляют или удаляют членов группы в соответствии со свойствами пользователей.</span><span class="sxs-lookup"><span data-stu-id="d128c-150">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="d128c-151">Например, группа "Marketing employees" (Сотрудники маркетингового отдела) должна включать всех пользователей, для которых в свойстве отдела задано значение "Marketing" (Маркетинг). Новые сотрудники этого отдела должны автоматически добавляться в группу, а сотрудники, покидающие отдел, — автоматически удаляться из нее.</span><span class="sxs-lookup"><span data-stu-id="d128c-151">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="d128c-152">Это правило можно указать в поле membershipRule во время создания группы, используя следующий формат: `"membershipRule": 'user.department -eq "Marketing"'`.</span><span class="sxs-lookup"><span data-stu-id="d128c-152">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="d128c-153">Значение GroupType также должно включать строку `"DynamicMembership"`.</span><span class="sxs-lookup"><span data-stu-id="d128c-153">GroupType must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="d128c-154">Приведенный ниже запрос создает группу Office 365 для сотрудников маркетингового отдела.</span><span class="sxs-lookup"><span data-stu-id="d128c-154">The following request creates a new Office 365 group for the marketing employees:</span></span> 

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

<span data-ttu-id="d128c-155">Дополнительные сведения о составлении правил членства см. в статье [Создание правил на основе атрибутов для динамического членства в группах в Azure Active Directory](https://docs.microsoft.com/ru-RU/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="d128c-155">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](https://docs.microsoft.com/ru-RU/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="d128c-156">**Примечание.** Чтобы правила динамического членства работали, у клиента должна быть лицензия на уровне [Azure Active Directory Premium P1](https://azure.microsoft.com/ru-RU/pricing/details/active-directory/) или выше.</span><span class="sxs-lookup"><span data-stu-id="d128c-156">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/ru-RU/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="d128c-157">Группы других типов</span><span class="sxs-lookup"><span data-stu-id="d128c-157">Other types of groups</span></span>

<span data-ttu-id="d128c-158">Группы Office 365 в Yammer используются для организации совместной работы пользователей с помощью записей Yammer.</span><span class="sxs-lookup"><span data-stu-id="d128c-158">Office 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="d128c-159">Группы такого типа можно возвращать с помощью запроса на чтение, но записи из них недоступны через API.</span><span class="sxs-lookup"><span data-stu-id="d128c-159">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="d128c-160">Если в группе включены записи и каналы бесед Yammer, то стандартные групповые беседы Office 365 отключены.</span><span class="sxs-lookup"><span data-stu-id="d128c-160">When Yammer posts and conversation feeds are enabled on a group, default Office 365 group conversations are disabled.</span></span> <span data-ttu-id="d128c-161">Дополнительные сведения см. в [документах, посвященных API Yammer для разработчиков](https://developer.yammer.com/docs).</span><span class="sxs-lookup"><span data-stu-id="d128c-161">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="d128c-162">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="d128c-162">Common use cases</span></span>

<span data-ttu-id="d128c-163">Ниже перечислены некоторые распространенные операции, которые можно выполнять с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d128c-163">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="d128c-164">**Варианты использования**</span><span class="sxs-lookup"><span data-stu-id="d128c-164">**Use cases**</span></span>  | <span data-ttu-id="d128c-165">**Ресурсы REST**</span><span class="sxs-lookup"><span data-stu-id="d128c-165">**REST resources**</span></span> | <span data-ttu-id="d128c-166">**См. также**</span><span class="sxs-lookup"><span data-stu-id="d128c-166">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="d128c-167">**Объект и методы группы**</span><span class="sxs-lookup"><span data-stu-id="d128c-167">**Group object and methods**</span></span> | | |
| <span data-ttu-id="d128c-168">Создание новых групп и получение существующих, обновление свойств и удаление групп.</span><span class="sxs-lookup"><span data-stu-id="d128c-168">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="d128c-169">В настоящее время с помощью API можно создавать только группы безопасности и группы Outlook.</span><span class="sxs-lookup"><span data-stu-id="d128c-169">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="d128c-170">group</span><span class="sxs-lookup"><span data-stu-id="d128c-170">group</span></span>](group.md) | [<span data-ttu-id="d128c-171">Создание групп</span><span class="sxs-lookup"><span data-stu-id="d128c-171">Create new groups</span></span>](../api/group_post_groups.md) <br/> [<span data-ttu-id="d128c-172">Перечисление групп</span><span class="sxs-lookup"><span data-stu-id="d128c-172">List groups</span></span>](../api/group_list.md) <br/> [<span data-ttu-id="d128c-173">Обновление групп</span><span class="sxs-lookup"><span data-stu-id="d128c-173">Update groups</span></span>](../api/group_update.md) <br/> [<span data-ttu-id="d128c-174">Удаление групп</span><span class="sxs-lookup"><span data-stu-id="d128c-174">Delete groups</span></span>](../api/group_delete.md) |
| <span data-ttu-id="d128c-175">**Методы для членства в группах**</span><span class="sxs-lookup"><span data-stu-id="d128c-175">**Group membership methods**</span></span> | | |
| <span data-ttu-id="d128c-176">Перечисление, добавление и удаление членов групп.</span><span class="sxs-lookup"><span data-stu-id="d128c-176">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="d128c-177">user</span><span class="sxs-lookup"><span data-stu-id="d128c-177">user</span></span>](user.md) <br/> [<span data-ttu-id="d128c-178">group</span><span class="sxs-lookup"><span data-stu-id="d128c-178">group</span></span>](group.md)| [<span data-ttu-id="d128c-179">Перечисление членов</span><span class="sxs-lookup"><span data-stu-id="d128c-179">List members</span></span>](../api/group_list_members.md) <br/> [<span data-ttu-id="d128c-180">Добавление члена</span><span class="sxs-lookup"><span data-stu-id="d128c-180">Add member</span></span>](../api/group_post_members.md) <br/> [<span data-ttu-id="d128c-181">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="d128c-181">Remove member</span></span>](../api/group_delete_members.md)|
| <span data-ttu-id="d128c-182">Проверка членства пользователя в группе, получение всех групп, в которых состоит пользователь.</span><span class="sxs-lookup"><span data-stu-id="d128c-182">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="d128c-183">user</span><span class="sxs-lookup"><span data-stu-id="d128c-183">user</span></span>](user.md) <br/> [<span data-ttu-id="d128c-184">group</span><span class="sxs-lookup"><span data-stu-id="d128c-184">group</span></span>](group.md)| [<span data-ttu-id="d128c-185">Проверка членства в группах</span><span class="sxs-lookup"><span data-stu-id="d128c-185">Check member groups</span></span>](../api/group_checkmembergroups.md) <br/> [<span data-ttu-id="d128c-186">Получение групп пользователя</span><span class="sxs-lookup"><span data-stu-id="d128c-186">Get member groups</span></span>](../api/group_getmembergroups.md)|
| <span data-ttu-id="d128c-187">Перечисление, добавление и удаление владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="d128c-187">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="d128c-188">user</span><span class="sxs-lookup"><span data-stu-id="d128c-188">user</span></span>](user.md) <br/> [<span data-ttu-id="d128c-189">group</span><span class="sxs-lookup"><span data-stu-id="d128c-189">group</span></span>](group.md)| [<span data-ttu-id="d128c-190">Перечисление владельцев</span><span class="sxs-lookup"><span data-stu-id="d128c-190">List owners</span></span>](../api/group_list_members.md) <br/> [<span data-ttu-id="d128c-191">Добавление члена</span><span class="sxs-lookup"><span data-stu-id="d128c-191">Add member</span></span>](../api/group_post_members.md) <br/> [<span data-ttu-id="d128c-192">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="d128c-192">Remove member</span></span>](../api/group_delete_members.md)|
