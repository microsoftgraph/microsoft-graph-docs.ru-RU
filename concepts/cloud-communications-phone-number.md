---
title: Управление номерами телефонов для ботов
description: В этой статье описывается создание бота, который можно достичь с помощью номера телефона.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: d6b71d2db1be951137ca33026f243dae6055c93f
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573574"
---
# <a name="manage-phone-numbers-for-bots"></a>Управление номерами телефонов для ботов 

В этой статье описывается создание бота, который можно достичь с помощью номера телефона. При создании бота будет полезно ознакомиться со следующими терминами:

- **Application** — приложение, которое находится в Azure, также именуемом **ботом.**

- **Пример приложения** — объект с отключенным пользователем, который может быть назначен номеру телефона, который может использоваться ботом. Это также называется учетной [записью ресурса.](/microsoftteams/manage-resource-accounts) Это единственный способ присвоения номера телефона боту.

Одно приложение может иметь несколько экземпляров приложений, а каждый клиент может иметь несколько экземпляров приложений, как показано на следующем изображении.

![Изображение, на котором показан номер телефона с клиентом с одним или более экземплярами приложений](images/communications-app-tenant.PNG)

## <a name="prerequisite---register-a-bot"></a>Обязательное условие — регистрация бота
Чтобы начать работу, следуйте инструкциям по регистрации [вызываемого бота.](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html) Для использования в коде вам потребуется использовать конфигуративные значения, такие как код бота, код приложения Майкрософт и пароль приложения Майкрософт.

Добавьте следующие разрешения в бот. Администратору клиента также необходимо дать согласие на эти разрешения:

- Calls.AccessMedia.All
- Calls.Initiate.All
- Calls.JoinGroupCall.All
- Calls.JoinGroupCallAsGuest.All

Дополнительные сведения о разрешениях, связанных с вызовами, см. в справке [Permissions.](permissions-reference.md#calls-permissions)


## <a name="assign-a-phone-number-to-your-bot"></a>Назначение номера телефона боту

Назначение номера телефона боту включает в себя три действия:

1.  Создание экземпляра приложения.
2.  Назначение лицензий Microsoft 365 экземпляру приложения.
3.  Назначьте номер телефона экземпляру приложения (только администратору клиента).

### <a name="create-an-application-instance"></a>Создание экземпляра приложения

Если он еще не установлен, администратору клиента необходимо установить [модуль Skype для бизнеса Online для](https://www.microsoft.com/download/details.aspx?id=39366) PowerShell. Администратор клиента должен войти с помощью учетных данных перед запуском cmdlet.

Чтобы создать новый экземпляр приложения, администратор клиента запускает следующий кодлет.

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId <app_id> -DisplayName <bot_display_name>`

При создания экземпляра приложения используйте комлет синхронизации.

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

Дополнительные сведения см. [в new-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)

### <a name="assign-microsoft-365-licenses-to-your-application-instance"></a>Назначение лицензий Microsoft 365 экземпляру приложения

Назначение виртуальной пользовательской лицензии экземпляру приложения. Подробные сведения см. в [материале Phone system virtual user license.](/microsoftteams/teams-add-on-licensing/virtual-user)

Назначение плана вызова экземпляру приложения. Подробные сведения [см. в материале Calling plans for Microsoft 365.](/microsoftteams/calling-plans-for-office-365)

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a>Назначение номера телефона экземпляру приложения (только администратору клиента)

Прежде чем выполнить настройку пользователей в пределах своей организации на осуществление и прием звонков, необходимо получить телефонные номера для них. Подробные сведения см. [в материале Получение номеров телефонов для пользователей.](/microsoftteams/getting-phone-numbers-for-your-users#get-new-phone-numbers-for-your-users)

Чтобы назначить номер телефона экземпляру приложения, администратор клиента:

1. Войт в центр администрирования Teams в качестве администратора клиента.
2. Переходит на **номера голосовых телефонов Центра**  >    >  **администрирования** Teams.
3. Назначает номер телефона службы (+11D-формат) с помощью следующего cmdlet.

  `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`
  
При присвоении номера телефона службы используйте комлет синхронизации.

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

Дополнительные сведения см. [в рублях Set-CsOnlineVoiceApplicationInstance](/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)

## <a name="unassign-a-bot-phone-number"></a>Отозвание номера телефона бота

Чтобы отогнать номер телефона, используйте следующий комдлет.

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

>**Примечание:** В настоящее время это работает только с онлайн-номерами, а не с номерами прямой маршрутики (DR). Это известная проблема.

## <a name="update-a-bot-phone-number"></a>Обновление номера телефона бота

После отвода номера можно назначить боту другой номер с помощью следующего cmdlet.

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a>См. также

- [Пример бота инцидента](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot). 
 - Дополнительные сведения о развертывании см. в [примере Deploying the sample.](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample)
