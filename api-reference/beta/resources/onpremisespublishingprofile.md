---
title: Тип ресурса Онпремисеспублишингпрофиле
description: Тип ресурса Онпремисеспублишингпрофиле.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4299ddec6a05e079d86a070b939c2220087281a0
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921531"
---
# <a name="onpremisespublishingprofile-resource-type"></a>Тип ресурса Онпремисеспублишингпрофиле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Различные службы Azure (например, [сквозная проверка подлинности](/azure/active-directory/hybrid/how-to-connect-pta)подключения Azure Active Directory, подключение [рабочего дня к пользователям Azure AD](/azure/active-directory/saas-apps/workday-inbound-tutorial)и [прокси приложения](https://aka.ms/whyappproxy) — предоставление доступа к различным локальным ресурсам извне корпоративной сети).

[Локальные агенты](onpremisesagent.md) (или [соединители](connector.md) для прокси-сервера приложения), установленные администратором, могут быть настроены на маршрутизацию запросов на конкретный [опубликованный ресурс](publishedresource.md).
[Группы агентов](onpremisesagentgroup.md) (или [группы соединителей](connectorgroup.md) для прокси приложения) позволяют администратору назначать определенные агенты для обслуживания определенных опубликованных локальных ресурсов. Администраторы также могут группировать несколько агентов вместе, а затем назначать каждый опубликованный ресурс группе агентов. Весь набор сущностей одного локального типа публикации представлен **онпремисеспублишингпрофиле**.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Онпремисеспублишингпрофиле](../api/onpremisespublishingprofile-get.md) | [онпремисеспублишингпрофиле](onpremisespublishingprofile.md) | Чтение свойств и связей объекта **онпремисеспублишингпрофиле** . |
| [Обновление Онпремисеспублишингпрофиле](../api/onpremisespublishingprofile-update.md) | Нет | Обновление объекта [онпремисеспублишингпрофиле](onpremisespublishingprofile.md) . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|хибридажентупдатерконфигуратион|[хибридажентупдатерконфигуратион](hybridagentupdaterconfiguration.md)| Представляет объект **хибридажентупдатерконфигуратион** .|
|id|String| Представляет тип публикации. Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`. Только для чтения.|
|isEnabled|Boolean| Указывает, включен ли [прокси приложения Azure AD](https://aka.ms/whyappproxy) для клиента. |

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|ажентграупс|Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)| Список существующих объектов **онпремисесажентграуп** . Только для чтения. Допускается значение null.|
|агенты|Коллекция [онпремисесажент](onpremisesagent.md)| Список существующих объектов **онпремисесажент** . Только для чтения. Допускается значение null.|
|коннекторграупс|Коллекция [коннекторграуп](connectorgroup.md)| Список существующих объектов **коннекторграуп** для приложений, опубликованных через прокси приложения. Только для чтения. Допускается значение null.|
|аудиовыход|Коллекция [соединителей](connector.md)| Список существующих объектов **Connector** для приложений, опубликованных через прокси приложения. Только для чтения. Допускается значение null.|
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


