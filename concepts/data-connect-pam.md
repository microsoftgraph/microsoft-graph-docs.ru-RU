---
title: Интеграция подключения к данным Microsoft Graph с Privileged Access Management
description: Подключение к данным Microsoft Graph использует Privileged Access Management, чтобы позволить администраторам Microsoft 365 утверждать запросы на перемещение данных.
author: fercobo-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 3631b652c5e17c333548662b429a56ce3015f55b
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629324"
---
# <a name="microsoft-graph-data-connect-integration-with-privileged-access-management"></a><span data-ttu-id="d7a69-103">Интеграция подключения к данным Microsoft Graph с Privileged Access Management</span><span class="sxs-lookup"><span data-stu-id="d7a69-103">Microsoft Graph Data Connect integration with Privileged Access Management</span></span>

<span data-ttu-id="d7a69-104">Подключение к данным Microsoft Graph использует Privileged Access Management (PAM), чтобы позволить администраторам Microsoft 365 утверждать запросы на перемещение данных.</span><span class="sxs-lookup"><span data-stu-id="d7a69-104">Microsoft Graph Data Connect relies on Privileged Access Management (PAM) to allow Microsoft 365 administrators to approve data movement requests.</span></span> <span data-ttu-id="d7a69-105">Конвейеры подключения к данным должны утверждаться участником группы утверждающих запросы на доступ к данным, который указывается администратором Microsoft 365 во время включения.</span><span class="sxs-lookup"><span data-stu-id="d7a69-105">Data Connect pipelines must be approved by a member of the data access request approver specified by the Microsoft 365 administrator during enablement.</span></span> <span data-ttu-id="d7a69-106">Чтобы настроить группу утверждающих, см. статью [Начало работы](data-connect-get-started.md).</span><span class="sxs-lookup"><span data-stu-id="d7a69-106">To set up the approver group, see [Get started](data-connect-get-started.md).</span></span>

<span data-ttu-id="d7a69-107">Каждому участнику группы утверждающих высылаются электронные письма с запросом на утверждение, чтобы уведомить их, когда действия копирования запрашивают доступ для извлечения данных Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d7a69-107">Approval request emails will be sent to each member of the approver group to notify them when copy activities request access to extract Microsoft 365 data.</span></span> <span data-ttu-id="d7a69-108">Утверждающие могут утверждать или отклонять эти запросы, указывать группу пользователей, из которой следует удалить извлекаемые данные, или отозвать ранее утвержденный запрос.</span><span class="sxs-lookup"><span data-stu-id="d7a69-108">Approvers can approve or deny these requests, specify a user group that should be scrubbed out of extracted data, or revoke a previously approved request.</span></span> <span data-ttu-id="d7a69-109">Утверждения сохраняются 6 месяцев, и требуется одно утверждение на каждое действие копирования в конвейере фабрики данных Azure.</span><span class="sxs-lookup"><span data-stu-id="d7a69-109">Approvals persist for 6 months, and one approval is needed per copy activity in the Azure Data Factory pipeline.</span></span>

<span data-ttu-id="d7a69-110">Каждый запрос всегда включает следующие сведения о наборе данных и пользователях, к которым относятся извлекаемые данные:</span><span class="sxs-lookup"><span data-stu-id="d7a69-110">Every request will always include the following details about the dataset and the users about whom data is being extracted:</span></span>

