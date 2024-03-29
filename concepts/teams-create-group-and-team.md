---
title: Создавайте команды и управляйте участниками с помощью API Microsoft Teams.
description: Используйте API Microsoft Teams в Microsoft Graph, чтобы создавать команды несколькими способами, добавлять участников и управлять ими, а также проверять свои результаты.
author: hachandr
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: a5f57cba104e9b9f89f07556d4708960f5ee5c0d
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555662"
---
# <a name="create-teams-and-manage-members-using-the-microsoft-teams-api"></a>Создавайте команды и управляйте участниками с помощью API Microsoft Teams.

Вы можете использовать API Microsoft Teams и Microsoft Graph, чтобы создавать команды разными способами. В этой статье описан рекомендуемый подход для достижения наилучших результатов.


## <a name="create-a-team"></a>Создание команды

В основе всех команд лежат группы Microsoft 365. Самый быстрый способ начать работу при создании команд посредством Microsoft Graph — настроить новую группу Microsoft 365, всех ее владельцев и участников, а затем преобразовать ее в команду.

1. Создайте группу [Microsoft 365](https://support.office.com/article/learn-about-office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2) с помощью операции [создания группы](/graph/api/group-post-groups). Вы можете указать владельцев и участников. Убедитесь в наличии соответствующих владельцев для только что созданной группы, как описано в шаге 2.

    Чтобы создать команду для этой группы, установите следующие значения свойств, как показано ниже.

    - **groupTypes** = { "Unified" } 
    - **mailEnabled** = true
    - **securityEnabled** = false

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

    Ниже показан пример отклика. 

    >**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

    ```http
    HTTP/1.1 200 OK
    Content-type: application/json
 
    {
        "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
        "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
    }
    ```

2. Обеспечьте для группы наличие двух или более владельцев. Это можно сделать с помощью операции [добавления владельца](/graph/api/group-post-owners). Они должны быть реальными учетными записями пользователей, а не учетными записями служб. Наличие двух владельцев помогает обслуживать сценарии, когда один владелец покидает компанию или недоступен для выполнения операций управления командой.

3. Добавьте всех участников (и гостей при необходимости) в группу с помощью операции [добавления участника](/graph/api/group-post-members), если это не сделано на шаге 1. При добавлении нескольких участников добавьте 1-секундную задержку после каждой операции добавления. 

4. После успешного создания группы, что может занять до 15 минут после выполнения шага 1, создайте команду Microsoft Teams с помощью операции [создания команды из группы](/graph/api/team-post#example-4-create-a-team-from-group). Если вы столкнулись с ошибкой, процесс создания группы, возможно, не завершен. Попробуйте подождать несколько минут. 

    ```http
    POST https://graph.microsoft.com/v1.0/teams
    Content-Type: application/json
    {
      "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
      "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('groupId')"
    }
    ```

    Ниже показан пример отклика. 

    >**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

    ```http
    HTTP/1.1 202 Accepted
    Content-Type: application/json
    Location: /teams/{teamId}/operations/{operationId}
    Content-Location: /teams/{teamId}
    {
    }
    ```

    Идентификатор созданной команды такой же, как и идентификатор группы.

5. После завершения этого процесса все владельцы и участники должны увидеть созданную команду в клиенте Teams.

## <a name="add-or-manage-members"></a>Добавление участников и управление ими

Чтобы добавить участников после создания команды, используйте операцию [добавления участника](/graph/api/group-post-members). Рекомендуем добавить 1-секундную задержку между операциями добавления. Учитывайте следующее касательно изменений участия:

1. Изменения участия, внесенные в группу Microsoft 365, синхронизируются с Teams с помощью фонового механизма синхронизации, который обычно занимает 24 часа (или больше в некоторых случаях).

2. Фоновый процесс запускается, если один или несколько пользователей команды (владелец или участник) активны в классическом клиенте Teams. Активность заключается в запуске приложения Teams и/или его работе. Пользователю не требуется специально посещать команду, которая изменяется.

    > [!NOTE]
    > Мобильные клиенты Teams не запускают синхронизацию членства. По крайней мере, один пользователь должен быть в настольном клиенте, чтобы обеспечить бесперебойную работу этого фонового процесса.

## <a name="checklist-for-validation"></a>Контрольный список для проверки

После создания команды вы можете воспользоваться следующим контрольным списком, чтобы проверить успешность создания команды.

### <a name="validate-team-creation"></a>Проверка создания команды

1. Убедитесь, что создана группа Microsoft 365, дублирующая команду, с помощью Центров администрирования Azure AD или Microsoft 365.

2. Убедитесь, что команда успешно создана, в портале администрирования Teams.

3. Проверьте, что у команды есть соответствующие владельцы и участники, с помощью портала администрирования Teams.

4. Убедитесь, что владельцы команды видят команду после входа в классический или веб-клиент Teams.

5. Убедитесь, что участники видят команду после входа в классический или веб-клиент Teams.

### <a name="validate-addition-of-members"></a>Проверка добавления участников

1. Проверьте, что новые участники отображаются в группе, с помощью Центра администрирования Azure AD или Microsoft 365.

2. Убедитесь, что добавленные участники видят команду после входа в классический или веб-клиент Teams.

## <a name="see-also"></a>См. также

- [Обзор API Microsoft Teams](teams-concept-overview.md)