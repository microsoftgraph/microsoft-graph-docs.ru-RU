---
title: Тип ресурса eventMessageDetail
description: Представляет сведения о сообщении системного события.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c5874d48789dc1145a47b74c6788adb735a253d1
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398814"
---
# <a name="eventmessagedetail-resource-type"></a>Тип ресурса eventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении системного события.

Системные сообщения — это сообщения, создаваемые для таких [](../resources/conversationMember.md) событий, как [участники,](../resources/channel.md) добавленные в **канал, участники**, добавленные в [чат](../resources/chat.md), и [обновленное описание](../resources/team.md) команды.

Список поддерживаемых событий

| Событие | Описание |
| :---- | :---------- |
| [callEndedEventMessageDetail](../resources/callEndedEventMessageDetail.md) | Вызов завершен. |
| [callRecordingEventMessageDetail](../resources/callRecordingEventMessageDetail.md) | Доступна запись звонка. |
| [callStartedEventMessageDetail](../resources/callStartedEventMessageDetail.md) | Вызов запущен. |
| [callTranscriptEventMessageDetail](../resources/callTranscriptEventMessageDetail.md) | Доступна расшифровка звонка. |
| [channelAddedEventMessageDetail](../resources/channelAddedEventMessageDetail.md) | Канал **добавлен** . |
| [channelDeletedEventMessageDetail](../resources/channelDeletedEventMessageDetail.md) | **Канал удален**. |
| [channelDescriptionUpdatedEventMessageDetail](../resources/channelDescriptionUpdatedEventMessageDetail.md) | **Описание канала** обновлено. |
| [channelRenamedEventMessageDetail](../resources/channelRenamedEventMessageDetail.md) | Канал **переименован** . |
| [channelSetAsFavoriteByDefaultEventMessageDetail](../resources/channelSetAsFavoriteByDefaultEventMessageDetail.md) | Канал **по** умолчанию настроен как избранный. |
| [channelUnsetAsFavoriteByDefaultEventMessageDetail](../resources/channelUnsetAsFavoriteByDefaultEventMessageDetail.md) | Канал **по** умолчанию не задан как избранный. |
| [chatRenamedEventMessageDetail](../resources/chatRenamedEventMessageDetail.md) | Чат переименован. |
| [conversationMemberRoleUpdatedEventMessageDetail](../resources/conversationMemberRoleUpdatedEventMessageDetail.md) | Роль обновлена для **члена**. |
| [meetingPolicyUpdatedEventMessageDetail](../resources/meetingPolicyUpdatedEventMessageDetail.md) | Политика собраний обновлена. |
| [membersAddedEventMessageDetail](../resources/membersAddedEventMessageDetail.md) | **Добавлены** члены. |
| [membersDeletedEventMessageDetail](../resources/membersDeletedEventMessageDetail.md) | **Элементы** удалены. |
| [membersJoinedEventMessageDetail](../resources/membersJoinedEventMessageDetail.md) | **Участники** присоединились. |
| [membersLeftEventMessageDetail](../resources/membersLeftEventMessageDetail.md) | **Участники** слева. |
| [tabUpdatedEventMessageDetail](../resources/tabUpdatedEventMessageDetail.md) | Вкладка обновлена. |
| [teamArchivedEventMessageDetail](../resources/teamArchivedEventMessageDetail.md) | Команда **архивирована** . |
| [teamCreatedEventMessageDetail](../resources/teamCreatedEventMessageDetail.md) | Команда **создана** . |
| [teamDescriptionUpdatedEventMessageDetail](../resources/teamDescriptionUpdatedEventMessageDetail.md) | **Описание команды** обновлено. |
| [teamJoiningDisabledEventMessageDetail](../resources/teamJoiningDisabledEventMessageDetail.md) | **Присоединение** к команде отключено. |
| [teamJoiningEnabledEventMessageDetail](../resources/teamJoiningEnabledEventMessageDetail.md) | **Присоединение** к команде включено. |
| [teamRenamedEventMessageDetail](../resources/teamRenamedEventMessageDetail.md) | Команда **переименована** . |
| [teamsAppInstalledEventMessageDetail](../resources/teamsAppInstalledEventMessageDetail.md) | [Teams установлено](../resources/teamsApp.md) приложение. |
| [teamsAppRemovedEventMessageDetail](../resources/teamsAppRemovedEventMessageDetail.md) | **Teams приложение** удалено. |
| [teamsAppUpgradedEventMessageDetail](../resources/teamsAppUpgradedEventMessageDetail.md) | **Teams приложение** было обновлено. |
| [teamUnarchivedEventMessageDetail](../resources/teamUnarchivedEventMessageDetail.md) | Команда **была** неархивна. |

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

