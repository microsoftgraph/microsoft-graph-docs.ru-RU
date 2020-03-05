---
title: Тип ресурса Онпремисеспублишингпрофиле
description: Тип ресурса Онпремисеспублишингпрофиле.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 94d09955ad20af1117b156e433c95f2914df7348
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522202"
---
# <a name="onpremisespublishingprofile-resource-type"></a>Тип ресурса Онпремисеспублишингпрофиле

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Различные службы Azure (например, сквозная проверка подлинности подключения Azure Active Directory, подготовка пользователей рабочего дня к Azure AD) обеспечивают условный доступ к различным локальным ресурсам извне корпоративной сети. [Локальные агенты](onpremisesagent.md) , установленные администратором клиента, можно настроить для доступа к определенному [опубликованному ресурсу](publishedresource.md)или обработки запросов.
[Группы агентов](onpremisesagentgroup.md) позволяют администратору клиента назначать определенные агенты для обслуживания определенных опубликованных локальных ресурсов. Администраторы клиентов могут объединить несколько агентов в группу, а затем назначить каждый опубликованный ресурс группе. Весь набор сущностей одного локального типа публикации представлен **онпремисеспублишингпрофиле**.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Онпремисеспублишингпрофиле](../api/onpremisespublishingprofile-get.md) | [онпремисеспублишингпрофиле](onpremisespublishingprofile.md) | Чтение свойств и связей объекта **онпремисеспублишингпрофиле** . |
| [Обновление Онпремисеспублишингпрофиле](../api/onpremisespublishingprofile-update.md) | Нет | Обновление объекта [онпремисеспублишингпрофиле](onpremisespublishingprofile.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|хибридажентупдатерконфигуратион|[хибридажентупдатерконфигуратион](hybridagentupdaterconfiguration.md)| Представляет объект **хибридажентупдатерконфигуратион** .|
|id|String| Представляет тип публикации. Возможные значения: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`. Только для чтения.|

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|ажентграупс|Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)| Список существующих объектов **онпремисесажентграуп** . Только для чтения. Допускается значение null.|
|агенты|Коллекция [онпремисесажент](onpremisesagent.md)| Список существующих объектов **онпремисесажент** . Только для чтения. Допускается значение null.|
|публишедресаурцес|Коллекция [публишедресаурце](publishedresource.md)| Список существующих объектов **публишедресаурце** . Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "hybridAgentUpdaterConfiguration": {"@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
