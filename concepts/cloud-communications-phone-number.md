---
title: Управление номерами телефонов для ботов с помощью API облачной связи
description: Узнайте, как создать бот, доступный по номеру телефона, а также назначить, отменить или обновить номер телефона бота с помощью API облачных коммуникаций Microsoft Graph.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 607fbcb9dd522364ba3e5ec69e80ac2d93ddfe8b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440966"
---
# <a name="manage-phone-numbers-for-bots"></a>Управление номерами телефонов для ботов

В этой статье описывается, как использовать API облачных коммуникаций в Microsoft Graph для создания бота, доступного по номеру телефона. При создании бота будет полезно ознакомиться со следующими терминами:

- **Приложения:** Приложение, размещенное в Azure, также называемом **ботом**.

- **Экземпляр приложения:** Объект отключенного пользователя, который может быть назначен номеру телефона, который может использоваться ботом. Это также называется учетной [записью ресурса](/microsoftteams/manage-resource-accounts). Это единственный способ назначения боту номера телефона.

Одно приложение может иметь несколько экземпляров приложения, а каждый клиент может иметь несколько экземпляров приложения, как показано на следующем рисунке.

![Изображение, показывающее номер телефона с клиентами с одним или несколькими экземплярами приложения](images/communications-app-tenant.PNG)

## <a name="prerequisite-register-a-bot"></a>Предварительные требования: регистрация бота

Чтобы приступить к работе, следуйте инструкциям по [регистрации вызывающего бота](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html). Для использования в коде потребуются такие значения конфигурации, как идентификатор бота, идентификатор приложения Майкрософт и пароль приложения Майкрософт.

Добавьте следующие разрешения в бот. Администратор клиента также должен дать согласие на эти разрешения:

- Calls.AccessMedia.All
- Calls.Initiate.All
- Calls.JoinGroupCall.All
- Calls.JoinGroupCallAsGuest.All

Дополнительные сведения о разрешениях, связанных с вызовами, см. в [справочнике по разрешениям](permissions-reference.md#calls-permissions).

## <a name="assign-a-phone-number-to-your-bot"></a>Назначение боту номера телефона

Назначение боту номера телефона состоит из трех шагов:

1. Создайте экземпляр приложения.
2. Назначьте лицензии Microsoft 365 экземпляру приложения.
3. Назначьте экземпляру приложения номер телефона (только администратор клиента).

### <a name="create-an-application-instance"></a>Создание экземпляра приложения

Если он еще не установлен, администратору клиента необходимо установить модуль Skype для бизнеса [Online](https://www.microsoft.com/download/details.aspx?id=39366) для PowerShell. Перед выполнением командлета администратор клиента должен выполнить вход с использованием своих учетных данных.

Чтобы создать новый экземпляр приложения, администратор клиента выполнит следующий командлет:

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId <app_id> -DisplayName <bot_display_name>`

При создании экземпляра приложения используйте командлет синхронизации:

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

Дополнительные сведения см. в [разделе New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).

### <a name="assign-microsoft-365-licenses-to-your-application-instance"></a>Назначение лицензий Microsoft 365 экземпляру приложения

Назначьте экземпляру приложения лицензию виртуального пользователя. Дополнительные сведения см. в [разделе "Лицензия виртуального пользователя телефонной системы"](/microsoftteams/teams-add-on-licensing/virtual-user).

Назначьте план звонков экземпляру приложения. Дополнительные сведения см [. в разделе "Планы звонков для Microsoft 365"](/microsoftteams/calling-plans-for-office-365).

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a>Назначение номера телефона экземпляру приложения (только администратор клиента)

Прежде чем настраивать телефоны для пользователей в вашей организации, получите для них телефонные номера. Дополнительные сведения см. в [статье "Получение номеров телефонов для пользователей"](/microsoftteams/getting-phone-numbers-for-your-users#get-new-phone-numbers-for-your-users).

Чтобы назначить номер телефона экземпляру приложения, администратор клиента:

1. Войдите в Центр администрирования Teams в качестве администратора клиента.
2. Переходит на **номера голосовых Администратор Teams** >  > **.**
3. Назначает номер телефона службы (+11D) с помощью следующего командлета:

   `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`
  
При присвоении номера телефона службы используйте командлет синхронизации:

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

Дополнительные сведения см. в [разделе Set-CsOnlineVoiceApplicationInstance](/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).

## <a name="unassign-a-bot-phone-number"></a>Отмена назначения номера телефона бота

Чтобы отменить назначение номера телефона, используйте следующий командлет:

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

> [!NOTE]
> В настоящее время это работает только с сетевыми номерами, а не с номерами прямой маршрутизации (DR). Это известная проблема.

## <a name="update-a-bot-phone-number"></a>Обновление номера телефона бота

После отмены назначения номера боту можно назначить другое число с помощью следующего командлета:

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a>См. также

- [Общие сведения об API облачных коммуникаций](cloud-communications-concept-overview.md)
- [Пример бота инцидента](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/V1.0Samples/RemoteMediaSamples/IncidentBot)
- [Развертывание примера](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/V1.0Samples/RemoteMediaSamples/README.md#deploying-the-sample)