* <span data-ttu-id="d7a69-111">**Запрашивающий**. Пользователь, запросивший конвейер.</span><span class="sxs-lookup"><span data-stu-id="d7a69-111">**Requestor**: The user who requested the pipeline.</span></span>
* <span data-ttu-id="d7a69-112">**Длительность**. Длительность сохранения утверждения (в случае утверждения).</span><span class="sxs-lookup"><span data-stu-id="d7a69-112">**Duration**: If approved, how long the approval will persist.</span></span> <span data-ttu-id="d7a69-113">Всегда 4320 часов (6 месяцев).</span><span class="sxs-lookup"><span data-stu-id="d7a69-113">Always 4320 hours (6 months).</span></span>
* <span data-ttu-id="d7a69-114">**Причина**. Причина запроса, обычно следующая: "Приложению, установленному для организации, требуется утверждение на доступ к данным Office 365".</span><span class="sxs-lookup"><span data-stu-id="d7a69-114">**Reason**: Reason for the request, typically "An app installed for your organization requires approval for access to Office 365 Data."</span></span>
* <span data-ttu-id="d7a69-115">**Время запроса**. Дата и время запроса.</span><span class="sxs-lookup"><span data-stu-id="d7a69-115">**Requested at**: The DateTime of the request.</span></span>
* <span data-ttu-id="d7a69-116">**ИД запроса**. Идентификатор запроса для целей утверждения.</span><span class="sxs-lookup"><span data-stu-id="d7a69-116">**Request id**: The ID of the request, used for approval purposes.</span></span>
* <span data-ttu-id="d7a69-117">**DataTable**. Набор извлекаемых данных (например, отправленные элементы).</span><span class="sxs-lookup"><span data-stu-id="d7a69-117">**DataTable**: The data set being extracted (for example, Sent Items).</span></span>
* <span data-ttu-id="d7a69-118">**Столбцы**. Список столбцов, извлекаемых из таблицы данных (например, SentDateTime).</span><span class="sxs-lookup"><span data-stu-id="d7a69-118">**Columns**: The list of columns being extracted from the data table (for example, SentDateTime).</span></span>
* <span data-ttu-id="d7a69-119">**AllowedGroups**. Группа или группы пользователей, данные которых извлекает конвейер.</span><span class="sxs-lookup"><span data-stu-id="d7a69-119">**AllowedGroups**: The group or groups of users against whom the pipeline is extracting data.</span></span> <span data-ttu-id="d7a69-120">Если список групп пуст, конвейер запрашивает доступ к данным всех пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d7a69-120">If the list of groups is empty, the pipeline is requesting access to data from all users in the tenant.</span></span>
* <span data-ttu-id="d7a69-121">**Запрос области пользователей**. Предикат, используемый для фильтрации пользователей.</span><span class="sxs-lookup"><span data-stu-id="d7a69-121">**User Scope Query**: The predicate used to filter out users.</span></span> <span data-ttu-id="d7a69-122">Применяется только при запросе всех пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d7a69-122">Only applies if the request is for all users in the tenant.</span></span> <span data-ttu-id="d7a69-123">Если этот параметр пуст, фильтр не применяется.</span><span class="sxs-lookup"><span data-stu-id="d7a69-123">If this is empty, no filter is applied.</span></span>
* <span data-ttu-id="d7a69-124">**OutputUri**. Выходной путь, в котором хранятся извлеченные данные.</span><span class="sxs-lookup"><span data-stu-id="d7a69-124">**OutputUri**: The output path in which the extracted data will be stored.</span></span>
* <span data-ttu-id="d7a69-125">**SourceTenantId**. Идентификатор клиента, из которого извлекаются данные.</span><span class="sxs-lookup"><span data-stu-id="d7a69-125">**SourceTenantId**: The tenant ID from which data is being extracted.</span></span>
* <span data-ttu-id="d7a69-126">**InstallerIdentity**. Удостоверение установщика приложения.</span><span class="sxs-lookup"><span data-stu-id="d7a69-126">**InstallerIdentity**: The identity of the app installer.</span></span>

<span data-ttu-id="d7a69-127">Следующие поля в запросе доступны только в некоторых случаях:</span><span class="sxs-lookup"><span data-stu-id="d7a69-127">The following fields in the request will be available only in some cases:</span></span>

