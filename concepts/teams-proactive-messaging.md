---
title: Упреждающий обмен сообщениями с помощью Bot в Microsoft Teams
description: Перед отправкой упреждающего сообщения пользователю Microsoft Teams с помощью настраиваемого приложения сначала необходимо установить Bot с помощью Microsoft Graph.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: dafd70f1d741f15b2cfe52efe7f0a4942f06f3bd
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288940"
---
# <a name="proactive-messaging-using-a-bot-in-microsoft-teams"></a>Упреждающий обмен сообщениями с помощью Bot в Microsoft Teams

Упреждающее сообщение — это сообщение, отправляемое пользователю Microsoft Teams без инициации беседы пользователем. Пользовательские приложения в Microsoft Teams могут отправлять активные сообщения пользователям с помощью программы Bot. Тем не менее, для этого необходимо установить робот в качестве личного приложения или в команду, членом которой является пользователь. Это требование может быть недопустимым в сценариях, в которых необходимо заблаговременно заданное сообщение для группы пользователей, у которых может быть установлено приложение Teams.

В этой статье рассказывается, как можно объединить Microsoft Graph с приложением Microsoft Teams, чтобы установить приложение для пользователей, а затем использовать приложение Teams для отправки им упреждающего сообщения без необходимости вручную устанавливать приложение.

На высоком уровне необходимо выполнить следующие действия:

* [Создание приложения Teams и программы Bot](#create-your-teams-app-and-bot)
* [Развертывание приложения в каталоге приложений клиента](#deploy-your-app-to-your-tenant-app-catalog)
* [Установка приложения для пользователей](#install-the-app-for-your-users)

## <a name="create-your-teams-app-and-bot"></a>Создание приложения Teams и программы Bot

Если у вас еще нет приложения Microsoft Teams с роботом, который может отправить сообщение, необходимо создать его. В документации по платформе Teams вы можете ознакомиться с разделом [Add Боты to Apps to Teams](/microsoftteams/platform/concepts/bots/bots-overview) . Сведения о создании почтового робота для упреждающего обмена сообщениями можно узнать в статье [профилактической системы обмена сообщениями для Боты](/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive).

Вы также можете использовать [шаблон приложения Communicator компании](https://github.com/OfficeDev/microsoft-teams-company-communicator-app) в качестве хорошей отправной точки для вашего приложения. Этот шаблон приложения — это готовое приложение Microsoft Teams, которое может создавать, планировать и распространять сообщения всей компании.

При создании приложения убедитесь, что вы заметите, что вы `id` используете его в манифесте приложения; вам потребуется установить приложение на следующем этапе.

Если вы делаете это для большой организации, приветственные сообщения от ленты смогут регулироваться. Если это возможно, выполните установку в пакетах и реализуйте функции обратной передачи в интерфейсе Bot. Подробнее: [ограничение скорости обработки](/microsoftteams/platform/concepts/bots/rate-limit).

## <a name="deploy-your-app-to-your-tenant-app-catalog"></a>Развертывание приложения в каталоге приложений клиента

Microsoft Graph может устанавливать только приложения, добавленные в каталог приложений клиента, или доступные в общедоступном магазине приложений Microsoft Teams. При работе с новым приложением необходимо убедиться в том, что он является [каталогом приложений клиента](/microsoftteams/platform/publishing/apps-publish#microsoft-teams-tenant-app-catalog).

## <a name="install-the-app-for-your-users"></a>Установка приложения для пользователей

Чтобы установить приложение Teams для пользователей, сначала необходимо убедиться, что приложение Microsoft Graph имеет необходимые разрешения — вам потребуется User. ReadWrite. ALL или Directory. ReadWrite. ALL, чтобы установить приложение Teams. Кроме того, вам потребуется чат. Read. ALL для последующего этапа. Для обоих разрешений требуется согласие администратора, и вам потребуется использовать разрешения приложения, а не делегирования пользователя, так как вы будете устанавливать приложения для пользователей, отличных от самого себя.

### <a name="check-to-see-if-the-app-is-already-installed"></a>Проверка того, установлено ли приложение

Сначала необходимо проверить, установлено ли приложение Teams для тех пользователей, которые вы хотите установить, как показано в примере.

```http
GET /users/{user-id}/teamwork/installedApps?$expand=teamsAppDefinition&$filter=teamsAppDefinition/teamsAppId eq '{teamsAppid}'
```

Где `{teamsAppId}` — это `id` манифест приложения Teams, который вы внесли ранее. Обратите внимание, что это может отличаться от `appid` вызовов Microsoft Graph, а также от `botId` . Может потребоваться вручную установить приложение для пользователя и протестировать вызов для этого пользователя, чтобы убедиться, что вы получили правильное `id` значение.

Вызов возвратит пустой массив, если приложение не установлено, или массив с одним [теамсаппинсталлатион](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) , если он уже установлен.

### <a name="install-the-app"></a>Установка приложения

Если приложение еще не установлено для этого пользователя, его можно установить, как показано в следующем примере.

```http
POST /users/{user-id}/teamwork/installedApps
{
   "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppid}"
}
```

Для получения дополнительных сведений обратитесь [к разделу Установка приложения для пользователя](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta).

Если у пользователя есть запущенные Microsoft Teams, то, возможно, они не увидят установки приложения, поэтому для его установки может потребоваться перезапустить приложение.

## <a name="get-the-chat-thread-id"></a>Получение идентификатора потока чата

Когда приложение устанавливается для пользователя, Bot получит `conversationUpdate` событие, которое будет содержать необходимые сведения для отправки упреждающего сообщения. Дополнительные сведения: [события Bot](/microsoftteams/platform/concepts/bots/bots-notifications).

Если вы потеряли его `chatThreadId` , вы сможете снова найти его, вызвав:

```http
GET /users/{user-id}/chats?$filter=installedApps/any(a:a/teamsApp/id eq '{teamsAppid}')
```

Свойство **ID** результата — идентификатор chatThread.

## <a name="sending-the-message"></a>Отправка сообщения

Теперь, когда у ленты есть необходимые сведения, вы можете [Отправить упреждающее сообщение](/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive).

## <a name="c-sample"></a>Пример кода на языке C#

В разделе https://github.com/microsoftgraph/contoso-airlines-teams-sample/tree/nkramer-promsg (Обратите внимание на ветвь).
Интересный код находится в `InstallAppToAllUsers()` [GraphService.CS](https://github.com/microsoftgraph/contoso-airlines-teams-sample/blob/nkramer-promsg/project/Models/GraphService.cs).