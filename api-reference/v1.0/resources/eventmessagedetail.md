---
title: тип ресурса eventMessageDetail
description: Представляет сведения о сообщении о событии системы.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ec2d6e8af1faecb92fb73b2fd04150c7fd29eb00
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322618"
---
# <a name="eventmessagedetail-resource-type"></a>тип ресурса eventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении о событии системы.

Системные сообщения — это сообщения, [](../resources/conversationMember.md) созданные для  таких событий, как участники, добавленные в [канал,](../resources/channel.md)участники, добавленные в [чат,](../resources/chat.md)и [обновленное](../resources/team.md) описание команды.

Список поддерживаемых событий

| Событие | Описание |
| :---- | :---------- |
| [callEndedEventMessageDetail](../resources/callStartedEventMessageDetail.md) | Вызов завершен. |
| [callRecordingEventMessageDetail](../resources/callRecordingEventMessageDetail.md) | Запись вызова доступна. |
| [callStartedEventMessageDetail](../resources/callStartedEventMessageDetail.md) | Вызов начался. |
| [callTranscriptEventMessageDetail](../resources/callTranscriptEventMessageDetail.md) | Имеется запись вызова. |
| [channelAddedEventMessageDetail](../resources/channelAddedEventMessageDetail.md) | Добавлен **канал.** |
| [channelDeletedEventMessageDetail](../resources/channelDeletedEventMessageDetail.md) | Канал  удален. |
| [channelDescriptionUpdatedEventMessageDetail](../resources/channelDescriptionUpdatedEventMessageDetail.md) | **Описание канала** обновлено. |
| [channelRenamedEventMessageDetail](../resources/channelRenamedEventMessageDetail.md) | Канал **переименован.** |
| [channelSetAsFavoriteByDefaultEventMessageDetail](../resources/channelSetAsFavoriteByDefaultEventMessageDetail.md) | Канал **по** умолчанию настроен как любимый. |
| [channelUnsetAsFavoriteByDefaultEventMessageDetail](../resources/channelUnsetAsFavoriteByDefaultEventMessageDetail.md) | Канал **по** умолчанию не установлен как любимый. |
| [chatRenamedEventMessageDetail](../resources/chatRenamedEventMessageDetail.md) | Чат переименован. |
| [conversationMemberRoleUpdatedEventMessageDetail](../resources/conversationMemberRoleUpdatedEventMessageDetail.md) | Роль была обновлена для **участника**. |
| [meetingPolicyUpdatedEventMessageDetail](../resources/meetingPolicyUpdatedEventMessageDetail.md) | Обновлена политика собраний. |
| [membersAddedEventMessageDetail](../resources/membersAddedEventMessageDetail.md) | **Добавлены** участники. |
| [membersDeletedEventMessageDetail](../resources/membersDeletedEventMessageDetail.md) | **Участники** удалены. |
| [membersJoinedEventMessageDetail](../resources/membersJoinedEventMessageDetail.md) | **Участники** присоединились. |
| [membersLeftEventMessageDetail](../resources/membersLeftEventMessageDetail.md) | **Участники** ушли. |
| [tabUpdatedEventMessageDetail](../resources/tabUpdatedEventMessageDetail.md) | Вкладка обновлена. |
| [teamArchivedEventMessageDetail](../resources/teamArchivedEventMessageDetail.md) | Команда **архивов.** |
| [teamCreatedEventMessageDetail](../resources/teamCreatedEventMessageDetail.md) | Создана  команда. |
| [teamDescriptionUpdatedEventMessageDetail](../resources/teamDescriptionUpdatedEventMessageDetail.md) | **Описание команды** обновлено. |
| [teamJoiningDisabledEventMessageDetail](../resources/teamJoiningDisabledEventMessageDetail.md) | **Присоединение** к команде отключено. |
| [teamJoiningEnabledEventMessageDetail](../resources/teamJoiningEnabledEventMessageDetail.md) | **Присоединение** к команде включено. |
| [teamRenamedEventMessageDetail](../resources/teamRenamedEventMessageDetail.md) | Команда **переименована.** |
| [teamsAppInstalledEventMessageDetail](../resources/teamsAppInstalledEventMessageDetail.md) | [Teams установлено](../resources/teamsApp.md) приложение. |
| [teamsAppRemovedEventMessageDetail](../resources/teamsAppRemovedEventMessageDetail.md) | **Teams приложение** удалено. |
| [teamsAppUpgradedEventMessageDetail](../resources/teamsAppUpgradedEventMessageDetail.md) | **Teams приложение** было обновлено. |
| [teamUnarchivedEventMessageDetail](../resources/teamUnarchivedEventMessageDetail.md) | Команда  была невечена. |

## <a name="properties"></a>Свойства
Отсутствуют.



## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eventMessageDetail"
}
```

