---
title: Работа с группами в Microsoft Graph
description: Группы — это коллекции пользователей и других субъектов, у которых есть общий доступ к ресурсам в службах Майкрософт или в вашем приложении. Microsoft Graph предоставляет интерфейсы API, с помощью которых можно создавать разнообразные группы и их функции, а также управлять ими в соответствии с конкретным случаем. Для всех операций с группами в Microsoft Graph необходимо согласие администратора.
author: Jordanndahl
localization_priority: Priority
ms.prod: groups
doc_type: conceptualPageType
ms.openlocfilehash: 5bba894a107c75b1df815579f1d03d97fa964e24
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680090"
---
# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="4a9af-105">Работа с группами в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4a9af-105">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="4a9af-106">Группы — это коллекции [пользователей](user.md) и других субъектов, у которых есть общий доступ к ресурсам в службах Майкрософт или в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="4a9af-106">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="4a9af-107">Microsoft Graph предоставляет интерфейсы API, с помощью которых можно создавать разнообразные группы и их функции, а также управлять ими в соответствии с конкретным случаем.</span><span class="sxs-lookup"><span data-stu-id="4a9af-107">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="4a9af-108">Для всех операций с группами в Microsoft Graph необходимо согласие администратора.</span><span class="sxs-lookup"><span data-stu-id="4a9af-108">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="4a9af-109">**Примечание.** Создавать группы можно только с помощью рабочих или учебных учетных записей.</span><span class="sxs-lookup"><span data-stu-id="4a9af-109">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="4a9af-110">Личные учетные записи Майкрософт не поддерживают группы.</span><span class="sxs-lookup"><span data-stu-id="4a9af-110">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="4a9af-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4a9af-111">Type</span></span>              | <span data-ttu-id="4a9af-112">Вариант использования</span><span class="sxs-lookup"><span data-stu-id="4a9af-112">Use case</span></span> | <span data-ttu-id="4a9af-113">groupTypes</span><span class="sxs-lookup"><span data-stu-id="4a9af-113">groupTypes</span></span> | <span data-ttu-id="4a9af-114">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="4a9af-114">mailEnabled</span></span> | <span data-ttu-id="4a9af-115">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="4a9af-115">securityEnabled</span></span> | <span data-ttu-id="4a9af-116">Создано и управляется с помощью API</span><span class="sxs-lookup"><span data-stu-id="4a9af-116">Created and managed via API</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="4a9af-117">Группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4a9af-117">Microsoft 365 groups</span></span>](#microsoft-365-groups) | <span data-ttu-id="4a9af-118">Обеспечение совместной работы пользователей с общими ресурсами Майкрософт в Интернете.</span><span class="sxs-lookup"><span data-stu-id="4a9af-118">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | <span data-ttu-id="4a9af-119">`true` или `false`</span><span class="sxs-lookup"><span data-stu-id="4a9af-119">`true` or `false`</span></span> | <span data-ttu-id="4a9af-120">Да</span><span class="sxs-lookup"><span data-stu-id="4a9af-120">Yes</span></span> |
| [<span data-ttu-id="4a9af-121">Группы безопасности</span><span class="sxs-lookup"><span data-stu-id="4a9af-121">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="4a9af-122">Управление доступом пользователей к ресурсам в приложении.</span><span class="sxs-lookup"><span data-stu-id="4a9af-122">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="4a9af-123">Да</span><span class="sxs-lookup"><span data-stu-id="4a9af-123">Yes</span></span> |
| [<span data-ttu-id="4a9af-124">Группы безопасности, поддерживающие почту</span><span class="sxs-lookup"><span data-stu-id="4a9af-124">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="4a9af-125">Управление доступом пользователей к ресурсам в приложении с общим почтовым ящиком группы.</span><span class="sxs-lookup"><span data-stu-id="4a9af-125">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="4a9af-126">Нет</span><span class="sxs-lookup"><span data-stu-id="4a9af-126">No</span></span> |
| <span data-ttu-id="4a9af-127">Группы рассылки</span><span class="sxs-lookup"><span data-stu-id="4a9af-127">Distribution groups</span></span> | <span data-ttu-id="4a9af-128">Рассылка почты участникам группы.</span><span class="sxs-lookup"><span data-stu-id="4a9af-128">Distributing mail to the members of the group.</span></span> <span data-ttu-id="4a9af-129">Рекомендуем использовать группы Microsoft 365, так как они предоставляют более широкий выбор ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a9af-129">It is recommended to use Microsoft 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="4a9af-130">Нет</span><span class="sxs-lookup"><span data-stu-id="4a9af-130">No</span></span> |

## <a name="microsoft-365-groups"></a><span data-ttu-id="4a9af-131">Группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4a9af-131">Microsoft 365 groups</span></span>
<span data-ttu-id="4a9af-132">Группы Microsoft 365 лучше всего проявляют себя при совместной работе над проектом или в команде.</span><span class="sxs-lookup"><span data-stu-id="4a9af-132">The power of Microsoft 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="4a9af-133">Они создаются с ресурсами, доступными всем участникам, включая:</span><span class="sxs-lookup"><span data-stu-id="4a9af-133">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="4a9af-134">беседы Outlook;</span><span class="sxs-lookup"><span data-stu-id="4a9af-134">Outlook conversations</span></span>
- <span data-ttu-id="4a9af-135">календарь Outlook;</span><span class="sxs-lookup"><span data-stu-id="4a9af-135">Outlook calendar</span></span>
- <span data-ttu-id="4a9af-136">файлы SharePoint;</span><span class="sxs-lookup"><span data-stu-id="4a9af-136">SharePoint files</span></span>
- <span data-ttu-id="4a9af-137">записную книжку OneNote;</span><span class="sxs-lookup"><span data-stu-id="4a9af-137">OneNote notebook</span></span>
- <span data-ttu-id="4a9af-138">сайт группы SharePoint;</span><span class="sxs-lookup"><span data-stu-id="4a9af-138">SharePoint team site</span></span>
- <span data-ttu-id="4a9af-139">планы для планировщика;</span><span class="sxs-lookup"><span data-stu-id="4a9af-139">Planner plans</span></span>
- <span data-ttu-id="4a9af-140">средства управления устройствами Intune.</span><span class="sxs-lookup"><span data-stu-id="4a9af-140">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="4a9af-141">Пример группы в Outlook</span><span class="sxs-lookup"><span data-stu-id="4a9af-141">Group in Outlook example</span></span>

<span data-ttu-id="4a9af-142">Ниже показано представление групп Outlook в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a9af-142">The following is a JSON representation of groups in Outlook.</span></span>

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
<span data-ttu-id="4a9af-143">Дополнительные сведения о группах Microsoft 365 и интерфейсах для администраторов см. в статье [Дополнительные сведения о группах Microsoft 365](https://support.office.com/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span><span class="sxs-lookup"><span data-stu-id="4a9af-143">To learn more about Microsoft 365 groups and the administrator experiences, see [Learn about Microsoft 365 groups](https://support.office.com/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="4a9af-144">Группы безопасности (обычные и поддерживающие почту)</span><span class="sxs-lookup"><span data-stu-id="4a9af-144">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="4a9af-145">Группы безопасности предназначены для управления доступом пользователей к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="4a9af-145">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="4a9af-146">Проверяя, является ли пользователь членом группы безопасности, приложение может принимать решения касательно авторизации, когда пользователь пытается получить доступ к защищенным ресурсам в приложении.</span><span class="sxs-lookup"><span data-stu-id="4a9af-146">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="4a9af-147">Членами групп безопасности могут быть как пользователи, так и другие группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="4a9af-147">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="4a9af-148">Группы безопасности, поддерживающие почту, используются так же, как и обычные группы безопасности, но включают общий почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="4a9af-148">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="4a9af-149">Группы безопасности, поддерживающие почту, нельзя создавать через API, но с ними можно выполнять все остальные операции для групп.</span><span class="sxs-lookup"><span data-stu-id="4a9af-149">Mail-enabled security groups can't be created through the API, but other group operations work.</span></span>  <span data-ttu-id="4a9af-150">Группы безопасности, поддерживающие почту, доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a9af-150">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="4a9af-151">Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange](/Exchange/recipients/mail-enabled-security-groups).</span><span class="sxs-lookup"><span data-stu-id="4a9af-151">Learn more in the [Manage mail-enabled security groups Exchange article](/Exchange/recipients/mail-enabled-security-groups).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="4a9af-152">Пример группы безопасности</span><span class="sxs-lookup"><span data-stu-id="4a9af-152">Security group example</span></span>

<span data-ttu-id="4a9af-153">Ниже показано представление группы безопасности в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a9af-153">The following is a JSON representation of a security group.</span></span>

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
## <a name="dynamic-membership"></a><span data-ttu-id="4a9af-154">Динамическое членство</span><span class="sxs-lookup"><span data-stu-id="4a9af-154">Dynamic membership</span></span>

<span data-ttu-id="4a9af-155">Для любых групп можно задавать правила динамического членства, которые автоматически добавляют или удаляют членов группы в соответствии со свойствами пользователей.</span><span class="sxs-lookup"><span data-stu-id="4a9af-155">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="4a9af-156">Например, группа "Marketing employees" (Сотрудники маркетингового отдела) должна включать всех пользователей, для которых в свойстве отдела задано значение "Marketing" (Маркетинг). Новые сотрудники этого отдела должны автоматически добавляться в группу, а сотрудники, покидающие отдел, — автоматически удаляться из нее.</span><span class="sxs-lookup"><span data-stu-id="4a9af-156">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="4a9af-157">Это правило можно указать в поле membershipRule во время создания группы, используя следующий формат: `"membershipRule": 'user.department -eq "Marketing"'`.</span><span class="sxs-lookup"><span data-stu-id="4a9af-157">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="4a9af-158">Значение GroupTypes также должно включать строку `"DynamicMembership"`.</span><span class="sxs-lookup"><span data-stu-id="4a9af-158">GroupTypes must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="4a9af-159">Приведенный ниже запрос создает группу Microsoft 365 для сотрудников маркетингового отдела.</span><span class="sxs-lookup"><span data-stu-id="4a9af-159">The following request creates a new Microsoft 365 group for the marketing employees:</span></span>

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

<span data-ttu-id="4a9af-160">Дополнительные сведения о составлении правил членства см. в статье [Создание правил на основе атрибутов для динамического членства в группах в Azure Active Directory](/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="4a9af-160">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="4a9af-161">**Примечание.** Чтобы правила динамического членства работали, у клиента должна быть лицензия на уровне [Azure Active Directory Premium P1](https://azure.microsoft.com/pricing/details/active-directory/) или выше.</span><span class="sxs-lookup"><span data-stu-id="4a9af-161">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="4a9af-162">Группы других типов</span><span class="sxs-lookup"><span data-stu-id="4a9af-162">Other types of groups</span></span>

<span data-ttu-id="4a9af-163">Группы Microsoft 365 в Yammer используются для организации совместной работы пользователей с помощью записей Yammer.</span><span class="sxs-lookup"><span data-stu-id="4a9af-163">Microsoft 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="4a9af-164">Группы такого типа можно возвращать с помощью запроса на чтение, но записи из них недоступны через API.</span><span class="sxs-lookup"><span data-stu-id="4a9af-164">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="4a9af-165">Если в группе включены записи и каналы бесед Yammer, то стандартные групповые беседы Microsoft 365 отключены.</span><span class="sxs-lookup"><span data-stu-id="4a9af-165">When Yammer posts and conversation feeds are enabled on a group, default Microsoft 365 group conversations are disabled.</span></span> <span data-ttu-id="4a9af-166">Дополнительные сведения см. в [документах, посвященных API Yammer для разработчиков](https://developer.yammer.com/docs).</span><span class="sxs-lookup"><span data-stu-id="4a9af-166">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="group-based-licensing"></a><span data-ttu-id="4a9af-167">Лицензирование на основе групп</span><span class="sxs-lookup"><span data-stu-id="4a9af-167">Group-based licensing</span></span>

<span data-ttu-id="4a9af-168">С помощью лицензирования на основе групп вы можете назначить одну или несколько лицензий на продукты группе Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4a9af-168">You can use group-based licensing to assign one or more product licenses to an Azure AD group.</span></span> <span data-ttu-id="4a9af-169">Azure AD обеспечит назначение лицензий всем участникам этой группы.</span><span class="sxs-lookup"><span data-stu-id="4a9af-169">Azure AD ensures that the licenses are assigned to all members of the group.</span></span> <span data-ttu-id="4a9af-170">Всем новым участникам, присоединившимся к группе, назначаются соответствующие лицензии.</span><span class="sxs-lookup"><span data-stu-id="4a9af-170">Any new members who join the group are assigned the appropriate licenses.</span></span> <span data-ttu-id="4a9af-171">При выходе участников из группы эти лицензии удаляются.</span><span class="sxs-lookup"><span data-stu-id="4a9af-171">When they leave the group, those licenses are removed.</span></span> <span data-ttu-id="4a9af-172">Эта возможность доступна только для групп безопасности и групп Microsoft 365 с параметром `securityEnabled=TRUE`.</span><span class="sxs-lookup"><span data-stu-id="4a9af-172">The feature can only be used with security groups and Microsoft 365 groups that have `securityEnabled=TRUE`.</span></span> <span data-ttu-id="4a9af-173">Дополнительные сведения о лицензировании на основе групп см. в статье [Что такое лицензии групп в Azure Active Directory?](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="4a9af-173">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory?](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="4a9af-174">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="4a9af-174">Common use cases</span></span>

<span data-ttu-id="4a9af-175">Ниже перечислены некоторые распространенные операции, которые можно выполнять с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4a9af-175">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="4a9af-176">**Варианты использования**</span><span class="sxs-lookup"><span data-stu-id="4a9af-176">**Use cases**</span></span>  | <span data-ttu-id="4a9af-177">**Ресурсы REST**</span><span class="sxs-lookup"><span data-stu-id="4a9af-177">**REST resources**</span></span> | <span data-ttu-id="4a9af-178">**См. также**</span><span class="sxs-lookup"><span data-stu-id="4a9af-178">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="4a9af-179">**Объект и методы группы**</span><span class="sxs-lookup"><span data-stu-id="4a9af-179">**Group object and methods**</span></span> | | |
| <span data-ttu-id="4a9af-180">Создание новых групп и получение существующих, обновление свойств и удаление групп.</span><span class="sxs-lookup"><span data-stu-id="4a9af-180">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="4a9af-181">В настоящее время с помощью API можно создавать только группы безопасности и группы Outlook.</span><span class="sxs-lookup"><span data-stu-id="4a9af-181">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="4a9af-182">group</span><span class="sxs-lookup"><span data-stu-id="4a9af-182">group</span></span>](group.md) | [<span data-ttu-id="4a9af-183">Создание групп</span><span class="sxs-lookup"><span data-stu-id="4a9af-183">Create new groups</span></span>](../api/group-post-groups.md) <br/> [<span data-ttu-id="4a9af-184">Перечисление групп</span><span class="sxs-lookup"><span data-stu-id="4a9af-184">List groups</span></span>](../api/group-list.md) <br/> [<span data-ttu-id="4a9af-185">Обновление групп</span><span class="sxs-lookup"><span data-stu-id="4a9af-185">Update groups</span></span>](../api/group-update.md) <br/> [<span data-ttu-id="4a9af-186">Удаление групп</span><span class="sxs-lookup"><span data-stu-id="4a9af-186">Delete groups</span></span>](../api/group-delete.md) |
| <span data-ttu-id="4a9af-187">**Методы для членства в группах**</span><span class="sxs-lookup"><span data-stu-id="4a9af-187">**Group membership methods**</span></span> | | |
| <span data-ttu-id="4a9af-188">Перечисление, добавление и удаление членов групп.</span><span class="sxs-lookup"><span data-stu-id="4a9af-188">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="4a9af-189">user</span><span class="sxs-lookup"><span data-stu-id="4a9af-189">user</span></span>](user.md) <br/> [<span data-ttu-id="4a9af-190">group</span><span class="sxs-lookup"><span data-stu-id="4a9af-190">group</span></span>](group.md)| [<span data-ttu-id="4a9af-191">Перечисление членов</span><span class="sxs-lookup"><span data-stu-id="4a9af-191">List members</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="4a9af-192">Добавление члена</span><span class="sxs-lookup"><span data-stu-id="4a9af-192">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="4a9af-193">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="4a9af-193">Remove member</span></span>](../api/group-delete-members.md)|
| <span data-ttu-id="4a9af-194">Проверка членства пользователя в группе, получение всех групп, в которых состоит пользователь.</span><span class="sxs-lookup"><span data-stu-id="4a9af-194">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="4a9af-195">user</span><span class="sxs-lookup"><span data-stu-id="4a9af-195">user</span></span>](user.md) <br/> [<span data-ttu-id="4a9af-196">group</span><span class="sxs-lookup"><span data-stu-id="4a9af-196">group</span></span>](group.md)| [<span data-ttu-id="4a9af-197">Проверка членства в группах</span><span class="sxs-lookup"><span data-stu-id="4a9af-197">Check member groups</span></span>](../api/group-checkmembergroups.md) <br/> [<span data-ttu-id="4a9af-198">Получение групп пользователя</span><span class="sxs-lookup"><span data-stu-id="4a9af-198">Get member groups</span></span>](../api/group-getmembergroups.md)|
| <span data-ttu-id="4a9af-199">Перечисление, добавление и удаление владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="4a9af-199">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="4a9af-200">user</span><span class="sxs-lookup"><span data-stu-id="4a9af-200">user</span></span>](user.md) <br/> [<span data-ttu-id="4a9af-201">group</span><span class="sxs-lookup"><span data-stu-id="4a9af-201">group</span></span>](group.md)| [<span data-ttu-id="4a9af-202">Перечисление владельцев</span><span class="sxs-lookup"><span data-stu-id="4a9af-202">List owners</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="4a9af-203">Добавление члена</span><span class="sxs-lookup"><span data-stu-id="4a9af-203">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="4a9af-204">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="4a9af-204">Remove member</span></span>](../api/group-delete-members.md)|

## <a name="whats-new"></a><span data-ttu-id="4a9af-205">Новые возможности</span><span class="sxs-lookup"><span data-stu-id="4a9af-205">What's new</span></span>
<span data-ttu-id="4a9af-206">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="4a9af-206">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>