* <span data-ttu-id="d7a69-128">Имя приложения и URI Marketplace (доступно только для приложений, установленных из Azure Marketplace).</span><span class="sxs-lookup"><span data-stu-id="d7a69-128">Application Name and the Marketplace URI (available only for applications installed from the Azure marketplace).</span></span>
* <span data-ttu-id="d7a69-129">Ссылки на политику конфиденциальности приложения и условия использования (доступны только при предоставлении приложением).</span><span class="sxs-lookup"><span data-stu-id="d7a69-129">Links to the application's privacy policy and terms of service (available only if the application provides it).</span></span>
* <span data-ttu-id="d7a69-130">Политики соответствия требованиям, применяемые приложением, например шифрование неактивных данных в выходном хранилище (доступны только при предоставлении приложением, и если приложение установлено из Azure Marketplace).</span><span class="sxs-lookup"><span data-stu-id="d7a69-130">The compliance policies that the application enforces, such as data encryption at rest in the output storage location (available only if the application provides it and if the application is installed from the Azure marketplace).</span></span>
* <span data-ttu-id="d7a69-131">Список запрещенных — группа пользователей, для которой может выполняться очистка извлеченных данных.</span><span class="sxs-lookup"><span data-stu-id="d7a69-131">Deny List - The user group that can be scrubbed out of the extracted data.</span></span> <span data-ttu-id="d7a69-132">Это поле не заполняется при запросе наборов данных, поддерживающих очистку извлеченных данных с целью обеспечения конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d7a69-132">This field is empty as a part of the request for datasets that support privacy scrubbing of extracted data.</span></span> <span data-ttu-id="d7a69-133">Оно может заполняться участником группы утверждающих, который утверждает запрос в соответствующее время.</span><span class="sxs-lookup"><span data-stu-id="d7a69-133">It can be populated by the member of the approver group who approves the request at approval time.</span></span>

## <a name="approving-requests"></a><span data-ttu-id="d7a69-134">Утверждение запросов</span><span class="sxs-lookup"><span data-stu-id="d7a69-134">Approving requests</span></span>

<span data-ttu-id="d7a69-135">Конвейеры подключения к данным должны утверждаться участником группы утверждающих запросы на доступ к данным.</span><span class="sxs-lookup"><span data-stu-id="d7a69-135">Data Connect pipelines must be approved by a member of a data access request approver group.</span></span> <span data-ttu-id="d7a69-136">Утверждающие могут утверждать, отклонять или отзывать конвейеры с помощью модуля PowerShell для Exchange Online или пользовательского интерфейса PAM.</span><span class="sxs-lookup"><span data-stu-id="d7a69-136">Approvers can approve, deny, or revoke pipelines by using the Exchange Online PowerShell module or the PAM user experience.</span></span>

### <a name="approving-denying-and-revoking-requests-by-using-powershell"></a><span data-ttu-id="d7a69-137">Утверждение, отклонение и отзыв запросов с помощью PowerShell</span><span class="sxs-lookup"><span data-stu-id="d7a69-137">Approving, denying, and revoking requests by using PowerShell</span></span>

<span data-ttu-id="d7a69-138">Используйте следующие действия для взаимодействия с запросом с помощью модуля PowerShell для Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="d7a69-138">Use the following steps to interact with a request using the Exchange Online PowerShell module:</span></span>

