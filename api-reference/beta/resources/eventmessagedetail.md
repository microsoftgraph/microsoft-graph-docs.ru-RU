---
title: тип ресурса eventMessageDetail
description: Представляет базовый тип для детализации сообщений событий.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da40b7413bc52a2ec0d663e2b7e0467f0e5e06fd
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535815"
---
# <a name="eventmessagedetail-resource-type"></a>тип ресурса eventMessageDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Этот абстрактный тип представляет сведения о сообщении события системы.

Системные сообщения — это сообщения, созданные для таких событий, как участники, добавленные в канал, участники, добавленные в чат, и обновленное описание команды.

Список поддерживаемых событий

| Событие | Описание |
| :---- | :---------- |
| [callEndedEventMessageDetail](../resources/callStartedEventMessageDetail.md) | Вызов завершен. |
| [callRecordingEventMessageDetail](../resources/callRecordingEventMessageDetail.md) | Запись вызова доступна. |
| [callStartedEventMessageDetail](../resources/callStartedEventMessageDetail.md) | Вызов начался. |
| [callTranscriptEventMessageDetail](../resources/callTranscriptEventMessageDetail.md) | Имеется запись вызова. |
| [channelAddedEventMessageDetail](../resources/channelAddedEventMessageDetail.md) | Добавлен канал. |
| [channelDeletedEventMessageDetail](../resources/channelDeletedEventMessageDetail.md) | Канал удален. |
| [channelDescriptionUpdatedEventMessageDetail](../resources/channelDescriptionUpdatedEventMessageDetail.md) | Описание канала обновлено. |
| [channelRenamedEventMessageDetail](../resources/channelRenamedEventMessageDetail.md) | Канал переименован. |
| [channelSetAsFavoriteByDefaultEventMessageDetail](../resources/channelSetAsFavoriteByDefaultEventMessageDetail.md) | Канал по умолчанию настроен как любимый. |
| [channelUnsetAsFavoriteByDefaultEventMessageDetail](../resources/channelUnsetAsFavoriteByDefaultEventMessageDetail.md) | Канал по умолчанию не установлен как любимый. |
| [chatRenamedEventMessageDetail](../resources/chatRenamedEventMessageDetail.md) | Чат переименован. |
| [conversationMemberRoleUpdatedEventMessageDetail](../resources/conversationMemberRoleUpdatedEventMessageDetail.md) | Роль была обновлена для участника. |
| [meetingPolicyUpdatedEventMessageDetail](../resources/meetingPolicyUpdatedEventMessageDetail.md) | Обновлена политика собраний. |
| [membersAddedEventMessageDetail](../resources/membersAddedEventMessageDetail.md) | Добавлены участники. |
| [membersDeletedEventMessageDetail](../resources/membersDeletedEventMessageDetail.md) | Участники удалены. |
| [membersJoinedEventMessageDetail](../resources/membersJoinedEventMessageDetail.md) | Участники присоединились. |
| [membersLeftEventMessageDetail](../resources/membersLeftEventMessageDetail.md) | Участники ушли. |
| [tabUpdatedEventMessageDetail](../resources/tabUpdatedEventMessageDetail.md) | Вкладка обновлена. |
| [teamArchivedEventMessageDetail](../resources/teamArchivedEventMessageDetail.md) | Команда архивов. |
| [teamCreatedEventMessageDetail](../resources/teamCreatedEventMessageDetail.md) | Создана команда. |
| [teamDescriptionUpdatedEventMessageDetail](../resources/teamDescriptionUpdatedEventMessageDetail.md) | Описание команды обновлено. |
| [teamJoiningDisabledEventMessageDetail](../resources/teamJoiningDisabledEventMessageDetail.md) | Присоединение к команде отключено. |
| [teamJoiningEnabledEventMessageDetail](../resources/teamJoiningEnabledEventMessageDetail.md) | Присоединение к команде включено. |
| [teamRenamedEventMessageDetail](../resources/teamRenamedEventMessageDetail.md) | Команда переименована. |
| [teamsAppInstalledEventMessageDetail](../resources/teamsAppInstalledEventMessageDetail.md) | Teams установлено приложение. |
| [teamsAppRemovedEventMessageDetail](../resources/teamsAppRemovedEventMessageDetail.md) | Teams приложение удалено. |
| [teamsAppUpgradedEventMessageDetail](../resources/teamsAppUpgradedEventMessageDetail.md) | Teams приложение было обновлено. |
| [teamUnarchivedEventMessageDetail](../resources/teamUnarchivedEventMessageDetail.md) | Команда была невечена. |

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

