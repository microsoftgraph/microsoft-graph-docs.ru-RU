---
title: Настройка параметров поведения и подготовки групп Microsoft 365
description: Ресурс group в Microsoft Graph позволяет задать определенное поведение и подготовить ресурсы при создании групп Microsoft 365.
author: yyuank
localization_priority: Priority
ms.openlocfilehash: 066ef0c65fa0b70fd89fc5dfc4cf14e047f1bc49
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034151"
---
# <a name="set-microsoft-365-group-behaviors-and-provisioning-options-preview"></a>Настройка параметров поведения и подготовки групп Microsoft 365 (предварительная версия)

Ресурс [group](/graph/api/resources/group?view=graph-rest-beta) в Microsoft Graph позволяет задать определенное поведение и подготовить ресурсы при создании групп Microsoft 365. В зависимости от ресурса, некоторые из них также можно подготовить при обновлении группы.

### <a name="configuring-and-provisioning-groups"></a>Настройка и подготовка групп

Ресурс **group** предоставляет два свойства, **resourceBehaviorOptions** и **resourceProvisioningOptions**, для настройки поведения и подготовки ресурсов при создании группы. 

> [!NOTE]
> В настоящее время свойства **resourceBehaviorOptions** и **resourceProvisioningOptions** доступны только в конечной точке бета-версии Microsoft Graph. Не используйте эти свойства в рабочих приложениях, так как они могут быть изменены без предварительного уведомления.

Свойство **resourceBehaviorOptions** — это набор строк, определяющих поведение групп Microsoft 365. Поведение группы можно задать только при [ее создании](/graph/api/group-post-groups?view=graph-rest-beta) (`POST`).

| Поддерживаемые значения для resourceBehaviorOptions   |Описание|Значение по умолчанию, если не задано иное|
|:---------------|:--------|:-----------|
| AllowOnlyMembersToPost|Только *члены* группы могут публиковать беседы в группе.|Любой пользователь в организации может публиковать беседы в группе.|
| HideGroupInOutlook|Эта группа скрыта в интерфейсе Outlook.|Все группы отображаются и доступны для обнаружения в интерфейсе Outlook.|
| SubscribeNewGroupMembers|Участники группы подписаны на получение сообщений групповых бесед. |Участники группы не получают сообщений групповых бесед.|
| WelcomeEmailDisabled|Новым участникам группы не отправляются приветственные письма.|При вступлении в группу новому участнику отправляется приветственное письмо.|

Свойство **resourceProvisioningOptions** — это набор строк, определяющих ресурсы, которые необходимо подготовить при создании группы Microsoft 365 и которые, как правило, не являются частью создания группы по умолчанию.

| Поддерживаемые значения для resourceProvisioningOptions   |Описание| Значение по умолчанию, если не задано иное |
|:---------------|:--------|:------------|
| Teams|Подготовка этой группы в качестве команды в Microsoft Teams. Кроме того, это значение можно добавить в набор строк **resourceProvisioningOptions** при [обновлении группы](/graph/api/group-update?view=graph-rest-beta) с помощью операции `PATCH`, чтобы преобразовать существующую группу Microsoft 365 в команду.| Эта группа является стандартной группой Microsoft 365 без возможностей Teams.|


## <a name="see-also"></a>См. также

- [Обзор групп Microsoft 365 в Microsoft Graph](office365-groups-concept-overview.md)
- [Обзор API Microsoft Teams](teams-concept-overview.md)
