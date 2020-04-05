---
title: Создание команд и управление участниками с помощью Microsoft Graph
description: 'Создание группы, включающей команду, состоит из следующих действий: '
author: hachandr
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 3eb6871cbe4b68addf3924b3641cf5559a78374f
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144343"
---
# <a name="creating-teams-and-managing-members-using-microsoft-graph"></a><span data-ttu-id="36afc-103">Создание команд и управление участниками с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="36afc-103">Creating teams and managing members using Microsoft Graph</span></span>

<span data-ttu-id="36afc-104">Вы можете использовать API Microsoft Teams и Microsoft Graph, чтобы создавать команды разными способами.</span><span class="sxs-lookup"><span data-stu-id="36afc-104">You can use the Microsoft Teams API in Microsoft Graph to create teams in multiple ways.</span></span> <span data-ttu-id="36afc-105">В этой статье описан рекомендуемый подход для достижения наилучших результатов.</span><span class="sxs-lookup"><span data-stu-id="36afc-105">This article describes the approach that we recommend for the best results.</span></span>


## <a name="initial-team-creation"></a><span data-ttu-id="36afc-106">Исходное создание команды</span><span class="sxs-lookup"><span data-stu-id="36afc-106">Initial team creation</span></span>

<span data-ttu-id="36afc-107">Все команды дублируются группами Office 365.</span><span class="sxs-lookup"><span data-stu-id="36afc-107">All teams are backed by Office 365 groups.</span></span> <span data-ttu-id="36afc-108">Самый быстрый способ начать работу при создании команд с помощью Microsoft Graph — настроить новую группу Office 365, всех ее владельцев и участников, а затем преобразовать ее в команду.</span><span class="sxs-lookup"><span data-stu-id="36afc-108">The quickest way to get your team up and running when you create new teams via Microsoft Graph is to set up a new Office 365 group, all all owners and members, and convert that into a team.</span></span>