1. <span data-ttu-id="d7a69-139">Установите модуль PowerShell для Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="d7a69-139">Install the Exchange Online Powershell module.</span></span> <span data-ttu-id="d7a69-140">Инструкции по установке см. в статье [Подключение к Exchange Online PowerShell с помощью многофакторной проверки подлинности](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d7a69-140">For installation instructions, see [Connect to Exchange Online PowerShell using multi-factor authentication](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span></span>

2. <span data-ttu-id="d7a69-141">Подключитесь к Exchange Online PowerShell с помощью многофакторной проверки подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="d7a69-141">Connect to Exchange Online Powershell using multi-factor authentication (MFA).</span></span> <span data-ttu-id="d7a69-142">Инструкции см. в статье [Подключение к Exchange Online PowerShell с помощью многофакторной проверки подлинности](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d7a69-142">For instructions, see [Connect to Exchange Online PowerShell using multi-factor authentication](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span></span>
    > [!NOTE]
    > <span data-ttu-id="d7a69-143">**Примечание**. Вам не нужно включать многофакторную проверку подлинности для своей организации, чтобы использовать эти действия при подключении к Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d7a69-143">**Note**: You do not need to enable multi-factor authentication for your organization to use these steps while connecting to Exchange Online PowerShell.</span></span> <span data-ttu-id="d7a69-144">Подключение с помощью многофакторной проверки подлинности создает маркер OAuth, используемый PAM для подписи ваших запросов.</span><span class="sxs-lookup"><span data-stu-id="d7a69-144">Connecting with MFA creates an OAuth token that is used by PAM for signing your requests.</span></span>

3. <span data-ttu-id="d7a69-145">Выполните вход с помощью своей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="d7a69-145">Sign in with your account.</span></span> <span data-ttu-id="d7a69-146">Обратите внимание, что вы должны быть участником настроенной группы утверждающих доступ к данным, чтобы иметь возможность утверждать, отклонять или отзывать запросы.</span><span class="sxs-lookup"><span data-stu-id="d7a69-146">Note that you must be part of the configured data access approver group in order to be able to approve, deny, or revoke requests.</span></span> <span data-ttu-id="d7a69-147">Гостевые пользователи не могут утверждать запросы, даже если они состоят в группе утверждающих.</span><span class="sxs-lookup"><span data-stu-id="d7a69-147">Guest users cannot approve requests, even if they are in the approver group.</span></span>

   ```powershell
   Connect-EXOPSSession
   ```

4. <span data-ttu-id="d7a69-148">Найдите все ожидающие запросы.</span><span class="sxs-lookup"><span data-stu-id="d7a69-148">Find all pending requests.</span></span>
   > [!NOTE]
   > <span data-ttu-id="d7a69-149">Значение свойства **Identity** будет использоваться для определения и утверждения или отклонения запроса.</span><span class="sxs-lookup"><span data-stu-id="d7a69-149">The value in the **Identity** property will be used to identify and approve or deny the request.</span></span> <span data-ttu-id="d7a69-150">Запишите это значение и используйте его в параметре -RequestId.</span><span class="sxs-lookup"><span data-stu-id="d7a69-150">Note this value and use it in the -RequestId parameter.</span></span>

   ```powershell
   Get-ElevatedAccessRequest | ?{$_.RequestStatus -eq 'Pending'}
   ```

5. <span data-ttu-id="d7a69-151">Подробнее ознакомьтесь с полем **context** нужного запроса.</span><span class="sxs-lookup"><span data-stu-id="d7a69-151">Take a closer look at the **context** field of the request you are interested in.</span></span>
   ><span data-ttu-id="d7a69-152">**Примечание.** Поле context запроса на доступ к данным описывает параметры и свойства действия копирования.</span><span class="sxs-lookup"><span data-stu-id="d7a69-152">**Note:** The context field of the data access request describes the parameters and properties of the copy activity.</span></span>

   ```powershell
   Get-ElevatedAccessRequest -RequestId $requestId).Context | ConvertFrom-Json
   ```

   <span data-ttu-id="d7a69-153">Вы получите примерно следующий ответ.</span><span class="sxs-lookup"><span data-stu-id="d7a69-153">You'll get a response that looks like the following.</span></span>

   ```powershell
   Key                          Value
   ---                          -----
   ApplicationName
   ComplianceStatus             [{"Timestamp":"2018-05-02T18:29:21.5705664Z","RequirementName":"adlsEncryption","PolicyComplianceState":"Compliant","Violations":0},{"Timestamp":"2018-05-02T...
   ApplicationMarketPlaceUri
   OutputUri                    adl://myadlserumvrroyspmq.azuredatalakestore.net/targetFolder/Event
   ApplicationPrivacyPolicyUri  http://www.wkw.com/privacy
   ApplicationTermsOfServiceUri http://www.wkw.com/tos
   InstallerIdentity            a89885c3-4b0e-499e-86ed-14d7ed9147c2@942229f8-4656-4fb0-828b-e938dad4019a
   SourceTenantId               942229f8-4656-4fb0-828b-e938dad4019a
   UserScopeQuery               tenant in (942229f8-4656-4fb0-828b-e938dad4019a)
   ApplicationId
   DataTable                    Calendar Events
   DestinationTenantId          942229f8-4656-4fb0-828b-e938dad4019a
   Columns                      Subject:string, HasAttachments:bool, End:DateTime, Start:DateTime, ResponseStatus:string, Organizer:Object, Attendees:string, Importance:string, Sensitivity:...
   ```

6. <span data-ttu-id="d7a69-154">Утвердите или отклоните запрос, используя значение свойства **Identity** для параметра -RequestId.</span><span class="sxs-lookup"><span data-stu-id="d7a69-154">Approve/deny the request using the value for **Identity** for the -RequestId parameter.</span></span>

   ```powershell
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!"
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

<span data-ttu-id="d7a69-155">Также можно утвердить запрос с использованием списка запрещенных, чтобы не добавлять данные от определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="d7a69-155">You can also approve the request with a deny list to ensure data from certain users is not included.</span></span> <span data-ttu-id="d7a69-156">Для этого нужно изменить контекст запроса, чтобы добавить параметр `object Id` группы, которую нужно пропустить, а затем утвердить запрос.</span><span class="sxs-lookup"><span data-stu-id="d7a69-156">To do so, you need to modify the context of the request to add the `object Id` of the group that you want to omit and then approve the request.</span></span>

   ```powershell
   $request = Get-ElevatedAccessRequest -RequestId
   $hash = $request.Context
   $hash["DenyList"] = <Object ID of denied user group>;
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!" -RequestContext $hash
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

<span data-ttu-id="d7a69-157">Кроме того, вы можете отозвать запросы, которые ранее были утверждены.</span><span class="sxs-lookup"><span data-stu-id="d7a69-157">You can also revoke requests that were previously approved.</span></span> <span data-ttu-id="d7a69-158">Аналогично утверждению запросов потребуется значение свойства **Identity** для параметра -RequestId.</span><span class="sxs-lookup"><span data-stu-id="d7a69-158">Similar to approving requests, the value for **Identity** is what is required in the -RequestId parameter.</span></span>

   ```powershell
   Revoke-ElevatedAccessAuthorization -Comment "Revoking this request!" -RequestId $requestId
   ```

   <span data-ttu-id="d7a69-159">Ответ будет выглядеть приблизительно так:</span><span class="sxs-lookup"><span data-stu-id="d7a69-159">You'll see a response similar to the following.</span></span>

   ```powershell
   AuthorizedBy          : user@tenant.onmicrosoft.com
   Type                  : Task
   AuthorizedAccess      : Data Access Request
   StartTimeUtc          : 7/24/2018 6:02:42 PM
   EndTimeUtc            : 10/22/2018 6:02:42 PM
   Revoked               : True
   RevocationDateTimeUtc : 7/24/2018 9:12:55 PM
   RevokedBy             : NAMPR00A001.prod.outlook.com/Microsoft Exchange Hosted  Organizations/tenant.onmicrosoft.com/user
   RevocationComment     : Revoking this request!
   Identity              : bda75607-0d87-43cb-bdf1-284b18446b34
   DateCreatedUtc        : 1/1/0001 12:00:00 AM
   DateUpdatedUtc        : 7/24/2018 9:12:55 PM
   ```

### <a name="approving-denying-and-revoking-requests-by-using-the-pam-user-experience"></a><span data-ttu-id="d7a69-160">Утверждение, отклонение и отзыв запросов с помощью пользовательского интерфейса PAM</span><span class="sxs-lookup"><span data-stu-id="d7a69-160">Approving, denying, and revoking requests by using the PAM user experience</span></span>

<span data-ttu-id="d7a69-161">Используйте следующие действия для взаимодействия с запросом с помощью веб-интерфейса PAM:</span><span class="sxs-lookup"><span data-stu-id="d7a69-161">Use the following steps to interact with a request using the PAM web experience:</span></span>

1. <span data-ttu-id="d7a69-162">Войдите на портал администрирования Microsoft 365, используя учетные данные администратора, и перейдите на страницу [пользовательского интерфейса утверждения управления привилегированным доступом](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess).</span><span class="sxs-lookup"><span data-stu-id="d7a69-162">Sign in to the Microsoft 365 admin portal using admin credentials and go to the [Privileged Access Managment approval user experience](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess) page.</span></span> <span data-ttu-id="d7a69-163">Будут показаны все запросы на доступ (ожидаемые, утвержденные, истекшие или отклоненные).</span><span class="sxs-lookup"><span data-stu-id="d7a69-163">This will show you all the access requests (pending/approved/expired/denied).</span></span>

2. <span data-ttu-id="d7a69-164">На открывшейся странице выберите нужный запрос.</span><span class="sxs-lookup"><span data-stu-id="d7a69-164">On the resulting page, select the request that you're interested in.</span></span> <span data-ttu-id="d7a69-165">Чтобы выбрать список запрещенных с целью очистки для обеспечения конфиденциальности, щелкните раскрывающийся **список запрещенных**, выберите группу, которую нужно очистить, и нажмите **Утвердить**.</span><span class="sxs-lookup"><span data-stu-id="d7a69-165">To select a deny list for privacy scrubbing, click the **DenyList** dropdown, select the group that needs to be scrubbed, and then select **Approve**.</span></span>

3. <span data-ttu-id="d7a69-166">Чтобы отозвать ранее утвержденный запрос, выберите его и нажмите **Отозвать**.</span><span class="sxs-lookup"><span data-stu-id="d7a69-166">To revoke a previously approved request, select the approved request that needs to be revoked, and choose **Revoke**.</span></span> <span data-ttu-id="d7a69-167">Следующая попытка перенести данные с помощью этого утверждения завершится сбоем.</span><span class="sxs-lookup"><span data-stu-id="d7a69-167">The next attempt to move data using that approval will fail.</span></span>

### <a name="approval-behavior"></a><span data-ttu-id="d7a69-168">Поведение при утверждении</span><span class="sxs-lookup"><span data-stu-id="d7a69-168">Approval behavior</span></span>

<span data-ttu-id="d7a69-169">Запросы на утверждение подключения к данным имеют определенные характеристики, которые важно учитывать:</span><span class="sxs-lookup"><span data-stu-id="d7a69-169">Data Connect approval requests have particular characteristics that are important to be aware of:</span></span>

* <span data-ttu-id="d7a69-p118">Запросы на утверждение основаны на именах фабрики данных Azure, конвейера и действия копирования. При каждом запуске копирования выполняется проверка того, что администратор Microsoft 365 утвердил запрос действия копирования на доступ к данным Office, а также проверка важных параметров действия копирования относительно параметров утверждения.</span><span class="sxs-lookup"><span data-stu-id="d7a69-p118">Approval requests are based on the Azure Data Factory, pipeline and copy activity names. Every copy activity run will verify that the Microsoft 365 admin has approved the copy activity's request to access Office data, and will validate the important parameters of the copy activity run against the parameters of the approval.</span></span>
* <span data-ttu-id="d7a69-172">При определенных условиях автоматически выполняется новый запрос на утверждение.</span><span class="sxs-lookup"><span data-stu-id="d7a69-172">Under certain conditions, a new approval request will automatically be triggered.</span></span> <span data-ttu-id="d7a69-173">Утверждающий подключение к данным должен утвердить новый запрос перед тем, как действие копирования сможет получить доступ к данным Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d7a69-173">A Data Connect approver will have to approve the new request before the copy activity can access Microsoft 365 data.</span></span>
* <span data-ttu-id="d7a69-174">Если параметры выполняемого копирования изменяются, выполняется новый запрос на утверждение.</span><span class="sxs-lookup"><span data-stu-id="d7a69-174">If the parameters of the copy activity run changes, a new approval request will be triggered.</span></span>
* <span data-ttu-id="d7a69-175">Если изменяются имена фабрики данных, конвейера или действия копирования, выполняется новый запрос на утверждение.</span><span class="sxs-lookup"><span data-stu-id="d7a69-175">If the Data Factory, pipeline or copy activity names change, a new approval request will be triggered.</span></span>
* <span data-ttu-id="d7a69-176">Например: потребуется новое утверждение, если изменяется таблица данных или набор столбцов, к которым обращается действие копирования.</span><span class="sxs-lookup"><span data-stu-id="d7a69-176">For example: A new approval will be required if the data table or set of columns that the copy activity is accessing changes.</span></span>
* <span data-ttu-id="d7a69-177">Действия копирования требуется утверждать каждые 6 месяцев.</span><span class="sxs-lookup"><span data-stu-id="d7a69-177">Copy activities will have to be approved once every 6 months.</span></span> <span data-ttu-id="d7a69-178">Если исходное утверждение получено 6 месяцев назад, автоматически выполняется новый запрос на утверждение.</span><span class="sxs-lookup"><span data-stu-id="d7a69-178">If the original approval was approved 6 months ago, a new approval request will automatically be triggered.</span></span>
* <span data-ttu-id="d7a69-179">Если утверждающий запросы на доступ к данным Microsoft 365 отклонил запрос на утверждение или отозвал ранее утвержденный запрос, действие копирования будет постоянно завершаться сбоем.</span><span class="sxs-lookup"><span data-stu-id="d7a69-179">If a Microsoft 365 Data Access approver has denied an approval request or revoked a previously approved request, the copy activity will fail continually.</span></span> <span data-ttu-id="d7a69-180">Вам следует в сотрудничестве с утверждающим выяснить причину отклонения или отзыва и соответствующим образом исправить параметры действия копирования.</span><span class="sxs-lookup"><span data-stu-id="d7a69-180">You should work with the approver to understand the reason for the denial or revocation and fix the parameters of the copy activity accordingly.</span></span> <span data-ttu-id="d7a69-181">Потребуется развернуть новое действие копирования или изменить имя существующего действия копирования, чтобы выполнить новый запрос на утверждение.</span><span class="sxs-lookup"><span data-stu-id="d7a69-181">A new copy activity will have to deployed, or the name of the existing copy activity will have to be changed in order to trigger a new approval request for approval.</span></span>
* <span data-ttu-id="d7a69-182">Запрос на утверждение истекает через 24 часа, если утверждающий запросы на доступ к данным Microsoft 365 не выполняет действий с запросом.</span><span class="sxs-lookup"><span data-stu-id="d7a69-182">An approval request will expire in 24 hours unless a Microsoft 365 data access approver acts on the request.</span></span> <span data-ttu-id="d7a69-183">Новый запрос отправляется на утверждение каждые 24 часа.</span><span class="sxs-lookup"><span data-stu-id="d7a69-183">A new request will be submitted once every 24 hours for approval.</span></span> <span data-ttu-id="d7a69-184">Если вы видите, что ваше действие копирования ожидает утверждения (на этапе ожидания согласия), в сотрудничестве с утверждающими запросы на доступ к данным Microsoft 365 получите утверждение для вашего запроса.</span><span class="sxs-lookup"><span data-stu-id="d7a69-184">If you see your copy activity waiting for approval (in the Consent Pending stage), then work with Microsoft 365 data access approvers to get your request approved.</span></span>

## <a name="privacy-scrubbing"></a><span data-ttu-id="d7a69-185">Очистка для обеспечения конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="d7a69-185">Privacy scrubbing</span></span>

<span data-ttu-id="d7a69-186">Участник группы утверждающих, который утверждает запрос, может указать имя одной группы пользователей, данные которых будут очищены от извлеченных данных.</span><span class="sxs-lookup"><span data-stu-id="d7a69-186">The member of the approver group who approves the request can specify the name of one user group whose data would be scrubbed out of extracted data.</span></span> <span data-ttu-id="d7a69-187">Строки, содержащие адреса электронной почты, соответствующие участникам запрещенной группы, будут очищены от извлеченных данных.</span><span class="sxs-lookup"><span data-stu-id="d7a69-187">The rows containing email addresses corresponding to the members of the denied group will be scrubbed out of extracted data.</span></span> <span data-ttu-id="d7a69-188">Группы, вложенные в запрещенную группу, будут развернуты, и очистка будет выполняться только для пользователей. Сведения о применении списка запрещенных во время утверждения с помощью PowerShell или пользовательского интерфейса PAM см. в разделе об утверждении запросов в этой статье.</span><span class="sxs-lookup"><span data-stu-id="d7a69-188">Groups nested within the denied group will be expanded and only users will be scrubbed out. Refer to the approving requests section of this topic for details on how to apply the deny list during approval, through either PowerShell or the PAM UX.</span></span>

<span data-ttu-id="d7a69-189">В следующей таблице представлены имена наборов данных и столбцов, для которых выполняется проверка содержимого с целью очистки для обеспечения конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d7a69-189">The following table shows the names of the datasets and the columns for which the contents are checked for privacy scrubbing.</span></span>

| <span data-ttu-id="d7a69-190">Имя набора данных</span><span class="sxs-lookup"><span data-stu-id="d7a69-190">Dataset name</span></span>                                                       | <span data-ttu-id="d7a69-191">Столбцы, используемые для очистки на основе списка запрещенных</span><span class="sxs-lookup"><span data-stu-id="d7a69-191">Columns used for deny list-based scrubbing</span></span>              |
| ------------------------------------------------------------------ | ------------------------------------------------------- |
| <span data-ttu-id="d7a69-192">**BasicDataSet_v0.Message_v0**</span><span class="sxs-lookup"><span data-stu-id="d7a69-192">**BasicDataSet_v0.Message_v0**</span></span><br><span data-ttu-id="d7a69-193">**BasicDataSet_v0.Message_v1**</span><span class="sxs-lookup"><span data-stu-id="d7a69-193">**BasicDataSet_v0.Message_v1**</span></span>   | <span data-ttu-id="d7a69-194">Sender, From, ToRecipients, CcRecipients, BccRecipients</span><span class="sxs-lookup"><span data-stu-id="d7a69-194">Sender, From, ToRecipients, CcRecipients, BccRecipients</span></span> |
| <span data-ttu-id="d7a69-195">**BasicDataSet_v0.SentItem_v0**</span><span class="sxs-lookup"><span data-stu-id="d7a69-195">**BasicDataSet_v0.SentItem_v0**</span></span><br><span data-ttu-id="d7a69-196">**BasicDataSet_v0.SentItem_v1**</span><span class="sxs-lookup"><span data-stu-id="d7a69-196">**BasicDataSet_v0.SentItem_v1**</span></span> | <span data-ttu-id="d7a69-197">Sender, From, ToRecipients, CcRecipients, BccRecipients</span><span class="sxs-lookup"><span data-stu-id="d7a69-197">Sender, From, ToRecipients, CcRecipients, BccRecipients</span></span> |
| <span data-ttu-id="d7a69-198">**BasicDataSet_v0.Event_v0**</span><span class="sxs-lookup"><span data-stu-id="d7a69-198">**BasicDataSet_v0.Event_v0**</span></span><br><span data-ttu-id="d7a69-199">**BasicDataSet_v0.Event_v1**</span><span class="sxs-lookup"><span data-stu-id="d7a69-199">**BasicDataSet_v0.Event_v1**</span></span>       | <span data-ttu-id="d7a69-200">Organizer, Attendees</span><span class="sxs-lookup"><span data-stu-id="d7a69-200">Organizer, Attendees</span></span>                                    |
| <span data-ttu-id="d7a69-201">**BasicDataSet_v0.Contact_v0**</span><span class="sxs-lookup"><span data-stu-id="d7a69-201">**BasicDataSet_v0.Contact_v0**</span></span><br><span data-ttu-id="d7a69-202">**BasicDataSet_v0.Contact_v1**</span><span class="sxs-lookup"><span data-stu-id="d7a69-202">**BasicDataSet_v0.Contact_v1**</span></span>   | <span data-ttu-id="d7a69-203">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="d7a69-203">EmailAddresses</span></span>                                          |
| <span data-ttu-id="d7a69-204">**BasicDataSet_v0.CalendarView_v0**</span><span class="sxs-lookup"><span data-stu-id="d7a69-204">**BasicDataSet_v0.CalendarView_v0**</span></span>                                | <span data-ttu-id="d7a69-205">Organizer, Attendees</span><span class="sxs-lookup"><span data-stu-id="d7a69-205">Organizer, Attendees</span></span>                                    |

## <a name="see-also"></a><span data-ttu-id="d7a69-206">См. также</span><span class="sxs-lookup"><span data-stu-id="d7a69-206">See also</span></span>

- [<span data-ttu-id="d7a69-207">Вопросы и ответы о подключении к данным</span><span class="sxs-lookup"><span data-stu-id="d7a69-207">Data Connect frequently asked questions</span></span>](data-connect-faq.md)
