---
title: Настройка параметров поведения и подготовки групп Microsoft 365
description: Ресурс group в Microsoft Graph позволяет задать определенное поведение и подготовить ресурсы при создании групп Microsoft 365.
author: Jordanndahl
ms.localizationpriority: high
ms.openlocfilehash: 3844be2abb14909c8af18af4206c0b655fe42612
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804600"
---
# <a name="set-microsoft-365-group-behaviors-and-provisioning-options"></a>Настройка параметров поведения и подготовки групп Microsoft 365

Ресурс [group](/graph/api/resources/group) в Microsoft Graph позволяет задать определенное поведение и подготовить ресурсы при создании групп Microsoft 365. В зависимости от ресурса, некоторые из них также можно подготовить при обновлении группы.

### <a name="configuring-and-provisioning-groups"></a>Настройка и подготовка групп

Ресурс **group** предоставляет два свойства, **resourceBehaviorOptions** и **resourceProvisioningOptions**, для настройки поведения и подготовки ресурсов при создании группы. 

Свойство **resourceBehaviorOptions** — это набор строк, определяющих поведение групп Microsoft 365. Поведение группы можно задать только при [ее создании](/graph/api/group-post-groups) (`POST`).

| Поддерживаемые значения для resourceBehaviorOptions   |Описание|Значение по умолчанию, если не задано иное|
|:---------------|:--------|:-----------|
| AllowOnlyMembersToPost|Только *члены* группы могут публиковать беседы в группе.|Любой пользователь в организации может публиковать беседы в группе.|
| HideGroupInOutlook|Эта группа скрыта в интерфейсе Outlook.|Все группы отображаются и доступны для обнаружения в интерфейсе Outlook.|
| SubscribeNewGroupMembers|Участники группы подписаны на получение сообщений групповых бесед. |Участники группы не получают сообщений групповых бесед.|
| WelcomeEmailDisabled|Новым участникам группы не отправляются приветственные письма.|При вступлении в группу новому участнику отправляется приветственное письмо.|

**resourceProvisioningOptions** — это коллекция строк, указывающая ресурсы группы, которые необходимо подготовить в рамках группы Microsoft 365. Эти ресурсы можно указать во время создания или обновления группы.

| Поддерживаемые значения для resourceProvisioningOptions   |Описание| Значение по умолчанию, если не задано иное |
|:---------------|:--------|:------------|
| Команда|Подготовка этой группы в качестве команды в Microsoft Teams. Кроме того, это значение можно добавить при [обновлении группы](/graph/api/group-update) с помощью операции `PATCH`, чтобы подготовить команду из существующей группы Microsoft 365.| Эта группа является стандартной группой Microsoft 365 без возможностей Teams.|


## <a name="see-also"></a>См. также

- [Обзор групп Microsoft 365 в Microsoft Graph](office365-groups-concept-overview.md)
- [Обзор API Microsoft Teams](teams-concept-overview.md)