1. <span data-ttu-id="36afc-109">Создайте [группу Office 365](https://support.office.com/article/learn-about-office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2) с помощью операции [создания группы](/graph/api/group-post-groups?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="36afc-109">Create an [Office 365 group](https://support.office.com/article/learn-about-office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2) using the [create group](/graph/api/group-post-groups?view=graph-rest-beta) operation.</span></span> <span data-ttu-id="36afc-110">Если вы пытаетесь настроить команду класса, используйте операцию [создания educationClass](/graph/api/educationroot-post-classes?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="36afc-110">If you're trying to set up a class team, use the [create educationClass](/graph/api/educationroot-post-classes?view=graph-rest-beta) operation.</span></span> <span data-ttu-id="36afc-111">Вы можете указать владельцев и участников.</span><span class="sxs-lookup"><span data-stu-id="36afc-111">You can specify owners and members.</span></span> <span data-ttu-id="36afc-112">Убедитесь в использовании соответствующих владельцев для создаваемой команды, как описано в шаге 2.</span><span class="sxs-lookup"><span data-stu-id="36afc-112">Make sure that you have the right owners for the newly created team, as described in Step 2.</span></span>

    <span data-ttu-id="36afc-113">Чтобы добавить команду, вам необходимо настроить следующие значения свойств, как показано ниже:</span><span class="sxs-lookup"><span data-stu-id="36afc-113">In order to include a team, you need to set the following property values, as shown:</span></span>

    - <span data-ttu-id="36afc-114">**groupTypes** = { "Unified" }</span><span class="sxs-lookup"><span data-stu-id="36afc-114">**groupTypes** = { "Unified" }</span></span> 
    - <span data-ttu-id="36afc-115">**mailEnabled** = true</span><span class="sxs-lookup"><span data-stu-id="36afc-115">**mailEnabled** = true</span></span>
    - <span data-ttu-id="36afc-116">**securityEnabled** = false</span><span class="sxs-lookup"><span data-stu-id="36afc-116">**securityEnabled** = false</span></span>

    ```http
    POST /groups
    {
        "displayName":"Flight 157",
        "mailNickname":"flight157",
        "description":"Everything about flight 157",
        "visibility":"Private",
        "groupTypes":["Unified"],
        "mailEnabled":true,
        "securityEnabled":false,
        "members@odata.bind":[
            "https://graph.microsoft.com/v1.0/users/bec05f3d-a818-4b58-8c2e-2b4e74b0246d",
            "https://graph.microsoft.com/v1.0/users/ae67a4f4-2308-4522-9021-9f402ff0fba8",
            "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783",
            "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133"
        ],
        "owners@odata.bind":[
            "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133",
            "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783"
        ]
    }
    ```

    <span data-ttu-id="36afc-117">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="36afc-117">The following example shows the response.</span></span> 

    ><span data-ttu-id="36afc-118">**Примечание.** Показанный объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="36afc-118">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="36afc-119">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36afc-119">All the properties will be returned from an actual call.</span></span>

    ```http
    HTTP/1.1 200 OK
    Content-type: application/json
    Content-length: xxx
    {
        "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
        "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
    }
    ```

2. <span data-ttu-id="36afc-120">Обеспечьте для команды наличие двух или более владельцев.</span><span class="sxs-lookup"><span data-stu-id="36afc-120">Ensure the team has two or more owners.</span></span> <span data-ttu-id="36afc-121">Это можно сделать с помощью операции [добавления владельца](/graph/api/group-post-owners?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="36afc-121">You can do so via the [add owner](/graph/api/group-post-owners?view=graph-rest-beta) operation.</span></span> <span data-ttu-id="36afc-122">Они должны быть реальными учетными записями пользователей, а не учетными записями служб.</span><span class="sxs-lookup"><span data-stu-id="36afc-122">These should be real user accounts and not service accounts.</span></span> <span data-ttu-id="36afc-123">Наличие двух владельцев помогает обслуживать сценарии, когда один владелец покидает компанию или недоступен для выполнения операций управления командой.</span><span class="sxs-lookup"><span data-stu-id="36afc-123">Having two owners helps handle cases where one owner leaves the company or is unavailable to perform team management operations.</span></span>

3. <span data-ttu-id="36afc-124">Добавьте всех участников (и гостей, если это необходимо) в группу с помощью операции [добавления участника](/graph/api/group-post-members?view=graph-rest-beta), если это не сделано на шаге 1.</span><span class="sxs-lookup"><span data-stu-id="36afc-124">Add all members (and guests if necessary) to the group using the [add member](/graph/api/group-post-members?view=graph-rest-beta) operation, if you did not do so in Step 1.</span></span>

4. <span data-ttu-id="36afc-125">После успешного создания группы, что может занять до 15 минут после выполнения шага 1, создайте команду Microsoft Teams с помощью операции [создания команды из группы](/graph/api/team-put-teams?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="36afc-125">After the group is successfully created, which can take upto 15 minutes after completing Step 1, create a Microsoft Teams team using the [create team from group](/graph/api/team-put-teams?view=graph-rest-beta) operation.</span></span> <span data-ttu-id="36afc-126">Если вы столкнулись с ошибкой, процесс создания группы, возможно, не завершен. Попробуйте подождать несколько минут.</span><span class="sxs-lookup"><span data-stu-id="36afc-126">If you run into an error, the group creation process might not be completed; try waiting a few more minutes.</span></span>

    ```http
    PUT /groups/{id}/team
    { }
    ```

    <span data-ttu-id="36afc-127">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="36afc-127">The following example shows the response.</span></span> 

    ><span data-ttu-id="36afc-128">**Примечание.** Показанный объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="36afc-128">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="36afc-129">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36afc-129">All the properties will be returned from an actual call.</span></span>

    ```http
    HTTP/1.1 200 OK
    Content-type: application/json
    Content-length: xxx
    {
        "@odata.context" : "https://graph.microsoft.com/v1.0/$metadata#teams/$entity",
        "id" : "b7f968af-ca51-42f6-a77e-82c7147bc8f2",
        "webUrl" : "https://example.com",
        "isArchived" : null,
        "memberSettings" : { },
        "guestSettings" : { },
        "messagingSettings" : { },
        "funSettings" : {}
    }
    ```

    <span data-ttu-id="36afc-130">Идентификатор созданной команды такой же, как и идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="36afc-130">The created team has the same ID as the group.</span></span>

5. <span data-ttu-id="36afc-131">После завершения этого процесса все владельцы и участники должны увидеть созданную команду в клиенте Teams.</span><span class="sxs-lookup"><span data-stu-id="36afc-131">After this process finishes, all owners and members should be able to see the newly created team in their Teams client.</span></span>

## <a name="adding-or-managing-members"></a><span data-ttu-id="36afc-132">Добавление участников и управление ими</span><span class="sxs-lookup"><span data-stu-id="36afc-132">Adding or managing members</span></span>

<span data-ttu-id="36afc-133">Чтобы добавить участников после создания команды, используйте операцию [добавления участника](/graph/api/group-post-members?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="36afc-133">To add members after a team is created, you use the [add member](/graph/api/group-post-members?view=graph-rest-beta) operation.</span></span> <span data-ttu-id="36afc-134">Учитывайте следующее касательно изменений участия:</span><span class="sxs-lookup"><span data-stu-id="36afc-134">Note the following with respect to membership changes:</span></span>

1. <span data-ttu-id="36afc-135">Изменения участия, внесенные в группу Office 365, синхронизируются с Teams с помощью фонового механизма синхронизации, который обычно занимает 24 часа (или больше в некоторых случаях).</span><span class="sxs-lookup"><span data-stu-id="36afc-135">Membership changes made to Office 365 groups sync to Teams via a background sync mechanism that typically takes 24 hours (or more in some cases).</span></span>

2. <span data-ttu-id="36afc-136">Фоновый процесс запускается, если один или несколько пользователей команды (владелец или участник) активны в классическом клиенте Teams.</span><span class="sxs-lookup"><span data-stu-id="36afc-136">The background process is triggered only if one or more users in the team (owner or member) is active in the Teams desktop client.</span></span> <span data-ttu-id="36afc-137">Активность заключается в запуске приложения Teams и/или его работе, пользователю не требуется специально посещать команду, которая изменяется.</span><span class="sxs-lookup"><span data-stu-id="36afc-137">Launching the Teams application and/or having it running constitutes activity — a user does not need to visit the team that is being modified specifically.</span></span>

    ><span data-ttu-id="36afc-138">**Примечание.** Мобильные клиенты Teams не запускают синхронизацию участия. По крайней мере один пользователь должен находиться в классическом клиенте, чтобы обеспечить правильное выполнение фонового процесса.</span><span class="sxs-lookup"><span data-stu-id="36afc-138">**Note:** The Teams mobile clients do not trigger the membership sync. At least one user should be on the desktop client to that ensure this background process goes smoothly.</span></span>

## <a name="checklist-for-validation"></a><span data-ttu-id="36afc-139">Контрольный список для проверки</span><span class="sxs-lookup"><span data-stu-id="36afc-139">Checklist for validation</span></span>

<span data-ttu-id="36afc-140">После создания команды вы можете воспользоваться следующим контрольным списком, чтобы проверить успешность создания команды.</span><span class="sxs-lookup"><span data-stu-id="36afc-140">After you create a team, you can use the following checklist to verify that the team was created successfully.</span></span>

### <a name="validate-team-creation"></a><span data-ttu-id="36afc-141">Проверка создания команды</span><span class="sxs-lookup"><span data-stu-id="36afc-141">Validate team creation</span></span>

1. <span data-ttu-id="36afc-142">Убедитесь, что создана группа Office 365, дублирующая команду, с помощью Центров администрирования Azure AD или Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="36afc-142">Verify that the Office 365 group backing the team is created via the Azure AD or Microsoft 365 admin centers.</span></span>

2. <span data-ttu-id="36afc-143">Убедитесь, что команда успешно создана, в портале администрирования Teams.</span><span class="sxs-lookup"><span data-stu-id="36afc-143">Verify that the team creation succeeded via the Teams admin portal.</span></span>

3. <span data-ttu-id="36afc-144">Проверьте, что у команды есть соответствующие владельцы и участники, с помощью портала администрирования Teams.</span><span class="sxs-lookup"><span data-stu-id="36afc-144">Verify that the team has the correct owners and members listed via the Teams admin portal.</span></span>

4. <span data-ttu-id="36afc-145">Убедитесь, что владельцы команды видят команду после входа в классический или веб-клиент Teams.</span><span class="sxs-lookup"><span data-stu-id="36afc-145">Verify that the team owners can see the team after signing into the Teams desktop or web client.</span></span>

5. <span data-ttu-id="36afc-146">Убедитесь, что участники видят команду после входа в классический или веб-клиент Teams.</span><span class="sxs-lookup"><span data-stu-id="36afc-146">Verify that members can see the team after signing into the Teams desktop or web client.</span></span>

### <a name="validate-addition-of-members"></a><span data-ttu-id="36afc-147">Проверка добавления участников</span><span class="sxs-lookup"><span data-stu-id="36afc-147">Validate addition of members</span></span>

1. <span data-ttu-id="36afc-148">Проверьте, что новые участники отображаются в группе, с помощью Центра администрирования Azure AD или Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="36afc-148">Verify that newly members show up in the group via the Azure AD or Microsoft 365 admin center.</span></span>

2. <span data-ttu-id="36afc-149">Убедитесь, что добавленные участники видят команду после входа в классический или веб-клиент Teams.</span><span class="sxs-lookup"><span data-stu-id="36afc-149">Verify that newly added members can see the team after signing into the Teams desktop or web client.</span></span>



## <a name="how-office-365-group-membership-changes-are-synchronized-to-microsoft-teams"></a><span data-ttu-id="36afc-150">Как изменения участия в группе в Office 365 синхронизируются с Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="36afc-150">How Office 365 group membership changes are synchronized to Microsoft Teams</span></span>

<span data-ttu-id="36afc-151">Изменения участия в группе Office 365, дублирующей команду, внесенные с помощью API Microsoft Graph или портала администрирования (за пределами клиента Teams), должны синхронизироваться со службой Teams, чтобы добавленные пользователи могли видеть команду и участвовать в ней.</span><span class="sxs-lookup"><span data-stu-id="36afc-151">Membership changes made to an Office 365 group backing a team via the Microsoft Graph API or through the admin portal (outside of the Teams client) have to sync to the Teams service in order for newly added users to be able to see and participate in the team.</span></span> <span data-ttu-id="36afc-152">Непосредственные изменения участия в группе синхронизируются со службой Teams с помощью фонового процесса.</span><span class="sxs-lookup"><span data-stu-id="36afc-152">Changes made directly to the group membership are synchronized to the Teams service via a background process.</span></span> <span data-ttu-id="36afc-153">Фоновый процесс работает в службе Teams и запускается действиями пользователей в классическом и веб-клиенте Teams.</span><span class="sxs-lookup"><span data-stu-id="36afc-153">This background process runs in the Teams service and is triggered by user activity in Teams desktop and web clients.</span></span>

<span data-ttu-id="36afc-154">Чтобы процесс запустился, у текущего владельца или участника команды (пользователь, который может просматривать команду в клиенте Teams) должен быть открыт классический (идеальный вариант) или веб-клиент Teams.</span><span class="sxs-lookup"><span data-stu-id="36afc-154">For the process to get triggered, a current owner or member of that team (someone who can see the team in the Teams client) must have the Teams desktop (ideally) or web client open.</span></span> <span data-ttu-id="36afc-155">Мобильные клиенты не запускают синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="36afc-155">Mobile clients do not trigger this sync.</span></span>

<span data-ttu-id="36afc-156">Текущее соглашение об уровне обслуживания для синхронизации с Teams изменений участия, внесенных в группы, составляет до 24 часов после запуска синхронизации действиями клиента.</span><span class="sxs-lookup"><span data-stu-id="36afc-156">The current SLA for synchronizing membership changes made to groups to Teams is up to 24 hours after the sync is triggered by client activity.</span></span> <span data-ttu-id="36afc-157">При определенных обстоятельствах это может занять больше времени (например, из-за загрузки службы).</span><span class="sxs-lookup"><span data-stu-id="36afc-157">It can take longer under certain circumstances (due to service load, for example).</span></span>


![Процесс синхронизации состава.](images/teams-roster-sync.png)

