---
title: Обзор групп Microsoft 365 в Microsoft Graph
description: 'Группы Microsoft 365 — фундаментальная служба, которая позволяет пользователям делиться беседами, файлами, заметками, календарями, планами и другими ресурсами. '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.custom: scenarios:getting-started
ms.openlocfilehash: 5539b392b77e7c121e9b69cfea1651d929e010ed00945c28ec783bf8f373da30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146179"
---
# <a name="overview-of-microsoft-365-groups-in-microsoft-graph"></a>Обзор групп Microsoft 365 в Microsoft Graph

Группы Microsoft 365 — фундаментальная служба, которая позволяет пользователям делиться беседами, файлами, заметками, календарями, планами и другими ресурсами. 


> [!VIDEO https://www.youtube-nocookie.com/embed/WB9w6QM9xIU]

## <a name="why-integrate-with-microsoft-365-groups"></a>Зачем выполнять интеграцию с группами Microsoft 365?   

Группы формируют основу для совместной работы пользователей и интеграции различных служб, обеспечивающей поддержку сложных сценариев планирования задач, командной работы, образования и т. д. Интеграция с группами Microsoft 365 позволяет приложению поддерживать миллионы пользователей при переходе между различными службами в наборе Microsoft 365 и за его пределами.  
 
### <a name="create-groups-to-facilitate-teamwork-across-services"></a>Создавайте группы для облегчения командной работы в различных службах 
 
С помощью API Microsoft Graph можно создавать и удалять группы, а также управлять ими в течение всего жизненного цикла совместной работы. Например, вы можете делать следующее:  
 
- Используйте API [создания группы](/graph/api/group-post-groups?view=graph-rest-1.0), чтобы подготовить новую группу. После этого группа становится доступна во множестве приложений, таких как Outlook, SharePoint, Microsoft Teams, Планировщик и даже Microsoft Stream. Microsoft Graph синхронизирует эти взаимосвязанные службы, предоставляя доступ всем участникам группы.  
 
    **Каждая группа Microsoft 365 интегрируется со стандартным набором служб Microsoft 365**

    ![Схема интеграции группы Microsoft 365 с файлами, заметками, задачами, сайтами, беседами и календарем](images/office365-groups-concept-overview-related-services-infographic.png)  

- Предоставьте участникам возможность добавить группу в [избранное](/graph/api/group-addfavorite?view=graph-rest-1.0) или [удалить ее из избранного](/graph/api/group-removefavorite?view=graph-rest-1.0) по своему желанию. 
- [Создавайте](/graph/api/group-post-conversations?view=graph-rest-1.0), [получайте](/graph/api/group-get-conversation?view=graph-rest-1.0) или [удаляйте](/graph/api/group-delete-conversation?view=graph-rest-1.0) беседы группы из собственного приложения. 
- Планируйте [события](/graph/api/resources/event?view=graph-rest-1.0) в календаре группы. 
- Получайте сведения о [сайте SharePoint](/graph/api/resources/site?view=graph-rest-1.0), связанном с группой, например [дочерних сайтах](/graph/api/site-list-subsites?view=graph-rest-1.0) или [списках](/graph/api/list-list?view=graph-rest-1.0) библиотеки документов. 
- [Создайте план](/graph/api/planner-post-buckets?view=graph-rest-1.0), принадлежащий группе, с помощью Планировщика. План позволяет визуально отслеживать командную работу, [создавая задачи](/graph/api/planner-post-tasks?view=graph-rest-1.0), которые можно [упорядочивать по сегментам](/graph/api/planner-post-buckets?view=graph-rest-1.0). 
- Получите доступ к связанной с группой записной книжке [OneNote](/graph/api/resources/onenote?view=graph-rest-1.0), в которой можно собирать примечания к собраниям и упорядочивать идеи. 
  
    **Группы Microsoft 365 и беседы в Outlook в Интернете**

    ![Снимок экрана Outlook в Интернете с группами в папке "Группы"](images/office365-groups-concept-overview-groups-in-outlook.png) 

- [Разрешите участникам группы](/graph/api/team-put-teams?view=graph-rest-beta) общаться в сохраняемом чате Microsoft Teams (ознакомительная версия).  
- [Удаляйте группы](/graph/api/group-delete?view=graph-rest-1.0). При удалении группы также удаляется все связанное с нею содержимое, что позволяет избежать образования потерянных сайтов, бесед и планов. 
 
### <a name="manage-group-membership-seamlessly"></a>Легко управляйте членством в группах 
 
Группы Microsoft 365 — это коллекции пользователей с совместным доступом к ресурсам в службах Майкрософт или приложении. Так как управление членством в группах централизовано, все изменения членства влияют на все службы, связанные с группой. Используйте Microsoft Graph, чтобы выполнять следующие задачи с членством в группах:
 
- [Добавляйте](/graph/api/group-post-members?view=graph-rest-1.0) и [удаляйте](/graph/api/group-delete-members?view=graph-rest-1.0) участников существующей группы. 
- Получайте [список владельцев](/graph/api/group-list-owners?view=graph-rest-1.0) или [участников](/graph/api/group-list-members?view=graph-rest-1.0) группы. Это помогает понять, кому доступно содержимое группы и кто может исполнять обязанности администратора, например обновлять группы или утверждать запросы на присоединение. 
- Делайте группы **общедоступными** (содержимое группы видно всем пользователям в организации) или **частными** (содержимое группы видно только участникам) с помощью операции [обновления группы](/graph/api/group-update?view=graph-rest-1.0). 
- [Удаляйте владельцев](/graph/api/group-delete-owners?view=graph-rest-1.0), больше не исполняющих свои обязанности для определенной группы, из списка владельцев группы. 
 
### <a name="establish-and-maintain-group-policy-settings"></a>Устанавливайте параметры групповой политики 
 
По мере роста количества групп, создаваемых в организации, с помощью Microsoft Graph можно управлять использованием и жизненным циклом группы. Вы можете применять групповые политики ко всем группам в организации. Используйте API Microsoft Graph, чтобы выполнять следующие задачи:

- Настраивайте [параметры групповых политик](/graph/api/resources/groupsetting?view=graph-rest-1.0), которые помогают определить поведение, например автоматическое удаление групп, не обновленных владельцем, и применение политик именования к группам Microsoft 365. 
- [Обновляйте](/graph/api/group-renew?view=graph-rest-1.0) группы, срок действия которых подходит к концу, чтобы участники группы могли продолжить совместную работу и доступ к содержимому. Если группа не будет обновлена в соответствии с установленной политикой срока действия, она будет автоматически удалена. 
- [Восстанавливайте](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0) удаленные группы.

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API групп в Microsoft Graph версии 1.0](/graph/api/resources/groups-overview?view=graph-rest-1.0)
- [API групп в бета-версии Microsoft Graph](/graph/api/resources/groups-overview?view=graph-rest-beta)


## <a name="next-steps"></a>Дальнейшие действия

- Опробуйте примеры запросов API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer). 
- Узнайте больше об [использовании API групп](/graph/api/resources/groups-overview?view=graph-rest-1.0) в Microsoft Graph.
