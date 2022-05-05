---
title: Использование внешних групп для управления разрешениями на доступ к источникам данных соединителей Graph Майкрософт
description: Внешние группы позволяют управлять разрешениями на просмотр внешних элементов в microsoft Graph и подключение к источникам данных за пределами Azure AD групп.
author: mecampos
doc_type: conceptualPageType
ms.prod: search
ms.localizationpriority: medium
ms.openlocfilehash: 17b6b37da6f91f08cf7397b52880bb2235dc430a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211027"
---
# <a name="use-external-groups-to-manage-permissions-to-microsoft-graph-connectors-data-sources"></a>Использование внешних групп для управления разрешениями на доступ к источникам данных соединителей Graph Майкрософт

[Внешние](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-1.0&preserve-view=true) группы позволяют управлять разрешениями на просмотр [](/graph/api/resources/externalconnectors-externalitem?view=graph-rest-1.0&preserve-view=true) внешних элементов в microsoft Graph подключения и подключения к источникам данных за пределами Azure Active Directory (Azure AD).

Для источников данных, которые зависят от Azure AD пользователей и групп, разрешения для внешних элементов задается путем связывания списка управления доступом (ACL) с идентификатором пользователя Azure AD и группы при создании или обновлении внешних элементов.[](/graph/api/externalconnectors-externalconnection-put-items?view=graph-rest-beta&preserve-view=true&tabs=http&viewFallbackFrom=graph-rest-1.0)

Однако для источников данных, использующих не Azure AD группы или конструкции, подобные группам, таким как Профили Salesforce, Dynamics Business Units, группы SharePoint, локальные группы ServiceNow или локальные группы Confluence, рекомендуется использовать внешние *группы*.

## <a name="common-external-group-scenarios"></a>Распространенные сценарии внешних групп

Ниже приведены распространенные примеры групп Azure AD приложения.

Microsoft Dynamics 365 позволяет клиентам структурировать свои CRM с помощью бизнес-подразделений и команд.Сведения о членстве для этих подразделений и команд не хранятся в Azure AD.

На следующем рисунке показана структура бизнес-подразделений и команд.

<!---Using html to adjust the size of the image --->
<br><p align="center"><img src="images/connectors-images/bu-teams-D365.png" alt="Diagram of a structure in Dynamics 365. A business unit has a team and a manager under it. This manager has other users." width="400px;"/></p>

Salesforce использует профили, роли и наборы разрешений для авторизации. Они относятся только к Salesforce, и сведения о членстве недоступны в Azure AD.

На следующем рисунке показана структура сведений о членстве в Salesforce.

<!---Using html to adjust the size of the image --->
<br><p align="center"><img src="images/connectors-images/roles-salesforce.png" alt="Diagram of a structure of roles in Salesforce. The role of vice president of sales is at the top level of the hierarchy and has three subordinates, namely, the head of sales operations, the head of sales, and the head of account management. The head of sales operations has a sales operations manager as a subordinate. The head of sales has a sales development manager as a subordinate." width="500px;"/></p>

## <a name="using-external-groups-in-your-connection"></a>Использование внешних групп в подключении

Чтобы использовать внешние группы в подключении, выполните следующие действия.

1. Для каждой группы, Azure AD группы, используйте API групп для создания внешней группы в Microsoft Graph.
2. При необходимости используйте внешнюю группу при определении списка ACL для внешних элементов.
3. Следите за тем, чтобы членство внешних групп было актуальным и синхронизированным.

### <a name="create-an-external-group"></a>Создание внешней группы

Внешние группы принадлежат к подключению. Чтобы создать внешние группы в подключениях, выполните следующие действия.

1. Используйте [API групп](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) в Microsoft Graph, как показано в следующем примере.

    > [!NOTE]
    > [DisplayName и](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-1.0&preserve-view=true#properties) **описание являются** необязательными полями.

    ```http
    POST /external/connections/{connectionId}/groups

    { 
      "id": "contosoEscalations", 
      "displayName": "Contoso Escalations", 
      "description": "Tier-1 escalations within Contoso"
    } 
    ```

2. Укажите идентификатор или имя в поле идентификатора. Используйте это значение для вызова внешней группы в последующих запросах.

    > [!NOTE]
    > Поле идентификатора позволяет использовать URL-адрес и безопасные наборы символов Base64 с именами файлов. Он имеет ограничение в 128 символов.

    Внешняя группа может содержать один или несколько из следующих элементов:
    * Пользователь Azure AD.
    * Группа Azure AD.
    * Другая внешняя группа, включая вложенные внешние группы.

3. После создания группы можно добавить в нее участников, как показано в следующих примерах.
    
    ```http
    POST https://graph.microsoft.com/beta/external/connections/{connectionId}/groups/{groupId}/members
    
    {
      "id": "contosoSupport",
      "type": "group",
      "identitySource": "external"
    }
    ```
    ```http
    POST https://graph.microsoft.com/beta/external/connections/{connectionId}/groups/{groupId}/members
    
    {
      "id": "25f143de-be82-4afb-8a57-e032b9315752",
      "type": "user",
      "identitySource": "azureActiveDirectory"
    }
    ```
    ```http
    POST https://graph.microsoft.com/beta/external/connections/{connectionId}/groups/{groupId}/members
    
    {
      "id": "99a3b3d6-71ee-4d21-b08b-4b6f22e3ae4b",
      "type": "group",
      "identitySource": "azureActiveDirectory"
    }
    ```

### <a name="use-external-groups-in-the-acl"></a>Использование внешних групп в ACL

Внешние группы можно использовать при определении [списков ACL](connecting-external-content-manage-items.md#access-control-list) для внешних элементов, как показано в следующем примере. Помимо Azure AD пользователей и групп внешний элемент может содержать внешние группы в записях управления доступом.

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
> Внешние группы можно использовать в списках ACL еще до их создания.

### <a name="keep-external-group-memberships-in-sync"></a>Синхронизация членства во внешних группах

Поддержив актуальное членство внешней группы в Microsoft Graph. При изменении членства в пользовательской группе убедитесь, что это изменение отражается во внешней группе в то время, которое подходит для ваших потребностей.

### <a name="manage-external-groups-and-membership"></a>Управление внешними группами и членством

Вы можете использовать API групп для управления внешними группами и членством в группах. Дополнительные сведения см. [в разделе externalGroup](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-1.0&preserve-view=true) и [externalGroupMember](/graph/api/resources/externalconnectors-externalgroupmember?view=graph-rest-beta&preserve-view=true&viewFallbackFrom=graph-rest-1.0).

## <a name="next-steps"></a>Дальнейшие действия

- [Сведения об ограничениях API соединителей Graph Майкрософт](connecting-external-content-api-limits.md)
- [Работа с API соединителей Microsoft Graph](connecting-external-content-connectors-api-overview.md)
- [Использование Postman с API соединителей Microsoft Graph](connecting-external-content-connectors-api-postman.md)
