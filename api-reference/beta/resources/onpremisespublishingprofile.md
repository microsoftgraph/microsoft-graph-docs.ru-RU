---
title: onPremisesPublishingProfile type
description: onPremisesPublishingProfile.
ms.localizationpriority: medium
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 2d984b304b47005db4de02d920cacc37ba21fb3c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125083"
---
# <a name="onpremisespublishingprofile-resource-type"></a>onPremisesPublishingProfile type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Различные службы Azure (например, Azure Active Directory Подключение проверки подлинности [passthrough,](/azure/active-directory/hybrid/how-to-connect-pta)подготовка рабочих [](/azure/active-directory/app-proxy/what-is-application-proxy) дней для пользователей [Azure AD](/azure/active-directory/saas-apps/workday-inbound-tutorial)и прокси-серверы приложений позволяют получать доступ к различным локальному ресурсу из-за пределов корпоративной сети.

[Локальное агенты](onpremisesagent.md) (или [соединители](connector.md) для прокси-серверов приложений), установленные администратором, могут быть настроены для маршрутов запросов на определенный [опубликованный ресурс.](publishedresource.md)
[Группы агентов](onpremisesagentgroup.md) [(или](connectorgroup.md) соединители группы для application Proxy) позволяют администратору назначать определенных агентов для обслуживания определенных опубликованных локально ресурсов. Администраторы также могут сгруппить несколько агентов вместе, а затем назначить каждый опубликованный ресурс группе агентов. Весь набор сущностями одного и того же локального типа публикации представлен **onPremisesPublishingProfile.**

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md) | [onPremisesPublishingProfile](onpremisespublishingprofile.md) | Ознакомьтесь с свойствами и отношениями **объекта onPremisesPublishingProfile.** |
| [Обновление наPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md) | Нет | Обновление [объекта onPremisesPublishingProfile.](onpremisespublishingprofile.md) |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](hybridagentupdaterconfiguration.md)| Представляет объект **hybridAgentUpdaterConfiguration.**|
|id|Строка| Представляет тип публикации. Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`. Только для чтения.|
|isEnabled|Boolean| Представляет, включен [ли прокси-сервер приложения Azure AD](/azure/active-directory/app-proxy/what-is-application-proxy) для клиента. |

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|agentGroups|[коллекция onPremisesAgentGroup](onpremisesagentgroup.md)| Список существующих **объектов onPremisesAgentGroup.** Только для чтения. Допускается значение null.|
|агенты|[коллекция onPremisesAgent](onpremisesagent.md)| Список существующих **объектов наPremisesAgent.** Только для чтения. Допускается значение null.|
|connectorGroups|[коллекция connectorGroup](connectorgroup.md)| Список существующих **объектов connectorGroup** для приложений, опубликованных через application Proxy. Только для чтения. Допускается значение null.|
|connectors|[коллекция соединители](connector.md)| Список существующих объектов **соединитений** для приложений, опубликованных через Application Proxy. Только для чтения. Допускается значение null.|
|publishedResources|[коллекция publishedResource](publishedresource.md)| Список существующих **объектов publishedResource.** Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
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