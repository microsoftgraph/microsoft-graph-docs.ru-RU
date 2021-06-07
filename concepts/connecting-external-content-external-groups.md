---
title: Использование внешних групп для управления разрешениями для источников данных Graph соединители Microsoft
description: Узнайте о внешних группах для управления разрешениями для внешних элементов.
author: mecampos
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 8a0ae00e7fc4d1509c29bfb204aae0ab3166970e
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781195"
---
# <a name="use-external-groups-to-manage-permissions-to-microsoft-graph-connector-data-sources"></a><span data-ttu-id="84400-103">Использование внешних групп для управления разрешениями для источников данных Graph соединители Microsoft</span><span class="sxs-lookup"><span data-stu-id="84400-103">Use external groups to manage permissions to Microsoft Graph connector data sources</span></span>

<span data-ttu-id="84400-104">[Внешние](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) группы позволяют управлять разрешениями для просмотра внешних элементов в подключении Microsoft Graph и подключения к источникам данных за пределами Azure Active Directory (Azure AD). [](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="84400-104">[External groups](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) allow you to manage permissions to view [external items](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) in a Microsoft Graph connection, and connect to data sources outside Azure Active Directory (Azure AD) groups.</span></span>

<span data-ttu-id="84400-105">Для источников данных, которые зависят от пользователей и групп Azure AD, при создании или обновлении внешних элементов устанавливаются разрешения [](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true) на внешние элементы, связывая список управления доступом (ACL) с пользователем Azure AD и групповым ИД.</span><span class="sxs-lookup"><span data-stu-id="84400-105">For data sources that rely on Azure AD users and groups, you set permissions on external items by associating an access control list (ACL) with an Azure AD user and group ID, when [creating](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true) or updating the external items.</span></span>

<span data-ttu-id="84400-106">Однако для источников данных, которые используют группы не Azure AD или групповые конструкции, такие как Профили Salesforce, Dynamics Business Units, SharePoint группы, локальные группы ServiceNow или локальные группы Confluence, рекомендуется использовать внешние *группы.*</span><span class="sxs-lookup"><span data-stu-id="84400-106">However, for data sources that use non-Azure AD groups, or group-like constructs, like Salesforce Profiles, Dynamics Business Units, SharePoint groups, ServiceNow local groups, or Confluence local groups, we recommend that you use *external groups*.</span></span>

## <a name="common-external-group-scenarios"></a><span data-ttu-id="84400-107">Общие внешние групповые сценарии</span><span class="sxs-lookup"><span data-stu-id="84400-107">Common external group scenarios</span></span>

<span data-ttu-id="84400-108">Ниже приводится ряд примеров групп, не относящуюся к приложениям Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84400-108">The following are common non-Azure AD application-specific group examples.</span></span>

<span data-ttu-id="84400-109">Microsoft Dynamics 365 позволяет клиентам структурировать свои ЦПМ с бизнес-подразделениями и группами.</span><span class="sxs-lookup"><span data-stu-id="84400-109">Microsoft Dynamics 365 allows customers to structure their CRMs with business units and teams.</span></span><span data-ttu-id="84400-110">Сведения о членстве для этих бизнес-подразделений и групп не хранятся в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84400-110"> The membership information for these business units and teams is not stored in Azure AD.</span></span>

<span data-ttu-id="84400-111">На следующем изображении показана структура бизнес-подразделений и групп.</span><span class="sxs-lookup"><span data-stu-id="84400-111">The following image shows the structure of the business units and teams.</span></span>

<!---Using html to adjust the size of the image --->
<br><p align="center"><img src="images/connectors-images/bu-teams-D365.png" alt="Diagram of an structure in Dynamics 365. A business unit has a team and a manager under it. This manager has other users." style="width:400px;"/></p>

<span data-ttu-id="84400-112">Salesforce использует профили, роли и наборы разрешений для авторизации.</span><span class="sxs-lookup"><span data-stu-id="84400-112">Salesforce uses profiles, roles, and permission sets for authorization.</span></span> <span data-ttu-id="84400-113">Они специфичествеен для Salesforce, а сведения о членстве недоступны в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84400-113">These are specific to Salesforce, and the membership information is not available in Azure AD.</span></span>

<span data-ttu-id="84400-114">На следующем изображении показана структура сведений о членстве в Salesforce.</span><span class="sxs-lookup"><span data-stu-id="84400-114">The following image shows the structure of the membership information in Salesforce.</span></span>

<!---Using html to adjust the size of the image --->
<br><p align="center"><img src="images/connectors-images/roles-salesforce.png" alt="Diagram of an structure of roles in Salesforce. The role of vicepresident of sales is at the top level of the hierarchy, it has three subordinates, namely, the head of sales operations, the head of sales, and the head of account managament. The head of sales at the same time has a sales operations manager as subordinate. And the head of sales has a sales development manager as subordinate." style="width:400px;"/></p>

## <a name="using-external-groups-in-your-connection"></a><span data-ttu-id="84400-115">Использование внешних групп в подключении</span><span class="sxs-lookup"><span data-stu-id="84400-115">Using external groups in your connection</span></span>

<span data-ttu-id="84400-116">Использование внешних групп в подключениях:</span><span class="sxs-lookup"><span data-stu-id="84400-116">To use external groups in your connections:</span></span>

1. <span data-ttu-id="84400-117">Для каждой группы, не влияемой на Azure AD, создайте внешнюю группу в Microsoft Graph с помощью [API групп.](/en-us/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="84400-117">For each non-Azure AD group, create an external group in Microsoft Graph using the [groups API](/en-us/graph/api/resources/group?view=graph-rest-beta&preserve-view=true).</span></span>
2. <span data-ttu-id="84400-118">Используйте внешнюю группу при определении ACL для внешних элементов по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="84400-118">Use the external group when defining the ACL for your external items as necessary.</span></span>  
3. <span data-ttu-id="84400-119">Следите за тем, чтобы членство внешних групп было в курсе и синхронизируется.</span><span class="sxs-lookup"><span data-stu-id="84400-119">Keep the membership of the external groups up to date and in sync.</span></span>

### <a name="create-external-groups"></a><span data-ttu-id="84400-120">Создание внешних групп</span><span class="sxs-lookup"><span data-stu-id="84400-120">Create external groups</span></span>

<span data-ttu-id="84400-121">Внешние группы относятся к подключению.</span><span class="sxs-lookup"><span data-stu-id="84400-121">External groups belong to a connection.</span></span> <span data-ttu-id="84400-122">Создание внешних групп в подключениях:</span><span class="sxs-lookup"><span data-stu-id="84400-122">To create external groups in your connections:</span></span>
* <span data-ttu-id="84400-123">Используйте API групп в Microsoft Graph, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="84400-123">Use the groups API in Microsoft Graph, as shown in the following example.</span></span>

    > [!NOTE]
    > <span data-ttu-id="84400-124">[DisplayName и](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) **описание являются** необязательными полями.</span><span class="sxs-lookup"><span data-stu-id="84400-124">The [displayName](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) and **description** are optional fields.</span></span>

    ```http
    POST /connections/{connectionId}/groups 

    {  
      "id": "contosoEscalations",  
      "displayName": "Contoso Escalations",  
      "description": "Tier-1 escalations within Contoso"
    }  
    ```

* <span data-ttu-id="84400-125">Предоставление идентификатора или имени в поле [ID.](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="84400-125">Provide either an identifier or a name in the [ID](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) field.</span></span> <span data-ttu-id="84400-126">Используйте это значение для вызова внешней группы в последующих запросах.</span><span class="sxs-lookup"><span data-stu-id="84400-126">Use this value to call the external group in subsequent requests.</span></span>

    > [!NOTE]
    > <span data-ttu-id="84400-127">Поле ID позволяет использовать наборы символов Base64, безопасных для URL-адресов и файлов, и имеет ограничение в 128 символов.</span><span class="sxs-lookup"><span data-stu-id="84400-127">The ID field allows you to use URL and filename-safe Base64 character sets, and it has a limit of 128 characters.</span></span>

<span data-ttu-id="84400-128">Внешняя группа может содержать одну или несколько следующих групп:</span><span class="sxs-lookup"><span data-stu-id="84400-128">An external group can contain one or more of the following:</span></span>
* <span data-ttu-id="84400-129">Пользователь Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84400-129">An Azure AD user.</span></span>
* <span data-ttu-id="84400-130">Группа Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84400-130">An Azure AD group.</span></span>
* <span data-ttu-id="84400-131">Другая внешняя группа, в том числе вложенные внешние группы.</span><span class="sxs-lookup"><span data-stu-id="84400-131">Another external group, including nested external groups.</span></span>

<span data-ttu-id="84400-132">После создания группы можно добавить членов в группу, как показано в следующих примерах.</span><span class="sxs-lookup"><span data-stu-id="84400-132">After you create the group, you can add members to the group, as shown in the following examples.</span></span>

```http
POST https://graph.microsoft.com/beta/connections/{connectionId}/groups/{groupId}/members

{ 
  "id": "contosoSupport", 
  "type": "group", 
  "identitySource": "external" 
}
```
```http
POST https://graph.microsoft.com/beta/connections/{connectionId}/groups/{groupId}/members 

{ 
  "id": "25f143de-be82-4afb-8a57-e032b9315752", 
  "type": "user", 
  "identitySource": "azureActiveDirectory" 
}
```
```http
POST https://graph.microsoft.com/beta/connections/{connectionId}/groups/{groupId}/members 

{ 
  "id": "99a3b3d6-71ee-4d21-b08b-4b6f22e3ae4b", 
  "type": "group", 
  "identitySource": "azureActiveDirectory" 
}
```

### <a name="use-external-groups-in-acl"></a><span data-ttu-id="84400-133">Использование внешних групп в ACL</span><span class="sxs-lookup"><span data-stu-id="84400-133">Use external groups in ACL</span></span>

<span data-ttu-id="84400-134">Внешние группы можно использовать при определении [ALS](connecting-external-content-manage-items.md#access-control-list) для внешних элементов, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="84400-134">You can use external groups when defining [ACLs](connecting-external-content-manage-items.md#access-control-list) for external items, as shown in the following example.</span></span> <span data-ttu-id="84400-135">Помимо пользователей и групп Azure AD внешний элемент может иметь внешние группы в записях управления доступом.</span><span class="sxs-lookup"><span data-stu-id="84400-135">In addition to Azure AD users and groups, an external item can have external groups in its access control entries.</span></span>

```http
PUT https://graph.microsoft.com/beta/external/connections/{id}/items/{id}  

Content-type: application/json  
{  
  "@odata.type": "microsoft.graph.externalItem",  
  "acl": [  
    {  
      "type": "group",  
      "value": "contosEscalations",  
      "accessType": "grant",  
      "identitySource": "External"  
    },  
    {  
      "type": "user",  
      "value": "87e9089a-08d5-4d9e-9524-b7bd6be580d5",  
      "accessType": "grant",  
      "identitySource": "azureActiveDirectory"  
    },  
    {  
      "type": "group",  
      "value": "96fbeb4f-f71c-4405-9f0b-1d6988eda2d2",  
      "accessType": "deny",  
      "identitySource": "azureActiveDirectory"  
    }  
  ],  
  "properties": {  
    "title": "Error in the payment gateway",  
    "priority": 1,  
    "assignee": "john@contoso.com"  
  },  
  "content": {  
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>",  
    "type": "html"  
  }  
}  
```

> [!NOTE]
> <span data-ttu-id="84400-136">Внешние группы в acLs можно использовать еще до создания групп.</span><span class="sxs-lookup"><span data-stu-id="84400-136">You can use external groups in ACLs even before the groups are created.</span></span>

### <a name="keep-external-group-memberships-in-sync"></a><span data-ttu-id="84400-137">Синхронизируйте внешние члены группы</span><span class="sxs-lookup"><span data-stu-id="84400-137">Keep external group memberships in sync</span></span>

<span data-ttu-id="84400-138">Сохранение членства вашей внешней группы в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="84400-138">Keep the membership of your external group up to date in Microsoft Graph.</span></span> <span data-ttu-id="84400-139">При изменении членства в настраиваемой группе убедитесь, что изменение отражается во внешней группе в то время, которое работает для ваших потребностей.</span><span class="sxs-lookup"><span data-stu-id="84400-139">When memberships change in your custom group, make sure that the change is reflected in the external group at a time that works for your needs.</span></span>

### <a name="manage-external-groups-and-membership"></a><span data-ttu-id="84400-140">Управление внешними группами и членством</span><span class="sxs-lookup"><span data-stu-id="84400-140">Manage external groups and membership</span></span>

<span data-ttu-id="84400-141">API групп можно использовать для управления внешними группами и членством в группе.</span><span class="sxs-lookup"><span data-stu-id="84400-141">You can use the groups API to manage your external groups and group membership.</span></span> <span data-ttu-id="84400-142">Подробнее см. в [материале externalGroup](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) и [externalGroupMember.](/graph/api/resources/externalgroupmember?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="84400-142">For details, see [externalGroup](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) and [externalGroupMember](/graph/api/resources/externalgroupmember?view=graph-rest-beta&preserve-view=true).</span></span>

## <a name="see-also"></a><span data-ttu-id="84400-143">См. также</span><span class="sxs-lookup"><span data-stu-id="84400-143">See also</span></span>
<span data-ttu-id="84400-144">Дополнительные информацию об API Graph соединителов Майкрософт см. в этой ссылке [Работа с API соединителов.](connecting-external-content-connectors-api-overview.md)</span><span class="sxs-lookup"><span data-stu-id="84400-144">To learn more about the Microsoft Graph connectors API, see [Working with the connectors API](connecting-external-content-connectors-api-overview.md).</span></span>
